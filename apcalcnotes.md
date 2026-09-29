# Calculus Notes

## Limits

### Calculus Principles

| Without Calculus | With Calculus |
| --- | --- |
| Approximate area using rectangles | Exact area under curve |
| Average rate of change | Instantaneous rate of change |
| Length of line segments | Length of arcs |
| Finite sums | Infinite sums |
| Volume of regular solids | Volume of arbitrary solids | 

### Limits

-   **Limit** - value that a function approaches: $\displaystyle \lim_{x \to c} f(x)$ 
-   To solve:
    1.  Plug in directly. If undefined, continue
    2.  Factor, simplify, rationalize
    3.  Find limit on graph
    4.  Analyze limit
    5.  L'Hôpital's rule

### Continuity and One-Sided Limits

-   **One-sided limits** approach a value from only one side, positive or negative: $\displaystyle \lim_{x \to c^+} f(x)$ or $\displaystyle \lim_{x \to c^-} f(x)$ 

-   **Continuity** - at a point $x = c$: $\displaystyle \lim_{x \to c^+} f(x)= \lim_{x \to c^-} f(x) = f(c)$ 
-   **Intermediate Value Theorem** - for a function $f$ continuous over $[a, b]$, $\exists$ $f(c) \in[f(a),f(b)]$ such that $c \in [a, b]$
    -   Function $f$ must pass through all $y$-values between $f(a)$ and $f(b)$ between $a$ and $b$

-   **Extreme Value Theorem** - a function $f$ continuous over $[a, b]$ has absolute minimum and absolute maximum over $[a, b]$

### Infinite Limits

-   **Vertical Asymptote** - function $f$ has vertical asymptote at $c$ if $\displaystyle \lim_{x \to c^\pm} f(x) = \pm\infty$
    -   function typically undefined at $c$ $\to$ look for division by 0 etc. 
-   **Horizontal Asymptote** - function $f$ has horizontal asymptote of $k$ if $\displaystyle \lim_{x \to \pm\infty} f(x) = k$
    -   function typically has decreasing rate of change towards infinity $\to$ $\displaystyle \frac{1}{x}, e^x, $ etc.
    -   function has division of similarly growing functions that "cancel" $\to$ $\displaystyle \frac{x + 2}{4x - 3}$

## Derivatives

### Derivative Definition

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

### Derivative Rules

-   **Constant Rule**: 
$$
\frac{d}{dx} c = 0
$$

-   **Sum Rule**: 
$$
\frac{d}{dx} \Big( f(x) + g(x) \Big) = f'(x) + g'(x)
$$

-   **Power Rule**: 
$$
\frac{d}{dx} x^n = nx^{n-1}
$$

-   **Trigonometric Functions**:
$$ 
\begin{align*}
\frac{d}{dx} \sin x &= \cos x & 
\frac{d}{dx} \cos x &= -\sin x\\ 
\frac{d}{dx} \tan x &= \sec^2 x & 
\frac{d}{dx} \cot x &= -\csc^2 x \\
\frac{d}{dx} \sec x &= \sec x \tan x & 
\frac{d}{dx} \csc x &= -\csc x \cot x \\
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
\frac{d}{dx} \arcsin x &= \frac{1}{\sqrt{1 - x^2}} & 
\frac{d}{dx} \arccos x &= \frac{-1}{\sqrt{1 - x^2}}\\ 
\frac{d}{dx} \arctan x &= \frac{1}{1 + x^2} & 
\frac{d}{dx} \text{arccot} x &= \frac{-1}{1 + x^2} \\
\frac{d}{dx} \text{arcsec} x &= \frac{1}{|u|\sqrt{x^2 - 1}} & 
\frac{d}{dx} \text{arccsc} x &= \frac{-1}{|u|\sqrt{x^2 - 1}} \\
\end{align*}
$$

