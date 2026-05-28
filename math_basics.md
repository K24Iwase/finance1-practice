# 数学の基礎

経済学で使う数学をまとめました。トグルを開いて確認してください。

---

## 微分

<details>
<summary>📖 基本ルール（クリックして展開）</summary>

### 基本公式

| 関数 | 導関数 |
|------|--------|
| $f(x) = c$（定数） | $f'(x) = 0$ |
| $f(x) = x^n$ | $f'(x) = nx^{n-1}$ |
| $f(x) = cf(x)$ | $(cf)'= cf'$ |
| $f(x)+g(x)$ | $f'+g'$ |
| $f(x)\cdot g(x)$ | $f'g + fg'$（積の微分） |
| $f(g(x))$ | $f'(g(x))\cdot g'(x)$（合成関数の微分） |

### 例題

$$f(x) = 3x^2 + 2x \Rightarrow f'(x) = 6x + 2$$

$$f(x) = (2x+1)^3 \Rightarrow f'(x) = 3(2x+1)^2 \cdot 2 = 6(2x+1)^2$$

</details>

---

## 偏微分

<details>
<summary>📖 偏微分のやり方（クリックして展開）</summary>

### 考え方

複数の変数がある関数で、**1つの変数だけに注目して微分**し、他の変数は定数として扱う。

### 記号

$f(x, y)$ を $x$ で偏微分：$\dfrac{\partial f}{\partial x}$ または $f_x$

### 例題

$$f(x, y) = x^2 y + 3xy^2$$

$$\frac{\partial f}{\partial x} = 2xy + 3y^2 \quad\text{（$y$ は定数として扱う）}$$

$$\frac{\partial f}{\partial y} = x^2 + 6xy \quad\text{（$x$ は定数として扱う）}$$

### 経済学での使い方

効用関数 $u(x, y) = x^{1/2}y^{1/2}$ の限界効用：

$$MU_x = \frac{\partial u}{\partial x} = \frac{1}{2}x^{-1/2}y^{1/2} = \frac{\sqrt{y}}{2\sqrt{x}}$$

$$MU_y = \frac{\partial u}{\partial y} = \frac{1}{2}x^{1/2}y^{-1/2} = \frac{\sqrt{x}}{2\sqrt{y}}$$

</details>

---

## 全微分

<details>
<summary>📖 全微分のやり方（クリックして展開）</summary>

### 考え方

関数 $z = f(x, y)$ で $x$ と $y$ が両方少し変化したとき、$z$ の変化量を求める。

$$dz = \frac{\partial f}{\partial x}dx + \frac{\partial f}{\partial y}dy$$

### 使い方（無差別曲線の傾き）

効用 $u = f(x, y)$ を一定（$du = 0$）に保つとき：

$$du = \frac{\partial u}{\partial x}dx + \frac{\partial u}{\partial y}dy = 0$$

$$\Rightarrow \frac{dy}{dx} = -\frac{\partial u/\partial x}{\partial u/\partial y} = -\frac{MU_x}{MU_y} = -MRS$$

**→ 無差別曲線の傾き = $-MRS$（限界代替率）**

### 例題

$u = xy$、$du=0$ のとき：

$$y\,dx + x\,dy = 0 \Rightarrow \frac{dy}{dx} = -\frac{y}{x}$$

</details>

---

## 最大化・最小化の条件

<details>
<summary>📖 最適化の立式（クリックして展開）</summary>

### 1変数の最大化

$$\max_x f(x)$$

**手順：**
1. $f'(x) = 0$ を解く → 候補点 $x^*$
2. $f''(x^*) < 0$ なら最大（山型）

**例：** $f(x) = 80x - 2x^2$

$$f'(x) = 80 - 4x = 0 \Rightarrow x^* = 20$$
$$f''(x) = -4 < 0 \quad\checkmark\text{（最大）}$$

### 2変数の最大化（制約なし）

$$\max_{x,y} f(x, y)$$

**手順：**
1. $\dfrac{\partial f}{\partial x} = 0$ と $\dfrac{\partial f}{\partial y} = 0$ を連立して解く

</details>

---

## ラグランジュ乗数法

<details>
<summary>📖 制約付き最大化の解き方（クリックして展開）</summary>

### 問題の形

$$\max_{x,y}\; f(x,y) \quad\text{s.t.}\quad g(x,y) = c$$

### 手順

**Step 1：** ラグランジュ関数を作る

$$\mathcal{L} = f(x,y) - \lambda\bigl(g(x,y)-c\bigr)$$

**Step 2：** 3つの偏微分 = 0 の連立方程式を解く

$$\frac{\partial \mathcal{L}}{\partial x} = 0,\quad \frac{\partial \mathcal{L}}{\partial y} = 0,\quad \frac{\partial \mathcal{L}}{\partial \lambda} = 0$$

**Step 3：** 連立方程式を解いて $x^*, y^*$ を求める

