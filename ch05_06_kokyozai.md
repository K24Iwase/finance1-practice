# ⑤⑥ 公共財・リンダール均衡

> **出題頻度：★★★** サムエルソン条件とリンダール均衡は最重要。

---

## 基本概念

### 公共財の特性
- **非排除性**：対価を払わない人を排除できない
- **非競合性**：1人が消費しても他者の消費量は減らない

### 私的財 vs 公共財：需要の足し方

| | 私的財 | 公共財 |
|--|--|--|
| 消費 | 各自が異なる量を購入 | 全員が同じ量を消費 |
| 足し方 | **横（量を合計）** | **縦（WTPを合計）** |
| 最適条件 | $MB_i = p = MC$ | $\sum MB_i = MC$（サムエルソン条件） |

---

<a name="kokyozai-p28"></a>

## p28（私的財 vs 公共財）★★★

### 問題概要
$$MB_i = 70-x \quad(\text{3人とも同じ}),\quad MC = 2x$$

### ① 私的財：社会的需要曲線（横に足す）

$$x_i = 70-p \Rightarrow X = 3x_i = 3(70-p) \Rightarrow \boxed{p = 70-\frac{1}{3}X}$$

### ② 私的財の競争均衡

$$70-\frac{1}{3}x = 2x \Rightarrow x^* = 30,\quad p^* = 60$$

$$CS = \frac{1}{2}(70-60)\times30 = 150,\quad PS = 60\times30 - \int_0^{30}2x\,dx = 900$$

$$SS = 1050$$

### ③ 公共財：社会的限界便益（縦に足す）

同じ量 $x$ を3人が同時に消費 → 各人の$MB$を縦に合計：

$$SMB = 3\times(70-x) = \boxed{210-3x}$$

### ④ 公共財の最適供給量・社会的純便益

**サムエルソン条件**：$SMB = MC$

$$210-3x = 2x \Rightarrow x^* = 42$$

$$\text{純便益} = \int_0^{42}(210-5x)\,dx = \left[210x-\frac{5}{2}x^2\right]_0^{42} = 8820-4410 = \boxed{4410}$$

---

## サムエルソン・ルール（重要！）

$$\sum_{i=1}^n MV_i = MC \quad\Leftrightarrow\quad \sum_{i=1}^n MRS_i = MRT$$

> **直感**：公共財1単位を増やすと全員が便益を得る。  
> 全員の「払ってよい金額の合計」が費用を上回る間は供給を増やすべき。

---

<a name="lindahl-p15"></a>

## p15（リンダール均衡・線形）★★★

### 問題概要
$$MV^a = 80-x,\quad MV^b = 140-2x,\quad MC = 60$$

### リンダール・メカニズムの仕組み
1. 政府が各人に負担率（個人価格）を提示
2. 各人がその価格で希望量を申告
3. 希望量が一致するまで負担率を調整

### ① 5割ずつの場合

各人の負担単価 $= 0.5\times60 = 30$

$$\text{a：}80-x = 30 \Rightarrow x_a = 50,\quad \text{b：}140-2x = 30 \Rightarrow x_b = 55$$

### ② 負担率を上げるべきは？

$x_b > x_a$ → bがより多く希望 → **bの負担率を上げる**

### ③ リンダール均衡

a の負担率 $\alpha$、b の負担率 $1-\alpha$：

$$x_a = 80-60\alpha,\quad x_b = 40+30\alpha$$

$$x_a = x_b \Rightarrow 80-60\alpha = 40+30\alpha \Rightarrow \alpha_a = \frac{4}{9},\quad \alpha_b = \frac{5}{9}$$

$$x^* = \frac{160}{3},\quad p_a = \frac{80}{3},\quad p_b = \frac{100}{3}$$

### ④ 社会最適であることの証明

リンダール均衡では定義より $MV^a = p_a$、$MV^b = p_b$、$p_a + p_b = MC$。

$$\therefore MV^a + MV^b = MC \quad\text{（サムエルソン条件）}\quad\checkmark$$

---

<a name="lindahl-p16"></a>

## p16（生産可能曲線・パレート最適）★★☆

### 問題概要
- 初期資源 $I=150$、消費財 $X$：1単位=資源1、公共財 $Y$：1単位=資源5
- $u^i = x^i Y$

### ① 生産可能曲線
$$\boxed{X + 5Y = 150}$$

### ② パレート最適

$MRS^i = x^i/Y$（$u^i = x^i Y$ より $MU_Y/MU_x = x^i/Y$）

サムエルソン条件 $\Sigma MRS = MRT = 5$：

$$\frac{x^A+x^B}{Y} = 5 \Rightarrow X = 5Y$$

生産可能曲線に代入：$5Y+5Y=150 \Rightarrow \boxed{Y^* = 15}$

---

<a name="lindahl-p18"></a>

## p18（リンダール均衡・非線形費用）★★☆

### 問題概要
$$u^i = x^i y,\quad \omega_A = 48,\quad \omega_B = 27,\quad c(y) = y^2$$

### ① $\theta$ の負担率での需要量

**個人A**の最適化（$x^A = 48-\theta y^2$ を代入）：

$$\max(48-\theta y^2)y \Rightarrow 48-3\theta y^2 = 0 \Rightarrow \boxed{y_A = \frac{4}{\sqrt{\theta}}}$$

**個人B**（$x^B = 27-(1-\theta)y^2$）：

$$\boxed{y_B = \frac{3}{\sqrt{1-\theta}}}$$

### ② リンダール均衡（$y_A = y_B$）

$$\frac{4}{\sqrt{\theta}} = \frac{3}{\sqrt{1-\theta}} \Rightarrow 16(1-\theta) = 9\theta \Rightarrow \boxed{\theta^* = \frac{16}{25}}$$

$$y^* = 5,\quad x_A = 32,\quad x_B = 18$$

### ③ パレート最適の証明

$MC = c'(y) = 2y = 10$（$y=5$ 代入）

$$MRS^A + MRS^B = \frac{32}{5} + \frac{18}{5} = 10 = MC \quad\checkmark$$

---

## 用語解説

| 用語 | 説明 |
|------|------|
| **フリーライダー** | 公共財の費用を負担せずに便益だけ享受する者 |
| **リンダール均衡** | 各人が自分の限界評価に等しい個人価格を支払う均衡 |
| **サムエルソン条件** | 公共財の最適供給条件：$\Sigma MRS = MRT$ |
| **非競合性** | ある人の消費が他者の消費量を減らさない性質 |
| **非排除性** | 対価を払わない人を消費から排除できない性質 |
