# Lecture 3: Set Theory

>**Definition**: Probability is the measure of the size of a subset in a sample space

## 2.1 Set Theory
### 2.1.1 Set
> Definition: A **set** is a collection of objects. We denote $A = [\xi_1,\xi_2,\xi_3,...,\xi_n\] as a set, and $\xi_{i}$ is the i-th element in the set.$

**Notation:**
 * $\xi \in A:$ An object $\xi$ is in set A
 * $\xi \not\in A:$ An object $\xi$ is not in set A

**Finite, Countable, Uncountable**
 *  Finite: $A = [0, 1]$
 *  Countable: $A =[2,4,6,8,...] $
 *  Uncountable: $A = [x |  0 < x < 1]$

**Open and Closed Intervals**
 * (a,b) = {$x$ | a $< x <$ b}
 * [a,b] = {$x$ | a $\leq x  \leq$ b}

> A set can contain functions !
>
> Examples: (a) Set of Straight line - f(x) = ax + b; 'a' and 'b' are the sources of randomness

### 2.1.2 Subset
A **subset** of A is sub-collection of objects in A. That is, $B \subset A$ if for any $\xi \in B$, this $\xi$ is also in A.

**Proper Subset**: $B \subset A$

> Example: If A = {1,2,3,4,5,6}, then B={1,2} is a *proper subset* of A.
> 
> Example: If A = {1,2,3}, then B={1,2,3} is an *improper subset* of A.

> Theorem: If $A \subseteq B$ and $B \subseteq A$, then $A=B$

### 2.1.3 Empty set and Universal set
**Empty Set**: A set is empty if it contains no element. We denote an empty set as $\emptyset$

**Universal Set**: The universal set is the set containing all elements. We denote an universal set as $\Omega$.
Therefore, any set is a subset of $\Omega$, including $\Omega$ itself.

### 2.1.4 Union
The **finite union** of two sets A and B contains all elements in A _or_ in B. That is,
$$A \cup B = \lbrace \xi \\ | \\ \xi \in \\ A \\ or \\ \xi \in B \rbrace$$

The **infinite union** of $A_{1}$, $A_{2}$,..., $A_{n}$ is denoted as 
$$A \overset{\mathrm{def}}{=} \bigcup\limits_{i=1}^{\infty} A_i$$
It holds that $x \in A$ is in **at least one** of $A_1$, $A_2$,..., $A_{n}$ 

### 2.1.5 Intersection
The **finite intersection** of two sets A and B contains all elements in A _and_ in B. That is,
$$A \cap B = \lbrace \xi \\ | \\ \xi \in \\ A \\ and \\ \xi \in B \rbrace$$

> Example: If A={1,2,3,4}, B={1,5,6}, then $A \cap B$ = {1}
>
> Example: If A = { t | 3 $\lt$ t $\leq$ 4}, B = { t | t $\geq$ 3.5}, then $A \cap B$ = [3.5, 4]

The **infinite intersection** of $A_{1}$, $A_{2}$,..., $A_{n}$ is denoted as 
$$A \overset{\mathrm{def}}{=} \bigcap\limits_{i=1}^{\infty} A_i$$
It holds that $x \in A$ is in **all** of $A_1$, $A_2$,..., $A_{n}$ 

### 2.1.6 Complement difference
The **complement** of a set A is the set containing all elements in $\Omega$ but not in A. That is
$$A^{c} = \lbrace \xi \\ | \\ \xi \\ \in \\ \Omega \\ and \\ \xi \\ \notin \\ A \rbrace$$

The **difference** A\B is the set containing all elements in A but not in B.
$$A\B = \lbrace \xi \\ | \\ \xi \in A \\ and \\ \xi \notin B \rbrace$$

> $A\B = A \cap B^{c}$


### 2.1.7 Disjoint and partition
Two sets A and B are **disjoint** if $A \cap B = \emptyset$. For a collection of sets { $A_{1}$, $A_{2}$, ..., $A_{n}$ }, we say that the collection is disjoint if $A_{i} \cap A_{j} = \emptyset$

A collection of sets { $A_{1}$, $A_{2}$, ..., $A_{n}$ } is a **partition** to the universal set $\Omega$ if it satisfies the following conditions:
1) (non-overlap) { $A_{1}$, $A_{2}$, ..., $A_{n}$ } is disjoint
2) (decompose) $A_{1} \cup A_{1} \cup ... A_{n} = \Omega$

### 2.1.8 Set Operations
There are four set operations:

* **Commutative** (Order doesn't matter)
  > $A \cap B = B \cap A$
  >
  > $A \cup B = B \cup A$
* **Associative** (How to do multiple union and intersection)
  > $A \cup (B \cup C) = (A \cup B) \cup C$
  >
  > $A \cap (B \cap C) = (A \cap B) \cap C$
* **Distributive** (How to mix union and intersection)
  > $A \cap (B \cup C) = (A \cap B) \cup (B \cap C)$
  > 
  > $A \cup (B \cap C) = (A \cup B) \cap (B \cup C)$
* **De Morgan's Law** (How to complement over intersection and union)
  > $(A \cap B)^{c} = A^{c} \cup B^{c}$
  >
  > $(A \cup B)^{c} = A^{c} \cap B^{c}$
___
## 2.2  Probability space

___
## 2.3 Axioms of Probability

___
## 2.4 Conditional Probability

___
## 2.5 Independene

___
## 2.6 Bayes Theorem

                     
