# AP Calculus Notes

## Unit 1 Limits

### 1.1 Calculus Principles

| Without Calculus | With Calculus |
| --- | --- |
| Approximate area using rectangles | Exact area under curve |
| Average rate of change | Instantaneous rate of change |
| Length of line segments | Length of arcs |
| Finite sums | Infinite sums |
| Volume of regular solids | Volume of arbitrary solids | 

### 1.2-1.3 Limits

-   **Limit** - value that a function approaches: $\displaystyle \lim_{x \to c} f(x)$ 
-   To solve:
    1.  Plug in directly. If undefined, continue
    2.  Factor, simplify, rationalize
    3.  Find limit on graph
    4.  Analyze limit
    5.  L'Hôpital's rule

### 1.4 Continuity and One-Sided Limits

**One-sided limits** approach a value from only one side, positive or negative: $\displaystyle \lim_{x \to c^+} f(x)$ or $\displaystyle \lim_{x \to c^-} f(x)$ 

**Continuity** - at a point $x = c$: $\displaystyle \lim_{x \to c^+} f(x)= \lim_{x \to c^-} f(x) = f(c)$ 

**Intermediate Value Theorem** - for a function $f$ continuous over $[a, b]$, $\exists$ $f(c) \in[f(a),f(b)]$ such that $c \in [a, b]$
-   Function $f$ must pass through all $y$-values between $f(a)$ and $f(b)$ between $a$ and $b$

**Extreme Value Theorem** - a function $f$ continuous over $[a, b]$ has absolute minimum and absolute maximum over $[a, b]$

### 1.5 Infinite Limits

-   **Vertical Asymptote** - function $f$ has vertical asymptote at $c$ if $\displaystyle \lim_{x \to c^\pm} f(x) = \pm\infty$
    -   function typically undefined at $c$ $\to$ look for division by 0 etc. 
-   **Horizontal Asymptote** - function $f$ has horizontal asymptote of $k$ if $\displaystyle \lim_{x \to \pm\infty} f(x) = k$
    -   function typically has decreasing rate of change towards infinity $\to$ $\displaystyle \frac{1}{x}, e^x, $ etc.
    -   function has division of similarly growing functions that "cancel" $\to$ $\displaystyle \frac{x + 2}{4x - 3}$

## Unit 2 Derivative 

### 2.1 Derivative Definition

Slope of secant line of function $\to$ $\displaystyle \frac{\Delta f(x)}{\Delta x}$ $\to$ $\displaystyle \frac{f(x + \Delta x) - f(x)}{\Delta x}$  

Slope of tangent line of function $\to$ $\displaystyle \lim_{h \to 0} \frac{f(x + h) - f(x)}{h}$ $\to$ **Derivative Definition**

**Derivative Notation**:
$$
\frac{\Delta f(x)}{\Delta x} \xrightarrow{\lim {\Delta x \to 0}} \frac{df(x)}{dx} \xrightarrow{\text{Notation}} \frac{d}{dx} f(x)
$$
<center>or</center>

$$ \frac{d}{dx} f(x) \to f'(x)$$

Derivative represents rate of change $\to$ derivative of position $=$ velocity, derivative of velocity $=$ acceleration
$$
\begin{align*}
x(&t)\\
x'(&t) = v(t)\\
x''(&t) = v'(t) = a(t)\\
\end{align*}
$$

### 2.2-2.4 Derivative Rules

**Power Rule**: 
$$
\frac{d}{dx} x^n = nx^{n-1}
$$

**Trigonometric Functions**:
$$ 
\begin{align*}
\frac{d}{dx} \sin(x) &= \cos(x) & 
\frac{d}{dx} \cos(x) &= -\sin(x)\\ 
\frac{d}{dx} \tan(x) &= \sec^2(x) & 
\frac{d}{dx} \cot(x) &= -\csc^2(x) \\
\frac{d}{dx} \sec(x) &= \sec(x)\tan(x) & 
\frac{d}{dx} \csc(x) &= -\csc(x)\cot(x) \\
\end{align*}
$$

**Chain Rule**:
$$ 
\frac{d}{dx} f\big(g(x)\big) = f'\big(g(x)\big) \cdot g'(x)
$$

**Product Rule**:
$$ 
\frac{d}{dx} \Big(f(x) \cdot g(x)\Big) = f'(x) \cdot g(x) + f(x) \cdot g'(x)
$$

**Quotient Rule**:
$$
\frac{d}{dx} \bigg(\frac{f(x)}{g(x)}\bigg) = \frac{f'(x) \cdot g(x) - f(x) \cdot g'(x)}{\big(g(x)\big)^2}
$$

**Logarithm**:
$$
\log_b x = \frac{\ln x}{\ln b} \to \frac{d}{dx} \ln x = \frac{1}{x}
$$

**Exponential**:
$$
\frac{d}{dx} \big(b^x\big) =  b^x \cdot \ln b
$$

### 2.5 Implicit Differentiation

$$
\begin{align*}
\frac{d}{dx} \big(x\big) &= 1 \cdot \frac{dx}{dx} = 1 \\
\frac{d}{dx} \big(y\big) &= 1 \cdot \frac{dy}{dx} \\
\end{align*}
$$

<center>Example:</center> 

$$
\begin{align*}
&\frac{d}{dx} \Big(y^2 + 1 = 4x^3 \Big) \\
2y &\frac{dy}{dx} = 12x^2 \\
&\frac{dy}{dx} = \frac{6x^2}{y} \\
&\frac{dy}{dx}\bigg|_{(2, 5)} = \frac{6(2)^2}{5} 
\end{align*}
$$