-   **General Inverse Functions**:
$$
\frac{d}{dx} f^{-1}(x) = \frac{1}{f'(f^{-1}(x))}
$$

### Implicit Differentiation

-   **Implicit Differentiation** - deriving one variable to another variable by treating it as a function of the other, applying chain rule where necessary
$$
\begin{align*}
\frac{d}{dx} \big(x\big) &= 1 \cdot \frac{dx}{dx} = 1 \\
\frac{d}{dx} \big(y\big) &= 1 \cdot \frac{dy}{dx} \\
\end{align*}
$$

### Related Rates

-   **Related Rates** - application of implicit differentiation typically on variables related by some equation changing over time: $A = \pi r^2$, $a^2 + b^2 = c^2$, etc.

## Derivation Application

### Extreme Value Theorem

-   **Extreme Value Theorem** - a function $f$ continuous over $[a, b]$ has absolute minimum and absolute maximum over $[a, b]$
    -   All extrema must appear at endpoints or critical points
    -   Function $f$ has critical point at $x = c$ if $f'(c) = 0$ or $f'(c)$ undefined  

### Mean Value Theorem and Rolle's Theorem 

- **Mean Value Theorem** - for a function $f$ continuous from $[a, b]$ and differentiable from $(a, b)$, $\exist$ $c \in (a, b)$ such that $\displaystyle f'(c) = \frac{f(b) - f(a)}{b - a}$
    -   There exists a point on a continuous and differentiable function where the slope equals average rate of change
    -   **Rolle's Theorem** - for a function $f$ continuous from $[a, b]$, differentiable from $(a, b)$, and $f(a) = f(b)$, $\exist$ $c \in (a, b)$ such that $f'(c) = 0$
        -   MVT where $\text{AROC} = 0$
    -   **Differentiability** - function $f$ is differentiable if $f'$ is continuous

### First Derivative Test 

-   **First Derivative Test** - function $f$ has relative maximum when $f'$ changes from positive to negative, and relative minimum when $f'$ changes from negative to positive
    -   **Relative Extrema** - $f'$ changes signs
    -   $f'$ can only change signs at a critical point

### Second Derivative Test and Concavity

-   **Second Derivative Test** - when $f'(c) = 0$, if $f''(c) > 0$ then $x = c$ is a relative maximum of $f$, if $f''(c) < 0$ then $x = c$ is a relative minumum of $f$  
    -   **Concavity** - $f$ has upwards concavity when $ f''(x) > 0 $ and downwards concavity if $ f''(x) < 0 $
    -   **Concavity Point** - function $f$ has concavity point at $x = c$ if $f''(c) = 0$ or $f''(c)$ undefined  
    -   **Point of Infection**  - $f''$ changes signs
        -   $f''$ can only change signs at a concavity point

### Limits at Infinity

-   **Horizontal Asymptote** - function $f$ has horizontal asymptote at $y = c$ if $\displaystyle \lim_{x \to -\infty} f(x) = c$ or $\displaystyle \lim_{x \to \infty} f(x) = c$

### Derivatives of Position

$$
\begin{align*}
&x(t) \to \text{position} \\
&x'(t) = v(t) \to \text{velocity} \\
&x''(t) = v'(t) = a(t) \to \text{acceleration} \\
\end{align*}
$$
-   **Speed** - $|v(t)|$, speed increases when $\text{sign}(v(t)) = \text{sign}(a(t))$ and decreases when $\text{sign}(v(t)) \ne \text{sign}(a(t))$

### L'Hôpital

$$
\lim_{x \to c} \frac{f(x)}{g(x)} \to \frac{0}{0} \text{ or } \frac{\pm \infty}{\pm \infty} \implies \lim_{x \to c} \frac{f(x)}{g(x)} = \lim_{x \to c} \frac{f'(x)}{g'(x)}
$$

### Optimization

-   **Optimization** - application of related rates, to find the minimum or maximum of an specified value. Found through derivative as all extrema must occur at a slope of 0 
 
### Differentials

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

## Integrals

### Antiderivatives and Indefinite Integrals

-   **Antiderivative** - the antiderivative of function $f(x)$ is $F(x)$ such that $F'(x) = f(x)$
    -   $\displaystyle \frac{d}{dx} \big(F(x)\big) = \frac{d}{dx} \big(F(x) + 1\big) = ... = \frac{d}{dx} \big(F(x) + c\big)$

-   **Indefinite Integral** - finding general function $F(x) + c$ for $f(x)$
    -   Notation: $\displaystyle \sum f(x) \ \Delta x \to \int f(x) \ dx$ 
    -   Reverse chain rule, power rule

### Approximating Area 

-   **Riemann Sums** - area under curve approximated by regular shapes
    -   Left - $\displaystyle \sum f(x_i) \ \Delta x$
    -   Right - $\displaystyle \sum f(x_{i+1}) \ \Delta x$
    -   Midpoint - $\displaystyle \sum f(\frac{x_i + x_{i+1}}{2}) \ \Delta x$
    -   Trapezoid - $\displaystyle \sum \frac{f(x_i) + f(x_{i+1})}{2} \ \Delta x$

### Definite Integral

-   **Definite Integral** - evaluating integral with bounds 
$$
\lim_{\Delta x \to 0} \sum_{i = a}^b f(x_i) \ \Delta x = \int_a^b f(x) \ dx \\
$$ 

### The Fundamental Theorem of Calculus

-   **The Fundamental Theorem of Calculus** - differentiation and integration are opposites:
$$
\begin{align*}
\lim_{\Delta x \to 0} \sum_{i = a}^b f(x_i) \ \Delta x &= \int_a^b f(x) \ dx \\
&= \Big[F(x) \Big|_a^b \\
&= F(b) - F(a)
\end{align*}
$$ 

-   Particle Motion -
    -   Distance - sum of size of all infinitesimal steps: $\displaystyle \int \big|v(t)\big| \ dt $
    -   Displacement - total change in position: $\displaystyle v(t) = x'(t) \implies \int_a^b v(t) \ dt = x(b) - x(a) = \Delta x(t)$ 
    -   Position - final $x$ value: $\displaystyle x(t) = x_0(t) + \int_a^b v(t) \ dt$ 

-   Bounds Manipulation
$$
\begin{align*}
\int_a^b f(x) \ dx &= - \int_b^a f(x) \ dx \\
F(b) - F(a) &= -\big(F(a) - F(b)\big) \\
\\
\int_a^b f(x) \ dx &= \int_a^c f(x) dx + \int_c^b f(x) \ dx \\
F(b) - F(a) &= \big(F(b) - F(c)\big) - \big(F(c) - F(a)\big) \\
\end{align*}
$$

-   **Second Fundamental Theorem of Calculus** - for all $x$ on a continuous interval of function $f$ including $a$, $\displaystyle \frac{d}{dx} \Bigg(\int_a^{b(x)} f(t) \ dt\Bigg) = f(x) \cdot b'(x) $

-   **Average Value** 
$$
\begin{align*}
\text{Standard Average} &= \frac{1}{i}\sum_{n=0}^i a_n \\
\text{Function Average} &= \frac{1}{b - a}\int_a^b f(x) \ dx
\end{align*}
$$

### Integration by Substitution

-   **$u$-Substitution** - reverse chain rule 
    -   Must change integral bounds in terms of $u$ 
$$
\begin{align*}
f(g(x)) \to dy = &f'(g(x))g'(x) \ dx \\
g(x) = u, \ \ \ \ \ \ \ &g'(x) \ dx = du \\
f(u) \to dy = &f'(u) \ du \\
\int f'(u) \ du = &f(u) + c
\end{align*}
$$

## Integration Application

### Logarithm Integration

$$
\int \frac{1}{x} \ dx = \ln |x| + c
$$

### Exponential Integration

$$
\int b^x \ dx = \frac{b^x}{\ln |b|} + c
$$

### Inverse Trig Integration

$$ 
\begin{align*}
\int \frac{1}{\sqrt{a^2 - x^2}} \ dx &= \arcsin \frac{x}{a} + c \\
\int \frac{1}{x\sqrt{x^2 - a^2}} \ dx &= \text{arcsec} \frac{x}{a} + c \\
\int \frac{1}{a^2 + x^2} \ dx &= \frac{1}{a} \arctan \frac{x}{a} + c \\
\end{align*}
$$

## Differential Equations

### Slope Fields

-   **Slope Field** - each point on a coordinate system represents the slope of a differential equation

![slope field image for dy/dx = y*sin x - (cos x)*e^(-cos x)](https://www.savemyexams.com/ap/maths/college-board/calculus-ab/20/revision-notes/differential-equations/first-order-differential-equations/slope-fields/)

-   **Euler's Method** - iteratively determine particular solution of differential equation using multiple linear approximations: $\displaystyle f_\text{next}(x) = f(x) + \frac{dy}{dx}\Big|_{(x, y)} \Delta x$

### Exponential Growth and Decay

-   Rate of change proportional to current value
$$
\begin{align*}
\frac{d}{dt}& (y = ke^t) \\
\frac{dy}{dt}& = ke^t \\
\frac{dy}{dt}& = ky
\end{align*}
$$

-   **Logistic Differential Equation** - exponential growth with a load limit $L$, starting value $a$, and growth rate $k$: $\displaystyle \frac{dy}{dt} = ky(1 - \frac{y}{L})$, $\displaystyle y(t) = \frac{L}{1 + ae^{-kt}}$

### Separation of Variables

-   Integrate differential equations with all instance of variables isolated on one side
    -   $\displaystyle \frac{dy}{dx} = xy \to \frac{dy}{y} = x dx \to \int \frac{dy}{y} = \int x \ dx$

## Integration Application

### Area Between Curves 

-   Area between functions $f(x)$ and $g(x)$ where $f(x) > g(x)$ on $[a, b]$ = $\displaystyle \int_a^b \big(f(x) - g(x)\big) \ dx$

### Area of Regions

-   **Disc Method**:
$$ 
\text{Area of disc} = \pi r^2 \\
\sum \text{Area of disc} = \pi \int \big(r(x)\big)^2 \ dx
$$

-   **Washer Method**:
$$ 
\text{Area of washer} = \pi (R^2 - r^2)\\
\sum \text{Area of washer} = \pi \int \big(R(x)\big)^2 - \big(r(x)\big)^2 \ dx
$$

-   **Shell Method**:
$$ 
\text{Surface Area of cylinder} = 2 \pi rh\\
\sum \text{SA}  = 2 \pi \int \big(r(x) \cdot h(x)\big) \ dx
$$

-   **Cross Sections** - given a cross sectional area $A(y)$ as a function of $f(x)$: $\displaystyle \text{Volume} = \int A(f(x)) \ dx$


### Arc Length and Surface Area

-   **Arc Length**:
$$
\begin{align*}
c^2 &= a^2 + b^2 \\
d &= \sqrt{(\Delta x)^2 + (\Delta y)^2} \\
s &= \int \sqrt{dx^2 + dy^2} \\
s &= \int \Bigg(\sqrt{1 + \Big(\frac{dy}{dx}\Big)^2}\Bigg) dx \\
\end{align*}
$$

-   **Surface Area**:
$$
\text{SA} = 2 \pi \int \Bigg(r(x) \sqrt{1 + \Big(\frac{dy}{dx}\Big)^2}\Bigg) dx 
$$

## Advanced Integration 

### Basic Integration

-   Expand numerator
-   Separate numerator
-   Complete the square
-   Rational long division
-   Add and subtract from numerator
-   Use trig identities
-   Multiply and divide by conjugate

### Integration by Parts

-   **Integration by Parts**:
$$ 
\begin{align*}
\frac{d}{dx} \Big(f(x) \cdot g(x)\Big) &= f'(x) \cdot g(x) + f(x) \cdot g'(x) \\
d (uv) &= u \ dv + v \ du \\
u \ dv &= d (uv) - v \ du \\
\int u \ dv &= uv - \int v \ du \\
\end{align*}
$$

-   **Tabular Method**:
    -   Add row product per column, skipping one row down for $dv$ column  

| $\text{sign}$ | $u$ | $dv$ |
| :---: | :---: | :---: |
| $+$ | $u$ | $dv$ |
| $-$ | $du$ | $\int dv$ |
| $+$ | $ddu$ | $\int \int dv$ |
| $...$ | $...$ | $...$ |
| $...$ | 0 | $...$ |

-   **Recursive Integration**:
$$
\begin{align*}
I = \int u \ dv &= uv - \int \Big(du \ v\Big) \\
\int du \ v &= ddu \int v - \int \Big(ddu \int v\Big) \\
\int ... &= ... \ - c \cdot I \\
(c+1) \cdot I &= ...
\end{align*}
$$

### Partial Fractions

-   **Partial Fraction Decomposition**:
$$ 
\begin{align*}
\frac{A}{P} + \frac{B}{Q} = \frac{AQ}{PQ} + \frac{BP}{PQ} &= \frac{AQ + BP}{PQ} \\
N &= AQ + BP \\
\int \frac{N}{PQ} \ dx &= \int \frac{A}{P} \ dx + \int \frac{B}{Q} \ dx \\
B &= \frac{N}{P(x)\big|_{x, Q(x) = 0}} \\
A &= \frac{N}{Q(x)\big|_{x, P(x) = 0}} \\
\end{align*}
$$

### Trig Substitution

-   **Trig Substitution** - using trig identities to replace radicals with known trig function:
$$
\begin{align*}
\sqrt{a^2 - x^2} &\to 1 - \sin^2 \theta \\
\sqrt{a^2 + x^2} &\to 1 + \tan^2 \theta \\
\sqrt{x^2 - a^2} &\to \sec^2 \theta - 1 \\
\end{align*}
$$

### Improper Integrals 

-   **Improper Integrals** - integrals that contain value within bounds that are undefined in the integrand
    -   $\displaystyle \int_0^\infty f(x) \ dx \to \lim_{b \to \infty} \int_0^b f(x) \ dx \to \lim_{b \to \infty} \Big[F(x)\Big|_0^b \to \lim_{b \to \infty} F(b) - F(0)$

## Infinite Sequences and Series

### Sequences 

-   **Sequence** - a function whose domain is $\mathbb{N}$

-   **Convergence of an Infinite Series** -
    -   **Convergence** - sequence approaches a limiting value at infinity
    -   **Divergence** - sequence does not have a limit at infinity

-   **Absolute Value Theorem** - $\displaystyle \lim_{n \to \infty} \big|a_n\big| = 0 \implies \lim_{n \to \infty} a_n = 0$

-   **Monotonic** - all terms are all nonincreasing or all nondecreasing

-   **Bounded** - bounded above if all terms $\le$ constant $c$ and bounded below if all terms $\ge c$ 

### Infinite Series 

-   **Series** - sum of first $n$ terms of sequence: $\displaystyle \sum_{i = 1}^n a_i$
    -   **Infinite Series** - sum of all terms in a sequence: $\displaystyle \sum_{n}^\infty a_n$
        -   **Convergence** - sum approaches a limiting value at infinity
        -   **Divergence** - sum does not have a limit at infinity


### Convergence Tests 

-   **Telescoping Series** - series with terms canceling, leaving a finite sum
    -   Often requires partial fraction decomposition
    -   Finite sum $\to$ always converge

-   **Geometric Series** - series with common ratio between terms: $\displaystyle \sum_{n}^\infty ar^n$
    -   Converges if $|r| < 1$, to $\displaystyle \frac{a}{1 - r}$
    -   Diverges otherwise, $|r| \ge 1$

-   **$n$-th Term Test** - if $\displaystyle \lim_{n \to \infty} a_n \ne 0$, then $\displaystyle \sum_{n}^\infty a_n$ diverges

-   **$p$-Series** - $\displaystyle \sum_n^\infty \frac{1}{n^p}$
    -   Converges if $p > 1$
    -   Diverges otherwise, $p \le 1$

-   **Integral Test** - $f(n) = a_n$, if $f(n)$ is positive, continuous, and decreasing for $k \ge 1$, then $\displaystyle \sum_{n = k}^\infty a_n$ and $\displaystyle \int_{k}^\infty f(x) \ dx$ share convergence behavior

-   **Direct Comparison Test** - $0 < a_n < b_n \ \forall \ n$:
$$ 
\begin{align*}
\sum_{n = k}^\infty b_n \ \ \text{convergence} &\implies \displaystyle \sum_{n = k}^\infty a_n \ \ \text{convergence} \\
\sum_{n = k}^\infty a_n \ \ \text{divergence} &\implies \displaystyle \sum_{n = k}^\infty b_n \ \ \text{divergence}
\end{align*}
$$

-   **Limit Comparison Test** - if $a_n > 0$ and $\displaystyle b_n > 0 \ \forall \ n$ and $\displaystyle \lim_{n \to \infty} \frac{a_n}{b_n}$ finite and positive, then $\displaystyle \sum_{n = k}^\infty b_n$ and $\displaystyle \sum_{n = k}^\infty a_n$ share convergence behavior

-   **Alternating Series Test** - series that alternates signs: $a_n > 0$, $\displaystyle \sum_{n = 1}^\infty (-1)^n a_n$ 
    -   Converges if $\displaystyle \lim_{n \to \infty} a_n = 0$ and $a_{n + 1} \le a_n \ \forall \ n$ 
    -   **Absolute Convergence** - series $\displaystyle \sum a_n$ is absolutely convergent if $\displaystyle \sum |a_n|$ converges
    -   **Conditional Convergence** - series $\displaystyle \sum a_n$ is conditionally convergent if $\displaystyle \sum a_n$ converges but $\displaystyle \sum |a_n|$ diverges 
    -   **Alternating Series Remainder** - sum of alternating series $S$ can be approximated by $|S - S_n| \le a_{n + 1}$

-   **Ratio Test** - series $\displaystyle \sum a_n$:
    -   Converges if $\displaystyle \lim_{n \to \infty} \Big|\frac{a_{n + 1}}{a_n}\Big| < 1$

    -   Diverges if $\displaystyle \lim_{n \to \infty} \Big|\frac{a_{n + 1}}{a_n}\Big| > 1$

-   **Root Test** - series $\displaystyle \sum a_n$:
    -   Converges if $\displaystyle \lim_{n \to \infty} \sqrt[n]{|a_n|} < 1$
    -   Diverges if $\displaystyle \lim_{n \to \infty} \sqrt[n]{|a_n|} > 1$

### Taylor Polynomials and Approximation

-   Linear approximation as a first degree polynomial approximation $\to$ matches value and slope at point
-   **Taylor Polynomial** - approximation at $x = c$:
$$
P_a(x) = \sum_{n = 0}^a \frac{f^n(c)}{n!} (x - c)^n
$$
-   **Maclaurin Polynomial** - approximation at $x = 0$:
$$
P_a(x) = \sum_{n = 0}^a \frac{f^n(0)}{n!} x^n
$$

-   **Lagrange Error Bound** - difference between function Taylor polynomial approximation:
$$
|f(x) - P_n(x)| = \frac{\displaystyle \max_{[c, x]}\big|f^{n + 1}(x)\big|}{(n + 1)!} (x - c)^{n + 1}
$$

### Power Series

-   **Power Series** - infinite polynomial approximation centered at $x = c$:
$$
\sum_{n = 0}^\infty a_n (x - c)^n
$$

-   **Radius of Convergence** - $R > 0$ such that the power series converges for $|x - c| < R$ and diverges otherwise
    -   Series converges for all $x$
    -   Series converges only at $x = c$

-   **Interval of Convergence** - exact bounds on $x$ where power series converges
    -   On interval on convergence, series is differentiable and continuous

-   Series derives and antiderives with respect to $x$, treating $n$ as a real number
    -   Derivative and antiderivative have same bounds, but inclusivity must be rechecked

### Functions as Power Series

-   Function into geometric series:
$$
\begin{align*}
\sum_{n = 1}^\infty ar^n &= \frac{a}{1 - r} \\
\frac{a}{1 - x} &= \sum_{n = 1}^\infty ax^n 
\end{align*}
$$

### Taylor Series

-   **Taylor Series** - infinite polynomial approximation of a function centered at $x = c$:
$$
\begin{align*}
P_a(x) &= \sum_{n = 0}^a \frac{f^n(c)}{n!} (x - c)^n \\
f(x) &= \sum_{n = 0}^\infty \frac{f^n(c)}{n!} (x - c)^n
\end{align*}
$$
-   Examples:
$$
\begin{align*}
e^x &= \sum_{n = 0}^\infty \frac{x^n}{n!} \\
\sin x &= \sum_{n = 0}^\infty (-1)^n \frac{x^{2n + 1}}{(2n + 1)!} \\
\cos x &= \sum_{n = 0}^\infty (-1)^n \frac{x^{2n}}{(2n)!} \\
\frac{1}{x} &= \sum_{n = 0}^\infty (-1)^n (x - 1)^n
\end{align*}
$$

-   Function composition works within power series: $\displaystyle e^{2x} = \sum_{n = 0}^\infty \frac{(2x)^n}{n!}$

## Polar, Parametric, and Vector Functions

### Parametric Equations 

-   **Parametric Equations** - sets of equations with more than one dependent variable, independent usually being time $t$
    -   Derivative where curve is given by $x = f(t)$ and $y = g(t)$: $\displaystyle \frac{dy}{dx} = \frac{dy/dt}{dx/dt}$
    -   Second derivative: $\displaystyle \frac{d^2y}{dx^2} = \frac{\frac{d}{dt} (dy/dx)}{dx/dt}$

-   **Vector** - ordered list of points
    -   Position vector: $\displaystyle \vec{x} = \langle x(t), y(t) \rangle$
    -   Velocity vector: $\displaystyle \vec{v} = \langle x'(t), y'(t) \rangle$
    -   Acceleration vector: $\displaystyle \vec{a} = \langle x''(t), y''(t) \rangle$
    -   **Magnitude** of vector - distance to origin: $\displaystyle \sqrt{(x(t))^2 + (y(t))^2}$
        -   **Speed** - magnitude of velocity vector

-   **Arc Length** - $\displaystyle \int \sqrt{(x(t))^2 + (y(t))^2} dt$

### Polar Functions

-   **Polar Coordinates** - point on plane represented by radial distance $r$ and angle $\theta$ instead of $x$ and $y$
    -   $r = \sqrt{x^2 + y^2}$
    -   $\theta = \arctan(\frac{y}{x})$

-   Polar function $r = f(\theta)$, $\theta$ can be treated as parameter of $x$ and $y$
    -   Derivative: $\displaystyle \frac{dy}{dx} = \frac{dy/d\theta}{dx/d\theta}$
    -   Area bounded by polar curve: 

$$
\begin{align*}
A_C = \pi r^2 \\
A_C = \frac{1}{2} (\theta = 2 \pi) r^2 \\
A_S = \frac{1}{2} \theta r^2 \\
dA_S = \frac{1}{2} r^2 d\theta \\
A = \frac{1}{2} \int r^2 d\theta
\end{align*}
$$

## Vectors and Space

### Vectors

-   **Scalar** - real number, 0 dimensional, magnitude without direction
-   **Vector** - directed segment, with direction and magnitude
    -   **Magnitude** - length of vector: $|\vec{v}|$
    -   **Equivalence** - same direction and magnitude
    -   **Parallelism** - vectors with the same direction, scalar multiples of each other, cross product of $\vec{0}$
        -   $\vec{0}$ is parallel to all vectors
    -   **Orthogonality** - vectors with the perpendicular direction, dot product of 0
        -   $\vec{0}$ is orthogonal to all vectors
    -   **Position Vectors** - standard form of vector, with tail at origin, written: $\langle v_1, v_2, ..., v_n \rangle$
        -   $v_1, v_2, v_3$ are the $x$-component, $y$-component, and $z$-component of vectors in $\mathbb{R}^3$
-   **Unit Vectors** - vector with length $1$, represented with $\hat{u}$
    -   **Coordinate Unit Vectors** - $\hat{i} = \langle 1, 0, 0 \rangle$, $\hat{j} = \langle 0, 1, 0 \rangle$,  $\hat{k} = \langle 0, 0, 1 \rangle$
        -   vector $\vec{u} = \langle u_1, u_2, u_3 \rangle = u_1\hat{i} + u_2\hat{j} + u_3\hat{k}$
    -   vector with length $|\vec{u}|$ and angle $\theta$ in $\mathbb{R}^2$: $|\vec{v}|\langle \cos \theta, \sin \theta \rangle$
### Vector Operations 
-   **Vector Addition**:
$$
\vec{u} + \vec{v} = \langle u_1 + v_1, u_2 + v_2, ..., u_n + v_n \rangle
$$
-   **Vector Subtraction**:
$$
\vec{u} - \vec{v} = \langle u_1 - v_1, u_2 - v_2, ..., u_n - v_n \rangle
$$
-   **Scalar Multiplication**
$$
c\vec{u} = \langle cu_1, cu_2, ..., cu_n \rangle
$$
-   **Dot Product** - how much of a vector is pointing along another - given two vectors $\vec{u}$ and $\vec{v}$ with angle $\theta \in [0, \pi]$:
$$
\vec{u} \cdot \vec{v} = |\vec{u}||\vec{v}|\cos \theta \\
\text{or} \\
\vec{u}\cdot\vec{v} = u_1v_1 + u_2v_2 + ... + u_nv_n 
$$
    -   by law of cosines, 
$$
\begin{align*}
|\vec{u} - \vec{v}|^2 &= |\vec{u}|^2 + |\vec{v}|^2 - 2|\vec{u}||\vec{v}|\cos \theta \\
2|\vec{u}||\vec{v}|\cos \theta &= |\vec{u}|^2 + |\vec{v}|^2 - |\vec{u} - \vec{v}|^2 \\
2\vec{u} \cdot \vec{v} &= |\vec{u}|^2 + |\vec{v}|^2 - |\vec{u} - \vec{v}|^2 \\
2\vec{u} \cdot \vec{v} &= u_1^2 + u_2^2 + v_1^2 + v_2^2 - (u_1 + v_1)^2 - (u_2 + v_2)^2 \\
2\vec{u} \cdot \vec{v} &= 2u_1v_1 + 2u_2v_2 \\
\vec{u} \cdot \vec{v} &= u_1v_1 + u_2v_2 \\
\end{align*}
$$
    -   returns a scalar, vectors are parallel if $\vec{u} \cdot \vec{v} = |\vec{u}||\vec{v}|$, and perpendicular or orthogonal if $\vec{u} \cdot \vec{v} = 0$ 
    -   $\displaystyle \cos(\theta) = \frac{\vec{u} \cdot \vec{v}}{|\vec{u}||\vec{v}|}$
    -   Properties
        -   Commutative: $\vec{u} \cdot \vec{v} = \vec{v} \cdot \vec{u}$
        -   Associative: $(\vec{u} \cdot \vec{v}) \cdot \vec{w} =\vec{u} \cdot (\vec{v} \cdot \vec{w})$
        -   Distributive: $\vec{u} \cdot (\vec{v} + \vec{w}) = \vec{u} \cdot \vec{v} + \vec{v} \cdot \vec{w}$
    -   **Work** - $W = \vec{F} \cdot \vec{d}$
-   **Magnitude**:
$$
\begin{align*}
|\vec{u}| &= \sqrt{u_1^2 + u_2^2 + ... + u_n^2} \\
&\text{ or} \\
|\vec{u}| &= \sqrt{\vec{u} \cdot \vec{u}}
\end{align*}
$$
-   **Projection** - vector projection of $\vec{u}$ on $\vec{v}, \vec{v} \ne 0$:
$$
\begin{align*}
\text{proj}_{\vec{v}} \vec{u} &= |\vec{u}|\cos \theta \frac{\vec{v}}{|\vec{v}|} \\
\text{proj}_{\vec{v}} \vec{u} &= \text{scal}_{\vec{v}} \vec{u} \frac{\vec{v}}{|\vec{v}|} \\
\text{proj}_{\vec{v}} \vec{u} &= \frac{\vec{u} \cdot \vec{v}}{\vec{v} \cdot \vec{v}}
\end{align*}
$$
-   **Scale** - length of projection of $\vec{u}$ on $\vec{v}, \vec{v} \ne 0$:
$$
\begin{align*}
\text{scal}_{\vec{v}} \vec{u} &= |\vec{u}|\cos \theta \\
\text{scal}_{\vec{v}} \vec{u} &= |\text{proj}_{\vec{v}} \vec{u}| \\ 
\text{scal}_{\vec{v}} \vec{u} &= \frac{\vec{u} \cdot \vec{v}}{|\vec{v}|}
\end{align*}
$$
-   **Cross Product** - vector with length of parallelogram formed by two vectors pointed orthogonally given by right-hand rule, given two vectors $\vec{u}$ and $\vec{v}$ with angle $\theta \in [0, \pi]$:
$$
\begin{align*}
|\vec{u} \times \vec{v}| &= |\vec{u}||\vec{v}|\sin \theta \\
\vec{u} \times \vec{v} &= 
\begin{vmatrix}
    \hat{i} & \hat{j} & \hat{k} \\
    u_1 & u_2 & u_3 \\
    v_1 & v_2 & v_3 \\
\end{vmatrix}
\end{align*}
$$    
    -   Properties
        -   Anticommutative: $\vec{u} \times \vec{v} = -(\vec{v} \times \vec{u})$
        -   Distributive: $\vec{u} \times (\vec{v} + \vec{w}) = \vec{u} \times \vec{v} + \vec{v} \times \vec{w}$ and $(\vec{u} + \vec{v}) \times \vec{w} = \vec{u} \times \vec{w} + \vec{v} \times \vec{w}$
    -   **Torque** - torque $\vec{\tau}$ given pivot $\vec{r}$ and force $\vec{F}$: $\vec{\tau} = \vec{r} \times \vec{F}$
    -   **Magnetic Force** - force $\vec{F}$ given charge $q$ and velocity of moving charge $\vec{v}$ and magnetic field $\vec{B}$: $\vec{F} = q(\vec{v} \times \vec{B})$

### Space 

-   **Sphere** - all points $(x, y, z)$ in 3 dimensions with distance $r$ to center at $(x_0, y_0, z_0)$, equation given by $(x - x_0)^2 + (y - y_0)^2 + (z - z_0)^2 = r^2$ 
-   **Line** - line with fixed point at $(x_0, y_0, z_0)$ and points along $(a, b, c)$, its equation is given by $\langle x, y, z \rangle = \langle x_0, y_0, z_0 \rangle + t\langle a, b, c \rangle$ for $t \in \mathbb{R}$
    -   $\vec{r} = \vec{r_0} + t\vec{v}$ for $t \in \mathbb{R}$
    -   **Distance to Point** - point $Q$ distance to line at point $Q'$ given point $P$ on line with direction $\vec{v}$ is height of parallelogram formed of $P, Q, P + \vec{v}$: $|PQ'| = |\vec{v} \times |\overrightarrow{PQ}|$
-   **Plane** - plane is defined with 3 noncollinear points, or a point $P$ and a normal vector $\vec{n}$. Any point $P_0$ on plane must be orthogonal to normal vector, so $\vec{n} \cdot \overrightarrow{P_0 P} = 0$. 
$$
\begin{align*}
\vec{n} &= \langle a, b, c \rangle \\
\overrightarrow{P_0 P} &= \langle x - x_0, y - y_0, z - z_0 \rangle \\
\vec{n} \cdot \overrightarrow{P_0 P} &= 0 \\
a(x - x_0) + b(y - y_0) + c(z - z_0) &= 0 \\
ax + by + cz &= ax_0 + by_0 + cz_0 \\
ax + by + cz &= d
\end{align*}
$$
    -   **Trace** - line where plane intersects coordinate plane
    -   **Parallelism** - planes are parallel if their normal vectors are parallel, $\vec{n_1} = c\vec{n_2}$
    -   **Orthogonality** - planes are parallel if their normal vectors are parallel, $\vec{n_1} = c\vec{n_2}$
-   **Cylinders** - projection of a 2 dimensional line onto a third parallel coordinate line, missing a variable
-   **Quadric Surface** - second degree equation of three variables, with general form: $Ax^2 + By^2 + Cz^2 + Dxy + Exz + Fyx + Gx + Hy + Iz + J = 0$
    -   **Ellipsiod**: 
    $$\displaystyle \frac{x^2}{a^2} + \frac{y^2}{b^2} + \frac{z^2}{c^2} = 1$$
    -   **Elliptic Paraboloid**: 
    $$\displaystyle \frac{x^2}{a^2} + \frac{y^2}{b^2} = z$$
    -   **Hyperboloid of One Sheet**: 
    $$\displaystyle \frac{x^2}{a^2} + \frac{y^2}{b^2} - \frac{z^2}{c^2} = 1$$
    -   **Hyperboloid of Two Sheet**: 
    $$\displaystyle \frac{x^2}{a^2} - \frac{y^2}{b^2} - \frac{z^2}{c^2} = 1$$
    -   **Elliptic Cone**: 
    $$\displaystyle \frac{x^2}{a^2} + \frac{y^2}{b^2} = \frac{z^2}{c^2}$$
    -   **Hyperboloid Paraboloid**: 
    $$\displaystyle \frac{x^2}{a^2} - \frac{y^2}{b^2} = z$$

### Vector Valued Functions

-   **Space Curve** - defined by parametric equations: $x = f(t), y = g(t), z = h(t)$, or $\vec{r}(t) = \langle f(t), g(t), h(t) \rangle$
    -   **Domain** - set intersection of all domains of components
    -   **Limit** - $\displaystyle \lim_{t \to a} \vec{r}(t) = \langle \lim_{t \to a} f(t), \lim_{t \to a} g(t), \lim_{t \to a} h(t) \rangle$ 
    -   **Continuity** - vector valued function $\vec{r}(t)$ is continuous at point $t = a$ if $\displaystyle \lim_{t \to a} \vec{r}(t)$ exists and $\displaystyle \lim_{t \to a} \vec{r}(t) = \vec{r}(a)$
        -   vector valued function $\vec{r}(t)$ is continuous over interval $I$ if it is continuous at each point $t= a \in I$
    - **Tangent Vector** - $\displaystyle \vec{r}'(t) = \lim_{\Delta t \to 0} \frac{\vec{r}(t + \Delta t) - \vec{r}(t)}{\Delta t}$
        -   derivative of $\vec{r}(t)$ with respect to $t$
        -   gives rate of change at point at $t$
        -   $\vec{r}(t)$ is differentiable on open interval $I$ if its components are differentiable on $I$, and its derivative on $I$ is $\vec{r}'(t) = \langle f'(t), g'(t), h'(t) \rangle$ 
    -   **Unit Tangent Vector** - unit tangent vector for value of $t$ on curve $\vec{r}(t)$ is $\displaystyle \vec{T}(t) = \frac{\vec{r}'(t)}{|\vec{r}'(t)|}$
    -   **Indefinite Integral** - with $\vec{r}(t) = \langle f(t), g(t), h(t) \rangle$, $\vec{R}(t) = \langle F(t), G(t), H(t) \rangle$  $\displaystyle \int \vec{r}(t) dt = R(t) + \vec{C}$, where $\vec{C}$ is an arbitrary vector with constant components
    -   **Definite Integral** - $\displaystyle \int_a^b \vec{r}(t) dt = \langle \int_a^b f(t) dt, \int_a^b g(t) dt, \int_a^b h(t) dt \rangle$ if $f$, $g$, $h$ are intergrable on $[a, b]$

### Derivative Rules

-   **Constant Rule**: 
$$
\frac{d}{dx} \vec{c} = \vec{0}
$$

-   **Sum Rule**: 
$$
\frac{d}{dx} \Big( \vec{u}(t) + \vec{v}(t) \Big) = \vec{u}'(t) + \vec{v}'(t)
$$

-   **Product Rule**: 
$$
\frac{d}{dx} \Big( f(t) \vec{u}(t) \Big) = f'(t)\vec{u}(t) + f(t)\vec{u}'(t)
$$

-   **Chain Rule**: 
$$
\frac{d}{dx} \vec{u}(f(t)) = \vec{u}'(f(t))f'(t)
$$

-   **Dot Product Rule**: 
$$
\frac{d}{dx} \Big( \vec{u}(t) \cdot \vec{v}(t) \Big) = \vec{u}'(t) \cdot \vec{v}(t) + \vec{u}(t) \cdot \vec{v}'(t)
$$

-   **Cross Product Rule**: 
$$
\frac{d}{dx} \Big( \vec{u}(t) \times \vec{v}(t) \Big) =\vec{u}'(t) \times \vec{v}(t) + \vec{u}(t) \times \vec{v}'(t)
$$