> **重要：** $\partial\mathcal{L}/\partial\lambda = 0$ は制約条件 $g(x,y)=c$ そのもの。

---

### 例題：消費者の効用最大化

$$\max_{x,y}\; u = x^{1/2}y^{1/2} \quad\text{s.t.}\quad p_x x + p_y y = I$$

ラグランジュ関数：

$$\mathcal{L} = x^{1/2}y^{1/2} - \lambda(p_x x + p_y y - I)$$

各変数で偏微分 = 0：

$$\frac{\partial \mathcal{L}}{\partial x} = \frac{1}{2}x^{-1/2}y^{1/2} - \lambda p_x = 0 \quad\cdots(1)$$

$$\frac{\partial \mathcal{L}}{\partial y} = \frac{1}{2}x^{1/2}y^{-1/2} - \lambda p_y = 0 \quad\cdots(2)$$

$$\frac{\partial \mathcal{L}}{\partial \lambda} = -(p_x x + p_y y - I) = 0 \quad\cdots(3)$$

$(1)\div(2)$：

$$\frac{y}{x} = \frac{p_x}{p_y} \Rightarrow p_y y = p_x x$$

$(3)$ に代入：$2p_x x = I \Rightarrow x^* = \dfrac{I}{2p_x},\quad y^* = \dfrac{I}{2p_y}$

**→ 各財に所得の1/2ずつ支出する（$u=x^{1/2}y^{1/2}$ のとき）**

</details>

---

## MRS と最適消費条件

<details>
<summary>📖 無差別曲線と予算線の接点（クリックして展開）</summary>

### 最適条件の意味

消費者の最適点では：

$$\text{無差別曲線の傾き} = \text{予算線の傾き}$$

$$MRS = \frac{p_x}{p_y} \quad\Leftrightarrow\quad \frac{MU_x}{MU_y} = \frac{p_x}{p_y}$$

### 直感

- $MRS > p_x/p_y$：$x$ の価値が値段より高い → $x$ を増やすべき
- $MRS = p_x/p_y$：最適（これ以上変えても得しない）
- $MRS < p_x/p_y$：$y$ の価値が値段より高い → $y$ を増やすべき

### 需要関数の導出パターン

効用関数 $u = x^a y^b$ のとき：

$$x^* = \frac{a}{a+b}\cdot\frac{I}{p_x},\quad y^* = \frac{b}{a+b}\cdot\frac{I}{p_y}$$

| 効用関数 | $x^*$ | $y^*$ |
|----------|-------|-------|
| $u = xy$ | $I/(2p_x)$ | $I/(2p_y)$ |
| $u = x^2y$ | $2I/(3p_x)$ | $I/(3p_y)$ |
| $u = x^{1/2}y^{1/2}$ | $I/(2p_x)$ | $I/(2p_y)$ |

</details>

---

## 消費者・生産者の最適化まとめ

<details>
<summary>📖 需要関数・供給関数の導出（クリックして展開）</summary>

### 消費者の需要関数

$$\max_x B(x) - px \Rightarrow B'(x) = p \Rightarrow \text{需要関数}$$

- $B(x)$ = 便益関数（総効用）
- $B'(x)$ = 限界便益（$MB$）
- 最適条件：$MB = p$（限界便益 = 市場価格）

### 生産者の供給関数

$$\max_x px - C(x) \Rightarrow C'(x) = p \Rightarrow \text{供給関数}$$

- $C(x)$ = 費用関数
- $C'(x)$ = 限界費用（$MC$）
- 最適条件：$MC = p$（限界費用 = 市場価格）

### 独占企業の最適化

$$\max_x p(x)\cdot x - C(x) \Rightarrow MR = MC$$

- $p(x)$ = 逆需要関数
- $MR = p + p'(x)\cdot x$（限界収入）
- 逆需要 $p = a-bx$ のとき：$MR = a-2bx$（**傾きが2倍**）

</details>

---

## 経済学でよく出るパターン集

<details>
<summary>📖 よく使う計算パターン（クリックして展開）</summary>

### 台形・三角形の面積（余剰計算）

$$\text{三角形} = \frac{1}{2}\times\text{底辺}\times\text{高さ}$$

$$\text{台形} = \frac{1}{2}\times(\text{上辺}+\text{下辺})\times\text{高さ}$$

**消費者余剰の計算例：**

需要曲線 $p=120-q$、均衡価格 $p^*=80$、均衡量 $q^*=40$

$$CS = \frac{1}{2}(120-80)\times40 = 800$$

### 積分で面積を求める

$$\int_0^{x^*} MB(x)\,dx - p^* x^* = CS \quad\text{（厳密な計算）}$$

例：$B(x) = 36x - \frac{2}{3}x^2$、$x^*=18$、$p^*=12$

$$CS = B(18) - 12\times18 = (648-216)-216 = 216$$

</details>
