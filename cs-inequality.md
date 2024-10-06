@import "style.css";

# CS Inequality Overview

## The Cauchy–Schwarz inequality (also called Cauchy–Bunyakovsky–Schwarz inequality)

### Statement:
Let $a_1,a_2,\cdots,a_n,b_1,b_2,\cdots,b_n \in \mathbb{C}$ then we have the following:

$$\left|\sum_{i=1}^n a_i\overline b_i\right|^2\leq \left(\sum_{i=1}^n|a_i|^2 \right)\left(\sum_{i=1}^n|b_i|^2\right)$$
and equality holds iff $a_i=tb_i$ for some $t\in \mathbb{C}$ $\forall i\in \{1,2,3,\cdots n \}$

### Proof:
Consider the function $f:\mathbb{C} \rightarrow \mathbb{R}$ defined by

$$
\begin{equation}
    f(t)=\sum_{i=1}^n |a_i-tb_i|^2 \quad (Remember)
\end{equation}
$$

**Note:**
$$
\begin{equation}
|z|^2=z\overline z 
\end{equation}
$$

Using (2) in (1) we get,

$$
\begin{align*}
    f(t)=\sum_{i=1}^n (a_i-tb_i)(\overline{a_i-tb_i}) \\
    =\sum_{i=1}^n (a_i-tb_i)(\overline{a_i}-\overline{t}\overline{b_i})\\
    =\sum_{i=1}^n \left(|a_i|^2-(a_i\overline{b_i} \overline{t}+\overline{a_i}b_it)+|b_i||t|^2\right)
\end{align*}
$$

Now, putting $t=x+iy$ in the above we get the following:
$$
\begin{align*}
    f(x+iy)=\left(\sum_{i=1}^n |a_i|^2\right)-\left(\sum_{i=1}^n(a_i\overline{b_i} (\overline{x+iy})+\overline{a_i}b_i(x+iy))\right)+\\ \left(\sum_{i=1}^n|b_i|\right)|t|^2\\
    =A-2x\Re(B)-i2y\Im(B)+C(x^2+y^2) \quad(\text{where }A=\left(\sum_{i=1}^n |a_i|^2\right)\\
    B= \sum_{i=1}^n a_i\overline b_i \text{ \& } C=\left(\sum_{i=1}^n|b_i|\right))
\end{align*}
$$

Now, completing the squares and organising terms we get,
$$
\begin{align}
    C\left(\left(x-\frac{\Re(B)}{C}\right)^2 + \left(y-\frac{\Im(B)}{C}\right)^2 \right)+A-\frac{|B|^2}{C}=f(t)
\end{align}
$$

From equation (1) we get $f(t)\geq 0$ $\forall t \in \mathbb{C}$ and hence from equation (3) we get that for $t=\frac{\Re(B)}{C}+i\frac{\Im(B)}{C}$ also $f(t)\geq 0$. That is $A-\frac{|B|^2}{C}\geq 0 \Rightarrow |B|^2\leq AC$.

---
Download the pdf of the above article [here](cs-inequality.pdf)