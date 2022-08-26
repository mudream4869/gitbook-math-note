# 替換法

### abc = 1 替換: $$a = \frac{y}{x}$$, $$b = \frac{z}{y}$$, $$c = \frac{x}{z}$$​

Example:

$$
\frac{1}{\sqrt{1 + a}} + \frac{1}{\sqrt{1 + b}} + \frac{1}{\sqrt{1 + c}} \leq \sqrt{\frac{9}{2}}
$$

​由柯西不等式：

$$
\left( \sum_{cyc}\sqrt{\frac{x}{x+y}} \right)^2 \leq \left(\sum_{cyc}{x(y+z)} \right) \left(\sum_{cyc}\frac{1}{(x+y)(y+z)} \right)
$$

所以我們只需要證明：

$$
\frac{(xy+yz+zx)(x+y+z)}{(x+y)(y+z)(z+x)} \leq \frac{9}{8}
$$

​即是：

$$
6xyz \leq \sum{x^2(y+z)}
$$