### 2.6 Related Rates

Application of implicit differentiation

$$
A = \pi r^2 \\
C = 2 \pi r 
$$
$$\text{Given } \frac{dC}{dt} = 2 \text{ find } \frac{dA}{dt}$$
$$\frac{dC}{dt} = 2 \pi \frac{dr}{dt}$$
$$\frac{dr}{dt} = \frac{1}{2 \pi} \frac{dC}{dt}$$
$$\frac{dA}{dt} = 2 \pi r \frac{dr}{dt}$$
$$\frac{dA}{dt} = 2 \pi r \frac{1}{2 \pi} \frac{dC}{dt}$$
$$\frac{dA}{dt} = r \frac{dC}{dt} = 2r$$

## Unit 3 

### 3.1 Extreme Value Theorem

**Extreme Value Theorem** - a function $f$ continuous over $[a, b]$ has absolute minimum and absolute maximum over $[a, b]$
-   All extrema must appear at endpoints or critical points
-   Function $f$ has critical point at $x = c$ if $f'(c) = 0$ or $f'(c)$ undefined  

$$ f(x) = \frac{1}{3}x^3 - x^2 - 8x + 12 $$
$$ f'(x) = x^2 - 2x - 8 $$
$$ 0 = (x - 2)(x + 4) \to x = 2, -4 $$
$$ f \text{ has critical points at } x = 2, -4 $$

### 3.2 Mean Value Theorem and Rolle's Theorem 

**Mean Value Theorem** - for a function $f$ continuous from $[a, b]$ and differentiable from $(a, b)$, $\exist$ $c \in (a, b)$ such that $\displaystyle f'(c) = \frac{f(b) - f(a)}{b - a}$
-   There exists a point on a continuous and differentiable function where the slope equals average rate of change
-   **Rolle's Theorem** - for a function $f$ continuous from $[a, b]$, differentiable from $(a, b)$, and $f(a) = f(b)$, $\exist$ $c \in (a, b)$ such that $f'(c) = 0$
    -   MVT where $\text{AROC} = 0$
-   **Differentiability** - function $f$ is differentiable if $f'$ is continuous

### 3.3 First Derivative Test 

**First Derivative Test** - function $f$ has relative maximum when $f'$ changes from positive to negative, and relative minimum when $f'$ changes from negative to positive
-   **Relative Extrema** - $f'$ changes signs
-   $f'$ can only change signs at a critical point

$$ f(x) = \frac{1}{3}x^3 - \frac{5}{2}x^2 + 6x + 2 $$
$$ f'(x) = x^2 - 5x + 6 $$
$$ 0 = (x - 3)(x - 2) \to x = 3, 2 $$

<center>

| | $(-\infty, 2)$ | $(2, 3)$ | $(3, \infty)$ |
| :---: | :---: | :---: | :---: |
| $f'(x)$ | + | - | + |

$f$ has relative maximum at $x = 2$ and relative minimum at $x = 3$

</center>

### 3.4 Second Derivative Test and Concavity

**Second Derivative Test** - when $f'(c) = 0$, if $f''(c) > 0$ then $x = c$ is a relative maximum of $f$, if $f''(c) < 0$ then $x = c$ is a relative minumum of $f$  
-   **Concavity** - $f$ has upwards concavity when $ f''(x) > 0 $ and downwards concavity if $ f''(x) < 0 $
-   **Concavity Point** - function $f$ has concavity point at $x = c$ if $f''(c) = 0$ or $f''(c)$ undefined  
-   **Point of Infection**  - $f''$ changes signs
    -   $f''$ can only change signs at a concavity point

$$ f(x) = \frac{1}{3}x^3 - \frac{5}{2}x^2 + 6x + 2 $$
$$ f'(x) = x^2 - 5x + 6 $$
$$ 0 = (x - 3)(x - 2) \to x = 3, 2 $$
$$ f''(x) = 2x - 5 $$

<center>

| | $(-\infty, \frac{5}{2})$ | $(\frac{5}{2}, \infty)$ |
| :---: | :---: | :---: |
| $f'(x)$ | - | + |

$f$ has relative maximum at $x = 2$ and relative minimum at $x = 3$

</center>


### 3.5 Limits at Infinity

**Horizontal Asymptote** - function $f$ has horizontal asymptote at $y = c$ if $\displaystyle \lim_{x \to -\infty} f(x) = c$ or $\displaystyle \lim_{x \to \infty} f(x) = c$

### 3.6 Derivatives of Position

$$
\begin{align*}
&x(t) \to \text{position} \\
&x'(t) = v(t) \to \text{velocity} \\
&x''(t) = v'(t) = a(t) \to \text{acceleration} \\
\end{align*}
$$
**Speed** - $|v(t)|$, speed increases when $\text{sign}(v(t)) = \text{sign}(a(t))$ and decreases when $\text{sign}(v(t)) = \text{sign}(a(t))$

### 3.7 L'Hôpital

$$
\lim_{x \to c} \frac{f(x)}{g(x)} \to \frac{0}{0} \text{ or } \frac{\pm \infty}{\pm \infty} \implies \lim_{x \to c} \frac{f(x)}{g(x)} = \lim_{x \to c} \frac{f'(x)}{g'(x)}
$$
$$
\lim_{x \to 0} \frac{\sin(x)}{x} = \lim_{x \to 0} \frac{\cos(x)}{1} = 1
$$

### 3.8 Optimization


