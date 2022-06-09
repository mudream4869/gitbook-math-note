# Cauchy-Schwarz 不等式

### 定理

設 $$a_i, b_i \in \R^+ \ \ (i=1, ..., n)$$，則

$$
\left( \sum_{i=1}^{n} a_ib_i \right)^2 \leq \left( \sum_{i=1}^{n} a_i^2 \right)\left( \sum_{i=1}^{n} b_i^2 \right)
$$

等號成立於

* $$\sum a_i^2 = 0$$​ 或 $$\sum b_i^2 = 0$$​

或者

* $$\exist k \ s.t. \ a_i = kb_i \ \forall i$$​

### 證明

考慮

$$
\sum(a_i-b_ix)^2 = \sum b_i^2 x - 2 \sum a_ib_i + \sum a_i^2 \geq 0 \ \forall x \in \R
$$

​判別式就是不等式，並且在式子 = 0 時 $$x = \frac{a_i}{b_i} \ \forall i$$

### 習題

* $$a_i, b_i \in \R^+$$，證明下面的不等式並且找等式成立條件：

$$
\sum_{i=1}^n \frac{a_i^2}{b_i} \geq \frac{\left( \sum_{i=1}^n a_i \right )^2}{\sum_{i=1}^n b_i}
$$

* $$a, b, c \in \R^+, abc=1$$​，證明

$$
\frac{a^4}{a+b} + \frac{b^4}{b+c} + \frac{c^4}{c+a} \geq \frac{3}{2}
$$

