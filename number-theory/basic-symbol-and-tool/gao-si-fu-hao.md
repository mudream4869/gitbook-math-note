---
description: 又稱取整函數
---

# 高斯符號

定義如下

* $$n \leq x < n+1 \Rightarrow \lfloor x \rfloor = n$$​
* $$n < x \leq n+1 \Rightarrow \lceil x \rceil = n +1$$
* $$\{x\} = x - \lfloor x \rfloor$$​

### 埃爾米特恆等式

$$
\lfloor mx \rfloor = \sum_{i=0}^{m-1} \left \lfloor x + \frac{i}{m} \right \rfloor
$$

​這裡就不多做證明

{% hint style="info" %}
HINT: 可以只考慮 $$x \in [0, 1)$$ 的情況。
{% endhint %}

&#x20;​由埃爾米特恆等式，可以再推得以下恆等式

$$
\sum_{k=0}^{m-1}\left\lfloor \frac{km}{n} \right \rfloor = \sum_{k=0}^{m-1} \sum_{i=0}^{m-1}\left\lfloor \frac{k}{n} + \frac{i}{m} \right \rfloor = \sum_{i=0}^{m-1}\left\lfloor \frac{in}{m} \right \rfloor
$$

也就是說，在這式子裡面 $$n$$ 和 $$m$$ 可以相互交換，而這和二次互反律也有關聯。

### n!因數分解

&#x20;$$n!$$ 裡面的 $$p$$ (質數) 的次方是多少？可以觀察 $$n$$ 底下，有多少個 $$p$$ 的倍數、$$p^2$$的倍數...：

$$
\sum_{i=1}(i - (i-1))\left \lfloor\frac{n}{p^i} \right \rfloor = \sum_{i=1}\left \lfloor\frac{n}{p^i} \right \rfloor
$$

之所以先乘 $$i$$ 是因為 $$p^i$$ 貢獻 $$i$$ 個 $$p$$，而扣掉 $$i-1$$，是因為和前面 $$p ... p^{i-1}$$ 重複計算。

