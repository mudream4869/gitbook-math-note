# Jenson 不等式

### 定義

當函數有這樣的性質

$$
f(\lambda x + (1-\lambda)y) \leq \lambda f(x) + (1-\lambda)f(y)
$$

​那我們將之稱為凸函數 (convex function)。

### 定理：擴增 n&#x20;

f 是凸函數，那

$$
f(\lambda_1x_1 + \lambda_2x_2 + ... + \lambda_nx_n) \leq \lambda_1f(x_1) + ... + \lambda_nf(x_n)
$$

​其中 $$\lambda_i \in [1, 0] \ \forall i$$​，$$\sum_{i=1}^n\lambda_i = 1$$​， $$n \geq 2$$。

#### 證明

對 n 使用歸納法：

* $$n=2$$​: ok
* $$n > 2$$​

令 $$\lambda = \sum_{i=1}^{n-1} \lambda_i$$​

$$
f(\lambda_1x_1 + \lambda_2x_2 + ... + \lambda_nx_n) \leq
f(\lambda(\frac{\lambda_1}{\lambda}x_1 + \frac{\lambda_2}{\lambda}x_2 + ...
 + \frac{\lambda_{n-1}}{\lambda}x_{n-1}
) + \lambda_nx_n) \leq \lambda f(...) + \lambda_n f(x_n)
$$

​然後再套 Jenson n-1 的不等式就得証了。

### 定理：凸函數

$$f$$​是二次可導函數，則：

$$f$$​是凸函數 and only if $$f''(x) > 0$$

{% hint style="info" %}
TODO
{% endhint %}

### 習題

1. 用 Jenson 證明平均不等式。
2. 證明：歐幾里得空間的三角形 $$\Delta ABC$$​ 滿足：$$\sin \angle A + \sin \angle B + \sin \angle C \leq \frac{3 \sqrt{3}}{2}$$​
3. x, y, z > 0，證明：$$\frac{x}{2x + y + z} + \frac{y}{x + 2y + z} + \frac{z}{x + y + 2z} \leq \frac{3}{4}$$
4. x, y, z > 0，證明：$$\frac{x}{\sqrt{y+z}} + \frac{y}{\sqrt{z+x}} + \frac{z}{\sqrt{x+y}} \geq \sqrt{\frac{3}{2}(x+y+z)}$$​

