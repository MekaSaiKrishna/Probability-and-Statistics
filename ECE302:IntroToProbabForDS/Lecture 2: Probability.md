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

> Example: The probability of getting a head when tossing a coin:
> $$\mathbb{P}(H) = 1/2$$
> Generally, our intuition is from a frequentist point of view. That is we arrive at a limiting number of occurence by conducting many many experiments. But in cases where we can't run an experiment infinitely many many times we can form a subjective opinion which is called the "Bayesian Approach"

### 2.2.1 Sample Space
A **sample space** $\Omega$ is the collection of all possible outcomes.

We denote $\omega$ as an element in $\Omega$.

> Example:
> > Coin Flip:
> > $\Omega$ = {'H', 'T'}
>
> > Throw a dice:
> > $\Omega$ = {1,2,3,4,5,6}
>
> > Waiting time for a bus in West Lafayette:
> > $\Omega$ = { t | 0 $\leq$ t $\leq$ 30}

Elements in the space can be anything, it can be 'discrete numbers', 'continuous intervals', 'functions' etc

### 2.2.2 Event Space
An **event** $F$ is a subset in the sample space $\Omega$.

> Example: Throw a dice. Let $\Omega$ = {1, 2, 3, 4, 5, 6}
> 
> $F_{1}$ = {even numbers} = {2, 4, 6}
>
> $F_{2}$ = {less than 3} = {1, 2}

> Example: Wait for a bus. Let $\Omega$ = {0 $\leq$ t $\leq$ 30}
> 
>$F_{1}$ = {0 $\leq$ t $\lt$ 10}
>
>  $F_{2}$ = {0 $\leq$ t $\lt$ 5} $\cup$ {20 $\lt$ t $\leq$ 20}

The collection of all events is called the **Event Space**, denoted as $\mathscr{F}$

### 2.2.3 Probability Law
A **probability law** is a function $\mathbb{P}$: $\mathscr{F} \rightarrow [0, 1]$ that maps an event A to a real number in [0, 1].

> Example: Consider flipping a coin. The event space $\mathscr{F}$ = {$\emptyste$,{H},{T},$\Omega$}. Suggest a probability law that makes sense:
>
> $\mathbb{P}(\emptyset) = 0$
>
> $\mathbb{P}(\lbrace H \rbrace) = 1/3$
>
> $\mathbb{P}(\lbrace T \rbrace) = 2/3$
>
> $\mathbb{P}(\Omega) = 1$


### 2.2.4 Measure (Optional)
Probability = relative size of a set (w.r.t the sample space).

> Example:
>
> Discrete numbers - counting
>
> 1D intervals - length
>
> 2D sets - area

 Defining probability as $$\mathbb{P} = \frac{\text{Size of E}}{\text{Size of} \\ \Omega}$$

 Therefore, an isolated point in an interval has ZERO probability, because it is a point and it isn't an interval.

> Example 1: Let $\Omega$ = [0, 1]. Then the set {0.5} has measure ZERO.
>
> Example 2: Let $\Omega$ = {1,2,3,4,5,6}. Then the set {1} has a probability of 1/6.
>
> Example 3: For any intervals $\mathbb{P}[[a,b]] = \mathbb{P}[(a,b)]$ because the two end points have measure zero: $\mathbb{P}[\lbrace a \rbrace] = \mathbb{P}[\lbrace b \rbrace] = 0$ 

 An event $A \in \mathbb{R}$ is said to hold **almost surely (a.s.)** if $$\mathbb{P}[A] = 1$$.
 except for all measure-zero sets in $\mathbb{R}$


### 2.2.5 Probability Space


___
## 2.3 Axioms of Probability

___
## 2.4 Conditional Probability

___
## 2.5 Independene

___
## 2.6 Bayes Theorem

                     
