# AP Calculus Notes

## Unit 1: Limits

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

-   **One-sided limits** approach a value from only one side, positive or negative: $\displaystyle \lim_{x \to c^+} f(x)$ or $\displaystyle \lim_{x \to c^-} f(x)$ 

-   **Continuity** - at a point $x = c$: $\displaystyle \lim_{x \to c^+} f(x)= \lim_{x \to c^-} f(x) = f(c)$ 
-   **Intermediate Value Theorem** - for a function $f$ continuous over $[a, b]$, $\exists$ $f(c) \in[f(a),f(b)]$ such that $c \in [a, b]$
    -   Function $f$ must pass through all $y$-values between $f(a)$ and $f(b)$ between $a$ and $b$

-   **Extreme Value Theorem** - a function $f$ continuous over $[a, b]$ has absolute minimum and absolute maximum over $[a, b]$

### 1.5 Infinite Limits

-   **Vertical Asymptote** - function $f$ has vertical asymptote at $c$ if $\displaystyle \lim_{x \to c^\pm} f(x) = \pm\infty$
    -   function typically undefined at $c$ $\to$ look for division by 0 etc. 
-   **Horizontal Asymptote** - function $f$ has horizontal asymptote of $k$ if $\displaystyle \lim_{x \to \pm\infty} f(x) = k$
    -   function typically has decreasing rate of change towards infinity $\to$ $\displaystyle \frac{1}{x}, e^x, $ etc.
    -   function has division of similarly growing functions that "cancel" $\to$ $\displaystyle \frac{x + 2}{4x - 3}$

## Unit 2: Derivatives

### 2.1 Derivative Definition

Slope of secant line of function $\to$ $\displaystyle \frac{\Delta f(x)}{\Delta x}$ $\to$ $\displaystyle \frac{f(x + \Delta x) - f(x)}{\Delta x}$  

Slope of tangent line of function $\to$ $\displaystyle \lim_{h \to 0} \frac{f(x + h) - f(x)}{h}$ $\to$ **Derivative Definition**

-   **Derivative Notation**:
$$
\frac{\Delta f(x)}{\Delta x} \xrightarrow{\lim {\Delta x \to 0}} \frac{df(x)}{dx} \xrightarrow{\text{Notation}} \frac{d}{dx} f(x)
$$
<center>or</center>

$$ \frac{d}{dx} f(x) \to f'(x)$$

-   **Derivative** - represents rate of change $\to$ derivative of position $=$ velocity, derivative of velocity $=$ acceleration
$$
\begin{align*}
x(&t)\\
x'(&t) = v(t)\\
x''(&t) = v'(t) = a(t)\\
\end{align*}
$$

### 2.2-2.4 Derivative Rules

-   **Power Rule**: 
$$
\frac{d}{dx} x^n = nx^{n-1}
$$

-   **Trigonometric Functions**:
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

-   **Chain Rule**:
$$ 
\frac{d}{dx} f\big(g(x)\big) = f'\big(g(x)\big) \cdot g'(x)
$$

-   **Product Rule**:
$$ 
\frac{d}{dx} \Big(f(x) \cdot g(x)\Big) = f'(x) \cdot g(x) + f(x) \cdot g'(x)
$$

-   **Quotient Rule**:
$$
\frac{d}{dx} \bigg(\frac{f(x)}{g(x)}\bigg) = \frac{f'(x) \cdot g(x) - f(x) \cdot g'(x)}{\big(g(x)\big)^2}
$$

-   **Logarithm**:
$$
\log_b x = \frac{\ln x}{\ln b} \to \frac{d}{dx} \ln x = \frac{1}{x}
$$

-   **Exponential**:
$$
\frac{d}{dx} \big(b^x\big) = b^x \cdot \ln b
$$

-   **Inverse Trigonometric**:
$$ 
\begin{align*}
\frac{d}{dx} \arcsin(x) &= \frac{1}{\sqrt{1 - x^2}} & 
\frac{d}{dx} \arccos(x) &= \frac{-1}{\sqrt{1 - x^2}}\\ 
\frac{d}{dx} \arctan(x) &= \frac{1}{1 + x^2} & 
\frac{d}{dx} \text{arccot}(x) &= \frac{-1}{1 + x^2} \\
\frac{d}{dx} \text{arcsec}(x) &= \frac{1}{|u|\sqrt{x^2 - 1}} & 
\frac{d}{dx} \text{arccsc}(x) &= \frac{-1}{|u|\sqrt{x^2 - 1}} \\
\end{align*}
$$

