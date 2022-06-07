# 平均不等式

### 定義與定理

$$a_i > 0 \ \forall \ i$$

* 算數平均數

$$
A_n = \frac{a_1 + a_2 + ... + a_n}{n}
$$

* 幾何平均數

$$
G_n = \sqrt[n]{a_1a_2...a_n}
$$

* 調和平均數

$$
H_n = \frac{n}{\frac{1}{a_1} + \frac{1}{a_2} + ... + \frac{1}{a_n}}
$$

則：

$$
H_n \leq G_n \leq A_n
$$

且等號成立 if and only if $$a_1 = a_2  = ... = a_n$$

事實上，幾何平均數和調和平均數的比較可以直接由算幾不等式推得，所以我們只需要證明算幾的部分就好。

### 遞推證明

#### n = 2 成立

顯然：$$\frac{x + y}{2} - \sqrt{xy} = \frac{(\sqrt x + \sqrt y)^2}{2} \geq 0$$

#### n 成立 -> 2n 成立

$$
\frac{\frac{a_1 + ... + a_n}{n} + \frac{a_{n+1} + ... + a_{2n}}{n}}{2} \geq \sqrt{\frac{a1 + ... a_n}{n}\frac{a_{n+1} + ... + a_{2n}}{n}} \geq \sqrt{\sqrt[n]{a_1...a_n}\sqrt[n]{a_{n+1}...a_{2n}}} = \sqrt[2n]{a_1...a_{2n}}
$$

#### n 成立 -> n-1 成立

令 $$s = a_1 + ... + a_{n-1}$$​

$$
\frac{s}{n-1} = \frac{a_1 + ... a_{n-1} + \frac{a_1 + ... a_{n-1}}{n-1}}{n} \geq \sqrt[n]{a_1...a_{n-1}(\frac{s}{n-1})}
$$

​移項後即得證。

### 由Jensen不等式證明

兩邊取 $$\ln$$ 可以由 $$\ln$$​的凸向上性直接得到

$$
\ln(\frac{a_1 + ... + a_n}{n}) \geq \frac{\ln a_1 + ... + \ln a_n}{n}
$$

​

### 習題

1. $$a, b > 0, ab^2 = 1$$，求 $$a + 4b$$ 的最小值？
2. $$a, b, c$$為三角形三邊長，證明：$$abc \geq (a+b-c)(b+c-a)(c+a-b)$$​
