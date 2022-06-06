# 模和同餘

當 a 除 n 的餘數 和 b 除 n 餘數相同，我們記做

$$
a \equiv b \ (mod \ n)
$$

​於是，可以有這些性質：

* $$a \equiv b \ (mod \ n) \Rightarrow a-c \equiv b-c\ (mod \ n)$$
* $$a \equiv b \ (mod \ n) \Rightarrow ac \equiv bc\ (mod \ n)$$
* $$a \equiv b \ (mod \ n) \Rightarrow n|a-b$$

也就是說，在模 n 底下，我們可以拿到一個環。

對於和 $$n$$ 互質的元素 $$m$$ ，存在反元素，通常可以記做 $$m^{-1}$$&#x20;

$$
(n, m) = 1 \Rightarrow \exist m^{-1} \ s.t. \ mm^{-1} \equiv 1 (mod \ n )
$$

​這並不是那麼的顯然，不過可以考慮輾轉相除法所能證明的

$$
(m, n)=1 \Rightarrow  \exist x,y \in \mathbb{N} \ s.t. \  mx+ny=1
$$

​直接使用就可以拿 $$x$$​ 做為 ​$$m$$​ 的反元素。

### 習題

1. 給定一個位數為 N 的大數，請設計出一個 7 個狀態的自動機使得輸入這個大數字串，最後走到的狀態可以代表這個大數除7的餘數。
2. $$2^{100}$$除7的餘數
3. 給定質數 $$p$$，證明在模 $$p$$ 底下存在一種 $$0, 1, 2, ..., p-1$$ 的排列方式 $$a_1, a_2, ..., a_n$$​，使\
   $$a_1, a_1a_2, a_1a_2a_3, ... a_1a_2...a_p$$​ 也是一種 $$0, 1, 2, ..., p-1$$ 的排列。
4. 用 (3) 來證明 Wilson 定理。
