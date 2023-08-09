# Lecture 1: Introduction

## 1.1 Infinite Series
### 1.1.1 Geometric Series
$$\sum_{k=0}^{n} r^{k} = 1 + r + r^2 + ... + r^n = \frac{1-r^{n+1}}{1-r}$$

Let 0 < r < 1, then the sum of an infinite geometric series is:
$$\sum_{k=0}^{\infty} r^{k} = \lim_{n\to\infty} \frac{1-r^{n+1}}{1-r} = \frac{1}{1-r}$$

* Other variations can arise if you either differentiate the above or integrate and play around with such combination of operations
  
### 1.1.2 Binomial Series
$$(a + b)^n = \sum_{k=0}^{n} {}^{n}C_{k} a^k b^{n-k}$$

Let 0 < p < 1, then it is obvious that $$\sum_{k=0}^{n} {}^{n}C_{k} p^k (1-p)^{n-k} = 1$$


## 1.2 Approximations
### 1.2.1 Taylor Approximations
An engineering tool!

Let $f: \mathbb{R} \rightarrow \mathbb{R}$ be a **continuous function** with **infinite** derivatives. Let $a \in \mathbb{R}$  be a fixed constant. The Taylor approximation of $f$ at x=a is 
$$f(x) = f(a) + f'(a)(x-a) + \frac{f''(a)}{2!}(x-a)^2 + ...$$
$$f(x)=\sum_{n=0}^{\infty}\frac{f^{(n)}(a)}{n!}(x-a)^n$$

* Example: Taylor approximation of f(x) = sin(x) **at x=0** is $\rightarrow$ f(x) $\simeq x - \frac{x^3}{3!} + \frac{x^5}{5!} + ...$ 
  
### 1.2.2 Exponential Series
Let x be **any real number**. Then,
$$e^x = 1+ x + \frac{x^2}{2!} + \frac{x^3}{3!} + ...= \sum_{k=0}^{\infty} \frac{x^k}{k!}$$
  
### 1.2.3 Logarithmic Approximation
Let 0 < x < 1 be a constant. Then,
$$log(1+x) = x - x^2 + O(x^3)$$ (Obtained from Taylor approximation at x=0)

This result will be used in "**_Central Limit Theorem_**"

# 1.3 Integration
* 1.3.1 Odd and Even functions
  
**Even Function:**
$$f(-x) = f(x)$$

**Odd Function:**
$$f(-x) = -f(x)$$
  
* 1.3.2 Fundamental Theorem of Calculus
Let $f:[a,b] \rightarrow \mathbb{R}$ be a continuous function defined on a closed interval [a,b]. Then, $$f(x) = \frac{d}{dx}\int_{a}^{x} f(t) dt$$

**Corollary:** Let $f:[a,b] \rightarrow \mathbb{R}$ be a continuous function defined on a closed interval [a,b]. Let $g: \mathbb{R} \rightarrow [a,b]$ be a continuously differentiable function. Then,
$$\frac{d}{dx}\int_{a}^{g(x)}f(t) dt = g'(x).f(g(x))$$ For anyd $x \in [a,b]$

>**Example**: Evaluate the integral  $$\frac{d}{dx} \int_{0}^{x-\mu} \frac{1}{\sqrt{2 \pi \sigma^2}} exp \bigg[-\frac{t^2}{2\sigma^2} \bigg]$$
This result will be useful when discussing Gaussian random variable:
>
>**Answer**: $\frac{1}{\sqrt{2 \pi \sigma^2}} e^{-\frac{(x-\mu)^2}{2\sigma^2}}$


# 1.4 Linear Algebra 
* 1.4.1 Inner Products
  
*Definition*: Let $\mathbf{x} = [x_{1},x_{2},x_{3},...,x_{N}]^T$ and $\mathbf{y} = [y_{1},y_{2},y_{3},...,y_{N}]^T$ be two vectors. The **inner product ($\mathbf{x^T y}$)** is 
$$\mathbf{x^T y} = x_{1}y_{1} + x_{2}y_{2} + x_{3}y_{3} + ... + x_{N}y_{N}$$

> Note: Important concept when we are trying to "*classify*"

# 1.5 Combinatorics
There are 50 students in a classroom. What is the probability that there is at least one pair of students having the same birthday?





































