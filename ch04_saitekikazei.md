# ④ 最適課税・独占

> **出題頻度：★★★** 死荷重の4倍の法則・ラーナー独占度は頻出。

---

## p21（所得税 vs 消費税の効用比較）★★★

### 問題概要
$$u = x^{\frac{1}{2}}y^{\frac{1}{2}},\quad p_x=1,\ p_y=2,\ I=60$$

### ① 課税前の最適消費

ラグランジュ法：$\frac{MU_x}{MU_y} = \frac{p_x}{p_y} \Rightarrow \frac{y}{x} \cdot \frac{1}{2} = \frac{1}{2} \Rightarrow y = x$

予算制約：$x + 2y = 60 \Rightarrow x = y = 20,\quad u_0 = 20$

### ② 所得税（税率10%）

手取り所得 $= 0.9 \times 60 = 54$

$$x = y = \frac{54}{3} = \frac{27}{1},\quad y = \frac{27}{2} \Rightarrow u = \frac{27\sqrt{2}}{2}$$

税収 $= 6$

### ③ 一般消費税（税率 $\tau_C$）

予算制約：$(1+\tau_C)x + 2(1+\tau_C)y = 60 \Rightarrow x + 2y = \frac{60}{1+\tau_C}$

$$x = \frac{30}{1+\tau_C},\quad y = \frac{15}{1+\tau_C}$$

税収 $= \frac{60\tau_C}{1+\tau_C}$

### ④ 所得税と同額（6）の消費税率

$$\frac{60\tau_C}{1+\tau_C} = 6 \Rightarrow \tau_C = \frac{1}{9} \Rightarrow x = 27,\quad y = \frac{27}{2},\quad u = \frac{27\sqrt{2}}{2}$$

> **結論**：同額の税収では所得税も消費税も効用水準が等しくなる（等価性）。

---

## p23（労働所得税と死荷重）★★★

### 問題概要
$$u'(l) = 360 - 180l \quad\text{（余暇の限界効用）},\quad w = 300$$

個人は時間 $[0,1]$ を余暇 $l$ と労働 $(1-l)$ に配分。

### ① 最適余暇（課税なし）

$$u'(l) = w \Rightarrow 360-180l = 300 \Rightarrow \boxed{l_0 = \frac{1}{3}}$$

### ② 余暇効用と労働所得

余暇効用 $=$ 限界効用曲線の台形面積：

$$\frac{1}{2}(u'(0)+u'(l_0))\times l_0 = \frac{1}{2}(360+300)\times\frac{1}{3} = 110$$

$$\text{労働所得} = 300\times\frac{2}{3} = 200$$

### ③ 税率 $t$ の課税後の余暇時間

手取り賃金 $= (1-t)w$：

$$360-180l' = (1-t)\times300 \Rightarrow l'(t) = \frac{1}{3}+\frac{5t}{3}$$

**$t=0.2$ のとき：$l' = 2/3$**

### ④ 余暇効用・労働所得（$t=0.2$）

$$\text{余暇効用} = \frac{1}{2}(360+240)\times\frac{2}{3} = 200$$

$$\text{手取り労働所得} = 240\times\frac{1}{3} = 80$$

### ⑤ 税収と死荷重

$$T = 0.2\times300\times\frac{1}{3} = 20$$

| | 余暇効用 | 労働所得 | 税収 | SS |
|--|--|--|--|--|
| 税なし | 110 | 200 | — | 310 |
| 税あり | 200 | 80 | 20 | 300 |

$$DWL = 310 - 300 = \boxed{10}$$

### ⑥ 死荷重は税率2倍で何倍？

$DWL \propto t^2$ のため：

$$\frac{DWL_{20\%}}{DWL_{10\%}} = \left(\frac{0.2}{0.1}\right)^2 = \boxed{4\text{倍}}$$

> **理由**：税率2倍 → 三角形の底辺（労働減少量）も高さ（税額）も2倍 → 面積は4倍

---

## p48（独占市場・ラーナー独占度）★★★

### 問題概要
$$\text{需要：}p = 100-2x,\quad C(x) = 20x$$

### ① 独占均衡

逆需要が $p = a-bx$ のとき $MR = a-2bx$（傾きが2倍）：

$$MR = 100-4x,\quad MC = 20$$

$$MR = MC \Rightarrow x^* = 20,\quad p^* = 60,\quad \pi = (60-20)\times20 = 800$$

### ② ラーナー独占度

$$L = \frac{p^*-MC}{p^*} = \frac{60-20}{60} = \boxed{\frac{2}{3}}$$

### ③ 価格弾力性との関係

$$\varepsilon = -\frac{p^*}{x^*}\cdot\frac{dx}{dp} = -\frac{60}{20}\times\left(-\frac{1}{2}\right) = \frac{3}{2}$$

$$\frac{1}{\varepsilon} = \frac{2}{3} = L \quad\checkmark$$

---

## p49（独占・死荷重）★★☆

### 問題概要
$$x = 60-p \Rightarrow p = 60-x,\quad C(x) = \frac{1}{2}x^2$$

### ① 独占均衡

$$MR = 60-2x,\quad MC = x$$

$$MR = MC \Rightarrow x^* = 20,\quad p^* = 40,\quad \pi = 40\times20 - \frac{1}{2}\times400 = 600$$

### ② ラーナー独占度

$$L = \frac{40-20}{40} = \boxed{\frac{1}{2}}$$

### ③ 死荷重

完全競争均衡：$p = MC \Rightarrow 60-x = x \Rightarrow x_c = 30,\quad p_c = 30$

$$DWL = \frac{1}{2}(p^*-MC|_{x^*})(x_c-x^*) = \frac{1}{2}(40-20)(30-20) = \boxed{100}$$

---

## ラーナー独占度まとめ

$$L = \frac{p-MC}{p} = \frac{1}{\varepsilon}$$

| $L$ | 意味 |
|-----|------|
| $L = 0$ | 完全競争（$p=MC$） |
| $L$ 大 | 独占力強い・$\varepsilon$ 小（需要が非弾力的） |
| $L$ 小 | 独占力弱い・$\varepsilon$ 大（需要が弾力的） |

---

## 用語解説

| 用語 | 説明 |
|------|------|
| **ラーナー独占度** | 独占力の強さを示す指標：$L=(p-MC)/p$ |
| **ラムゼイ・ルール** | 最適課税：価格弾力性が大きい財ほど低税率 |
| **死荷重** | 独占・課税による非効率性から生じる社会的損失 |
| **限界収入（MR）** | 追加1単位の販売から得られる収入増加分 |
