# AP Calculus Notes

### Unit 1

#### 1.1 Calculus Principles

| Without Calculus | With Calculus |
| ---------------- | ------------- |
| Approximate area using rectangles | Exact area under curve |
| Average rate of change | Instantaneous rate of change |
| Length of line segments | Length of arcs |
| Finite sums | Infinite sums |
| Volume of geometric solids | Volume of arbitrary solids | 

#### 1.2-1.3 Limits

-   **Limit** - value that a function approaches: $\displaystyle \lim_{x \to c} f(x)$ 
-   To solve:
    1.  Plug in directly. If undefined, continue
    2.  Factor, simplify, rationalize
    3.  Find limit on graph
    4.  Analyze limit
    5.  L'Hôpital's rule

#### 1.4 Continuity and One-Sided Limits

-   One-sided limits approach a value from only one side, positive or negative: $\displaystyle \lim_{x \to c^+} f(x)$ or $\displaystyle \lim_{x \to c^-} f(x)$
-   **Continuity** - at a point $x = c$: $\displaystyle \lim_{x \to c^+} f(x)= \lim_{x \to c^-} f(x) = f(c)$ 
-   **Intermediate Value Theorem** - for a function $f$ continuous over $[a, b]$, $f(c) = k$ where $k \in [f(a),f(b)] $ such that $c \in [a, b]$
    -   Function $f$ must pass through all $y$-values between $f(a)$ and $f(b)$ between $a$ and $b$
-   **Extreme Value Theorem** - a function $f$ continuous over $[a, b]$ has absolute minimum and absolute maximum over $[a, b]$

#### 1.5 Infinite Limits

-   **Vertical Asymptote** - function $f$ has vertical asymptote at $c$ if $\displaystyle \lim_{x \to c^\pm} f(x) = \pm\infty$
    -   function typically undefined at $c$ $\to$ look for division by 0 etc. 
-   **Horizontal Asymptote** - function $f$ has horizontal asymptote of $k$ if $\displaystyle \lim_{x \to \pm\infty} f(x) = k$
    -   function typically has decreasing rate of change towards infinity $\to$ $\displaystyle \frac{1}{x}, e^x, $ etc.
    -   function has division of similarly growing functions that "cancel" $\to$ $\displaystyle \frac{x + 2}{4x - 3}$