-   **General Inverse Functions**:
$$
\frac{d}{dx} f^{-1}(x) = \frac{1}{f'(f^{-1}(x))}
$$

### 2.5 Implicit Differentiation

-   **Implicit Differentiation** - deriving one variable to another variable by treating it as a function of the other, applying chain rule where necessary
$$
\begin{align*}
\frac{d}{dx} \big(x\big) &= 1 \cdot \frac{dx}{dx} = 1 \\
\frac{d}{dx} \big(y\big) &= 1 \cdot \frac{dy}{dx} \\
\end{align*}
$$

### 2.6 Related Rates

-   **Related Rates** - application of implicit differentiation typically on variables related by some equation changing over time: $A = \pi r^2$, $a^2 + b^2 = c^2$, etc.

## Unit 3: Derivative Application

### 3.1 Extreme Value Theorem

-   **Extreme Value Theorem** - a function $f$ continuous over $[a, b]$ has absolute minimum and absolute maximum over $[a, b]$
    -   All extrema must appear at endpoints or critical points
    -   Function $f$ has critical point at $x = c$ if $f'(c) = 0$ or $f'(c)$ undefined  

### 3.2 Mean Value Theorem and Rolle's Theorem 

- **Mean Value Theorem** - for a function $f$ continuous from $[a, b]$ and differentiable from $(a, b)$, $\exist$ $c \in (a, b)$ such that $\displaystyle f'(c) = \frac{f(b) - f(a)}{b - a}$
    -   There exists a point on a continuous and differentiable function where the slope equals average rate of change
    -   **Rolle's Theorem** - for a function $f$ continuous from $[a, b]$, differentiable from $(a, b)$, and $f(a) = f(b)$, $\exist$ $c \in (a, b)$ such that $f'(c) = 0$
        -   MVT where $\text{AROC} = 0$
    -   **Differentiability** - function $f$ is differentiable if $f'$ is continuous

### 3.3 First Derivative Test 

-   **First Derivative Test** - function $f$ has relative maximum when $f'$ changes from positive to negative, and relative minimum when $f'$ changes from negative to positive
    -   **Relative Extrema** - $f'$ changes signs
    -   $f'$ can only change signs at a critical point

### 3.4 Second Derivative Test and Concavity

-   **Second Derivative Test** - when $f'(c) = 0$, if $f''(c) > 0$ then $x = c$ is a relative maximum of $f$, if $f''(c) < 0$ then $x = c$ is a relative minumum of $f$  
    -   **Concavity** - $f$ has upwards concavity when $ f''(x) > 0 $ and downwards concavity if $ f''(x) < 0 $
    -   **Concavity Point** - function $f$ has concavity point at $x = c$ if $f''(c) = 0$ or $f''(c)$ undefined  
    -   **Point of Infection**  - $f''$ changes signs
        -   $f''$ can only change signs at a concavity point

### 3.5 Limits at Infinity

-   **Horizontal Asymptote** - function $f$ has horizontal asymptote at $y = c$ if $\displaystyle \lim_{x \to -\infty} f(x) = c$ or $\displaystyle \lim_{x \to \infty} f(x) = c$

### 3.6 Derivatives of Position

$$
\begin{align*}
&x(t) \to \text{position} \\
&x'(t) = v(t) \to \text{velocity} \\
&x''(t) = v'(t) = a(t) \to \text{acceleration} \\
\end{align*}
$$
-   **Speed** - $|v(t)|$, speed increases when $\text{sign}(v(t)) = \text{sign}(a(t))$ and decreases when $\text{sign}(v(t)) \ne \text{sign}(a(t))$

### 8.7 L'Hôpital

$$
\lim_{x \to c} \frac{f(x)}{g(x)} \to \frac{0}{0} \text{ or } \frac{\pm \infty}{\pm \infty} \implies \lim_{x \to c} \frac{f(x)}{g(x)} = \lim_{x \to c} \frac{f'(x)}{g'(x)}
$$

### 3.7 Optimization

-   **Optimization** - application of related rates, to find the minimum or maximum of an specified value. Found through derivative as all extrema must occur at a slope of 0 
 
### 3.9 Differentials

-   **Differential** - treating $\displaystyle \frac{dy}{dx}$ as a fraction of two real numbers, where $dy$ and $dx$ are the differentials
$$
\begin{align*}
y &= f(x) \\
\frac{dy}{dx} &= f'(x) \\
dy &= f'(x) \cdot dx \\
\end{align*}
$$

-   **Linear Approximation** - constructing a tangent line at a point to approximate function behavior
$$
\begin{align*}
y -  y_1 &= m(x - x_1) \\
y &= y_1 + m(x - x_1) \\
L(x) &= f(x) + f'(x) \Delta x
\end{align*}
$$

-   **Error Propagation** - use of related rates to propagate errors
$$
\begin{align*}
L(x) &= f(x) + f'(x) \Delta x \\
L(x) &= f(x) + \epsilon \\
\Delta x &= \epsilon _\text{in} \\
\epsilon &= f'(x) \epsilon _\text{in}
\end{align*}
$$

-   **Relative Error** - error proportional to true value: $\displaystyle \% \text{error} = \frac{\epsilon}{f(x)} $ 

## Unit 4: Integrals

### 4.1 Antiderivatives and Indefinite Integrals

-   **Antiderivative** - the antiderivative of function $f(x)$ is $F(x)$ such that $F'(x) = f(x)$
    -   $\displaystyle \frac{d}{dx} \big(F(x)\big) = \frac{d}{dx} \big(F(x) + 1\big) = ... = \frac{d}{dx} \big(F(x) + c\big)$

-   **Indefinite Integral** - finding general function $F(x) + c$ for $f(x)$
    -   Notation: $\displaystyle \sum f(x) \Delta x \to \int f(x) dx$ 
    -   Reverse chain rule, power rule

### 4.2 Approximating Area 

-   **Riemann Sums** - Area under curve approximated by regular shapes
    -   Left - $\displaystyle \sum f(x_i) \Delta x$
    -   Right - $\displaystyle \sum f(x_{i+1}) \Delta x$
    -   Midpoint - $\displaystyle \sum f(\frac{x_i + x_{i+1}}{2}) \Delta x$
    -   Trapezoid - $\displaystyle \sum \frac{f(x_i) + f(x_{i+1})}{2} \Delta x$

### 4.3 Definite Integral

-   **Definite Integral** - evaluating integral with bounds 
$$
\lim_{\Delta x \to 0} \sum_{i = a}^b f(x_i) \Delta x = \int_a^b f(x) dx \\
$$ 

### 4.4 The Fundamental Theorem of Calculus

-   **The Fundamental Theorem of Calculus** - differentiation and integration are opposites:
$$
\begin{align*}
\lim_{\Delta x \to 0} \sum_{i = a}^b f(x_i) \Delta x &= \int_a^b f(x) dx \\
&= \Big[F(x) \Big|_a^b \\
&= F(b) - F(a)
\end{align*}
$$ 

-   Particle Motion -
    -   Distance - sum of size of all infinitesimal steps: $\displaystyle \int \big|v(t)\big| dt $
    -   Displacement - total change in position: $\displaystyle v(t) = x'(t) \implies \int_a^b v(t) dt = x(b) - x(a) = \Delta x(t)$ 
    -   Position - final $x$ value: $\displaystyle x(t) = x_0(t) + \int_a^b v(t) dt$ 

-   Bounds Manipulation
$$
\begin{align*}
\int_a^b f(x) dx &= - \int_b^a f(x) dx \\
F(b) - F(a) &= -\big(F(a) - F(b)\big) \\
\\
\int_a^b f(x) dx &= \int_a^c f(x) dx + \int_c^b f(x) dx \\
F(b) - F(a) &= \big(F(b) - F(c)\big) - \big(F(c) - F(a)\big) \\
\end{align*}
$$

-   **Second Fundamental Theorem of Calculus** - for all $x$ on a continuous interval of function $f$ including $a$, $\displaystyle \frac{d}{dx} \Bigg(\int_a^{b(x)} f(t)dt\Bigg) = f(x) \cdot b'(x) $

-   **Average Value** 
$$
\begin{align*}
\text{Standard Average} &= \frac{1}{i}\sum_{n=0}^i a_n \\
\text{Function Average} &= \frac{1}{b - a}\int_a^b f(x) dx
\end{align*}
$$

### 4.5 Integration by Substitution

-   **$u$-Substitution** - reverse chain rule 
    -   Must change integral bounds in terms of $u$ 
$$
\begin{align*}
f(g(x)) \to dy = &f'(g(x))g'(x)dx \\
g(x) = u, \ \ \ \ \ \ \ &g'(x)dx = du \\
f(u) \to dy = &f'(u)du \\
\int f'(u)du = &f(u) + c
\end{align*}
$$

## Unit 5: Integration Application

### 5.1-5.2 Logarithm Integration

$$
\int \frac{1}{x} dx = \ln |x| + c
$$

### 5.3-5.4 Exponential Integration

$$
\int b^x dx = \frac{b^x}{\ln |b|} + c
$$

### 5.6-5.7 Inverse Trig Integration

$$ 
\begin{align*}
\int \frac{1}{\sqrt{a^2 - x^2}} dx &= \arcsin \frac{x}{a} + c \\
\int \frac{1}{x\sqrt{x^2 - a^2}} dx &= \text{arcsec} \frac{x}{a} + c \\
\int \frac{1}{a^2 + x^2} dx &= \frac{1}{a} \arctan \frac{x}{a} + c \\
\end{align*}
$$