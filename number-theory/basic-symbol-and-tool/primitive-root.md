# 原根

### 定義

$$\gcd(a, m) = 1$$，則存在**最小的正整數** $$d$$ 使的

$$
a^d \equiv 1 \ (mod \ m)
$$

​此時，我們稱 $$d$$ 為 $$a$$ 在模 $$m$$ 底下的指數，並且記為  $$\delta_m(a)$$。

當 $$\delta_m(a) = \phi(m)$$，稱 a 為原根。​

### 性質

1. $$a^d \equiv 1 \Rightarrow \delta_m(a) \mid d$$
2. 由 (1) 可以知 $$\delta_m(a) \mid \phi(m)$$​
3. $$\delta_m(a) = \delta_m(a^{-1})$$
4. $$\delta_m(a^k) = \frac{\delta_m(a)}{(\delta_m(a), k)}$$​
5. $$\delta_m(ab) = \delta_m(a)\delta_m(b) \Leftrightarrow (\delta_m(a),\delta_m(b)) = 1$$​

