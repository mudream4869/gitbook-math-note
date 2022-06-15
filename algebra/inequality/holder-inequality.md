# Holder 不等式

### 定理

$$a_i, b_i > 0, p,q > 1, \frac{1}{p} + \frac{1}{q} = 1$$​，則

$$
\sum_{i=1}^na_ib_i \leq \left( \sum_{i=1}^n a^p\right)^\frac{1}{p} \left( \sum_{i=1}^n b^q\right)^\frac{1}{q}
$$

​並且等號成立在 $$a^p = \lambda b^q$$。

### 證明

不失一般性，設 $$||a||_p = ||b||_q = 1$$​。根據 [Young 不等式](young-inequality.md)：

$$
\sum a_ib_i \leq \frac{\sum a_i^p}{p} + \frac{\sum b_i^q}{q} = \frac{1}{p} + \frac{1}{q} = 1
$$

​回推等號成立的條件是：

$$
\left(\frac{a}{||a||_p}\right)^p = \left(\frac{b}{||b||_q}\right)^q
$$

得證。

### 習題

1. 證明：$$\frac{1}{\sin^4\theta} + \frac{1}{\cos^4\theta} \geq 8$$​
