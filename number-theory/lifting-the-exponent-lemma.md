---
description: 簡稱 LTE
---

# Lifting The Exponent Lemma

本來是為了 [Zsigmondy's Theorem](zsigmondys-theorem.md) 做準備，但忽然想起這其實挺好用的，所以特別分出來。

定義：當 $$n = p_1^{n_1} p_2^{n_2} ...$$，$$v_{p_i}(n) = n_i$$​ ，即 $$v_p(n)$$是取得 $$p$$ 在 $$n$$ 裡面質因數方解的次方數。

### 描述

$$p$$是質數，$$p \nmid ab$$，$$p \mid a - b$$

For $$p = 2$$ 且 $$2 \mid n$$：

$$
v_p(a^n - b^n) = v_p(a - b) + v_p(a + b) + v_p(\frac{n}{2})
$$

​ 其餘 case：

$$
v_p(a^n - b^n) = v_p(a－b) + v_p(n)
$$

### ​證明

其實我們可以只需要證明**其餘 Case** 即可，因為假如我們證明了**其餘Case**，就可以處理特例：

先設 $$v_2(n) = k$$，所以**根據其餘 Case**：

$$
v_2(a^n - b^n) = v_2(a^{2^k} - b^{2^k})
$$

然後因式分解可以得到

$$
v_2(a^{2^k} - b^{2^k}) = v_2(a-b) + v_2(a+b) + \sum_{i = 1}^{t-1}v_2(a^{2^i} - b^{2^i})
$$

​考慮到奇數的平方和只會是 $$4k + 2$$​，也就是只會有一個 2。所以後面sum就變成 $$t-1$$ ，完成特例的推導。

接下來我們先證明一個特化的版本 $$v_p(n) = 0$$：

當 $$p \nmid abn, p\mid a-b$$，有

$$
v_p(a^n - b^n) = a_p(a-b)
$$

​也就是說，我們要證明 $$p \nmid \sum_{i = 1}^{n-1} a^{p-i}b^i$$，而在模 p 底下，我們有：

$$
\sum_{i = 1}^{n-1} a^{p-1-i}b^i \equiv \sum_{i = 1}^{n-1} a^{p-1} \equiv na^{p-1} \not\equiv 0
$$

然後為了推到題設，我們需要幾個讀者自己證明的 **Lemma**:

#### Lemma 1

當 $$p > 2, p \nmid k$$，有：

$$
v_p((1+kp)^p - 1) = 2
$$

#### ​Lemma 2

當 $$p > 2, p \nmid ab, p\mid a-b$$，有：

$$
v_p(a^p - b^p) = v_p(a-b) + 1
$$

{% hint style="info" %}
HINT: 因式分解+ Lemma 1
{% endhint %}

有了 Lemma 2 ，就可以輕易的把次方下放。

### 習題

* $$a, b$$​為正整數，解$$|2^a - 3^b| = 1$$​
