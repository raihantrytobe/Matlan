# ADVANCED MATH 2026 (-DFA-)
## Function of Several Variables

---

### Slide 1 & 2: Title
* **Course:** ADVANCED MATH 2026 (-DFA-)
* **Topic:** Function of Several Variables

---

### Slide 3: I. Function of Several Variables

1. **Basics (Function of one variable)**
   $$f(x) = a$$
   Example: $y = 7x^2 \implies y = f(x)$

2. **Function of two variables**
   $$z = f(x,y)$$
   Example: $A = \frac{1}{2}g \cdot h \implies A = f(g,h)$

3. **Function of three variables**
   $$w = f(x,y,z)$$

> **Key Notes:**
> * Everything inside the bracket is **independent variable(s)**.
> * The restrictions of the independent variable(s) determine the **domain of $f$**.
> * That means if you are asked to provide the domain of function $f$, you need to look at the domain of each of the independent variables.

---

### Slide 4: Examples of Finding Domain

1. **Example:** Find the domain of $f(x,y) = \ln(xy)$
   * a. Draw in the Coordinate Plane!
   * b. Put the domain in writing!
   * c. Provide the domain in Math form!

2. **Another Example:** Find the domain of $f(x,y,z) = \frac{x}{\sqrt{9 - x^2 - y^2 - z^2}}$

---

### Slide 5: Solution to Example 1

**Problem:** Find the domain of $f(x,y) = \ln(xy)$

* **Condition:** For $\ln$ to work, $xy > 0$.
* **In Writing:** $D$: All ordered pairs of $(x \text{ and } y)$ in Quadrant I and Quadrant III, and not on the axes.
* **In Math Form:**
  $$D = \{(x,y) : xy > 0\}$$
* **Coordinate Plane Representation:** Areas shaded strictly inside Quadrant I ($x > 0, y > 0$) and Quadrant III ($x < 0, y < 0$), excluding the $x$-axis and $y$-axis.

---

### Slide 6: Solution to Example 2

**Problem:** Find the domain of $f(x,y,z) = \frac{x}{\sqrt{9 - x^2 - y^2 - z^2}}$

* **Condition:** The expression inside the square root in the denominator must be strictly greater than zero:
  $$9 - x^2 - y^2 - z^2 > 0 \implies x^2 + y^2 + z^2 < 9$$
* **In Math Form:**
  $$D = \{(x,y,z) : x^2 + y^2 + z^2 < 9\}$$
  *(Geometrically, this represents the interior of a sphere centered at the origin with radius $3$).*

---

### Slide 7 & 8: II. Explicit and Implicit Function

| Aspect | Explicit Function | Implicit Function |
| :--- | :--- | :--- |
| **1. Definition** | A function in which the output variable (dependent variable) can be explicitly written only in terms of the input variable (independent variable). | A function that cannot be written as one variable in terms of the other variable (or variables are mixed together). |
| **2. General Form** | $y = f(x)$ or $z = f(x,y)$ or $w = f(x,y,z)$, etc. | $f(x,y) = 0$ or $f(x,y,z) = 0$ or $f(x,y,z,w) = 0$ |
| **3. Examples** | $y = x^2 + 4x$ <br> $y = \frac{x^3 - 9}{x + 2}$ *(convertible from implicit)* | $xy + 2x - \sin(xy) + y^2 = 0$ <br> $x^3 - xy - 2y - 9 = 0$ <br> $x^3 - y(x + 2) - 9 = 0$ |

---

### Slide 9: Exercises — Explicit vs Implicit

**Identify the functions below as Explicit (E) or Implicit (I / I to E):**
* a. $y = \sqrt{x + 7}$
* b. $xy - y = 9$
* c. $\sin(xy) = x - 9$
* d. $\ln(xy) - \sin(y) + y - \cos(xy) = 9x - 8$
* e. $x + y + xy = 10$
* f. $\sin(x + y) = \frac{1}{2}$

---

### Slide 10: III. Derivative of Explicit Functions

Differentiation is done via straightforward, simple, and standard algebraic differentiation.

* **Example 1:** Find the derivative of $y = x^2 + \sin x - x + 4$
  $$\frac{dy}{dx} = 2x + \cos x - 1$$

* **Example 2:** Find the derivative of $y = \frac{1}{x^2 + 1}$
  $$\frac{dy}{dx} = \frac{(0)(x^2 + 1) - (1)(2x)}{(x^2 + 1)^2} = -\frac{2x}{(x^2 + 1)^2}$$

* **Exercises:** Find the derivative of:
  * a. $y = \sin(x^2)$
  * b. $f(x) = \frac{x^2 + 1}{x - 1}$
  * c. $f(x) = \arctan(2x)$

---

### Slide 11: IV. Derivative of Implicit Functions

Implicit differentiation is done in two steps:
1. Differentiate the entire expression $f(x,y) = 0$ with respect to only one variable (usually $x$), applying the chain rule to terms containing $y$.
2. Move/rearrange variables to isolate and find $\frac{dy}{dx}$.

**Example:** Find the derivative of $x^2 + xy + y = 0$ *(Note: This is an I to E function; solving explicitly first gives the same result)*
* **Step 1:**
  $$2x + (1)(y) + x\frac{dy}{dx} + \frac{dy}{dx} = 0$$
* **Step 2:**
  $$\frac{dy}{dx}(x + 1) = -(2x + y)$$
  $$\frac{dy}{dx} = -\frac{2x + y}{x + 1}$$

---

### Slide 12: Implicit Differentiation (Another Example)

**Example:** Find the derivative of $y = 5x^2 - 9e^y$
Rewrite as: $y + 9e^y = 5x^2$

* **Step 1:**
  $$\frac{dy}{dx} + 9e^y\frac{dy}{dx} = 10x$$
* **Step 2:**
  $$\frac{dy}{dx}(1 + 9e^y) = 10x$$
  $$\frac{dy}{dx} = \frac{10x}{1 + 9e^y}$$

---

### Slide 13: Exercises — Implicit Differentiation

**Find the derivative ($\frac{dy}{dx}$) of:**
* a. $x^4 + y^3 - 3x^2y = 0$
* b. $x^2 + y^2 = 1$
* c. $2x + 3y = 6$
* d. $\frac{x^2}{4} + \frac{y^2}{9} = 1$
* e. $xy = 1$
* f. $x^3 + y^3 - 3xy = 0$
* g. $e^x + y^2 = x^2 + 1$

---

### Slide 14: V. Partial and Total Derivative $\left(\frac{\partial f}{\partial x}\right)$ vs $\left(\frac{df}{dx}\right)$

Let $f(x,y)$ be a function of $x$ and $y$.

| Partial Derivative | Total Derivative |
| :--- | :--- |
| **a.** $y$ is independent of $x \implies f(x,y)$ | **a.** $y$ can depend on $x \implies f(x, y(x))$ |
| **b.** Notation: $\frac{\partial f}{\partial x}$ | **b.** Notation: $\frac{df}{dx}$ |
| **c. Example:** $f(x,y) = 3x^2 + 2y$ <br> $\frac{\partial f}{\partial x} = \frac{\partial}{\partial x}(3x^2) + \frac{\partial}{\partial x}(2y) = 6x$ | **c. Example:** $f(x,y) = 3x^2 + 2y$ <br> $\frac{df}{dx} = \frac{d}{dx}(3x^2) + \frac{d}{dx}(2y) = 6x + 2\frac{dy}{dx}$ |

---

### Slide 15: Exercises — Total Differential / Total Derivative

**Find the total derivative / total differential of:**
1. $z = f(x,y) = x^2y + \sin(y)$
   $$dz = \frac{\partial f}{\partial x}dx + \frac{\partial f}{\partial y}dy = 2xy\,dx + \{x^2 + \cos(y)\}dy$$
2. $y = f(x) = x^3 - 4x^2$
3. $z = f(x,y) = e^{xy} + \ln(x)$
4. $w = f(x,y,z) = x^2 + y^2 + z^2$

---

### Slide 16: VI. Higher-Order Partial Derivatives

If $f$ is a function of several variables, we can find higher-order partials.

**Definition:** If $f(x,y)$ is a function of two variables, then $\frac{\partial f}{\partial x}$ and $\frac{\partial f}{\partial y}$ are also functions of two variables and their partials can be taken again:
* $f_{xx} = \frac{\partial}{\partial x}\left(\frac{\partial f}{\partial x}\right) = \frac{\partial^2 f}{\partial x^2}$ : the derivative of $f$ taken twice with respect to $x$.
* $f_{yx} = \frac{\partial}{\partial x}\left(\frac{\partial f}{\partial y}\right) = \frac{\partial^2 f}{\partial x \partial y}$ : the derivative of $f$ with respect to $y$ and then with respect to $x$.
* $f_{xy} = \frac{\partial}{\partial y}\left(\frac{\partial f}{\partial x}\right) = \frac{\partial^2 f}{\partial y \partial x}$ : the derivative of $f$ with respect to $x$ and then with respect to $y$.
* $f_{yy} = \frac{\partial}{\partial y}\left(\frac{\partial f}{\partial y}\right) = \frac{\partial^2 f}{\partial y^2}$ : the derivative of $f$ taken twice with respect to $y$.

---

### Slide 17: Example — Higher-Order Partial Derivatives

**Example:** Find all partials up to the second order of the function:
$$f(x,y) = x^4y^2 - x^2y^6$$

**Solution:**
1. $f_x = \frac{\partial f}{\partial x} = 4x^3y^2 - 2xy^6$
2. $f_y = \frac{\partial f}{\partial y} = 2x^4y - 6x^2y^5$
3. $f_{xx} = \frac{\partial}{\partial x}\left(\frac{\partial f}{\partial x}\right) = \frac{\partial^2 f}{\partial x^2} = 12x^2y^2 - 2y^6$
4. $f_{yy} = \frac{\partial}{\partial y}\left(\frac{\partial f}{\partial y}\right) = \frac{\partial^2 f}{\partial y^2} = 2x^4 - 30x^2y^4$
5. $f_{xy} = \frac{\partial}{\partial y}\left(\frac{\partial f}{\partial x}\right) = \frac{\partial^2 f}{\partial y \partial x} = 8x^3y - 12xy^5$
6. $f_{yx} = \frac{\partial}{\partial x}\left(\frac{\partial f}{\partial y}\right) = \frac{\partial^2 f}{\partial x \partial y} = 8x^3y - 12xy^5$

---

### Slide 18: Exercises — Higher-Order Partial Derivatives

* **A.** Find all partials up to the second order of the function:
  $$f(x,y) = \cos(2x) - x^2e^{5y} + 3y^2$$
* **B.** Find $f_{xxyzz}$ for $f(x,y,z) = z^3y^2\ln(x)$
* **C.** Find $\frac{\partial^3 f}{\partial y \partial x^2}$ for $f(x,y) = e^{xy}$
* **D.** Find all partials up to the second order of $f(r,\theta) = 3r^2\cos(2\theta)$

---

### Slide 19: VII. Gradient & Partial Derivatives

Consider $f(x,y) = x^2\sin(y)$:
$$f_x = \frac{\partial f}{\partial x} = 2x\sin(y)$$
$$f_y = \frac{\partial f}{\partial y} = x^2\cos(y)$$

The **Gradient** puts all partial derivatives into a vector, denoted with the upside-down triangle ($\nabla$, called *del* or *nabla*), which means gradient of $f$:
$$\nabla f(x,y) = \begin{bmatrix} 2x\sin(y) \\ x^2\cos(y) \end{bmatrix} \quad \text{or} \quad \nabla f(x,y) = \begin{bmatrix} 2x\sin(y), & x^2\cos(y) \end{bmatrix}$$

In general, for more than 2 variables:
$$\nabla f = \begin{bmatrix} \frac{\partial f}{\partial x} \\ \frac{\partial f}{\partial y} \\ \vdots \end{bmatrix} = \begin{bmatrix} f_x \\ f_y \\ \vdots \end{bmatrix}$$

* **Formula for the gradient:**
  $$\nabla f(x,y) = f_x(x,y)\mathbf{i} + f_y(x,y)\mathbf{j}$$
* **Gradient at point $(a,b)$:**
  $$\nabla f(a,b) = f_x(a,b)\mathbf{i} + f_y(a,b)\mathbf{j}$$

---

### Slide 20 & 21: Examples — Gradient Vector

**Example 1:** Find the gradient of $f(x,y) = 3x^2 + 2y + 6$ at $(1, -1)$.
* $f_x(x,y) = \frac{\partial f}{\partial x} = 6x$ and $f_y(x,y) = \frac{\partial f}{\partial y} = 2$
* $\nabla f(x,y) = f_x(x,y)\mathbf{i} + f_y(x,y)\mathbf{j} = 6x\mathbf{i} + 2\mathbf{j}$
* At $(1, -1)$:
  $$\nabla f(1, -1) = 6\mathbf{i} + 2\mathbf{j} = (6, 2)$$

**Example 2:** Find the gradient of $f(x,y) = xe^y + x^2y$ at $(2, 0)$.
* $f_x(x,y) = \frac{\partial f}{\partial x} = e^y + 2xy$ and $f_y(x,y) = \frac{\partial f}{\partial y} = xe^y + x^2$
* $\nabla f(x,y) = (e^y + 2xy)\mathbf{i} + (xe^y + x^2)\mathbf{j}$
* At $(2, 0)$:
  $$\nabla f(2, 0) = (e^0 + 0)\mathbf{i} + (2e^0 + 4)\mathbf{j} = \mathbf{i} + 6\mathbf{j} = (1, 6)$$

---

### Slide 22: Exercises — Gradient Vector

**Find the gradient vector for these functions:**
1. $f(x,y) = x^3y + 3xy^2$ at $(2, -2)$
2. $f(x,y) = xe^{xy}$
3. $f(x,y) = x^2y\cos(y)$
4. $f(x,y,z) = xz\ln(x + y + z)$
5. $f(x,y) = \sin(3x)\cos(3y)$
   *(Solution shown on slide)*:
   * $f_x(x,y) = 3\cos(3x)\cos(3y)$
   * $f_y(x,y) = -3\sin(3x)\sin(3y)$
   * $\nabla f(x,y) = \big(3\cos(3x)\cos(3y)\big)\mathbf{i} - \big(3\sin(3x)\sin(3y)\big)\mathbf{j}$

---

### Slide 23: VIII. Tangent Line (Persamaan Garis Singgung)

The tangent line is one of the most important applications of differentiation. *(Visual illustrates a curve with a secant line passing through points $P$ and $Q$, approaching the tangent line at the point of tangency).*

**Example for one variable:**
Obtain the tangent line for $y = f(x) = x^3 - 5x^2 + 7$ at $(1, 3)$.
* $f_x(x) = \frac{df}{dx} = 3x^2 - 10x$
* $y - y_0 = f'(1)(x - x_0)$
* $y - 3 = (3 \cdot 1^2 - 10 \cdot 1)(x - 1)$
* $y - 3 = -7x + 7 \implies y = -7x + 10$
* Therefore, the tangent line is $y = -7x + 10$ or $7x + y - 10 = 0$.

---

### Slide 24: Tangent Line / Tangent Plane for Two Variables

**Example 1:** Obtain the tangent plane (linear approximation) for $z = f(x,y) = \ln(2x + y)$ at $(-1, 3)$.
* $z_0 = f(-1, 3) = \ln(-2 + 3) = \ln(1) = 0$
* $f_x(x,y) = \frac{2}{2x + y} \implies f_x(-1, 3) = 2$
* $f_y(x,y) = \frac{1}{2x + y} \implies f_y(-1, 3) = 1$
* Formula:
  $$z - z_0 = f_x(-1, 3)(x - x_0) + f_y(-1, 3)(y - y_0)$$
  $$z - 0 = 2(x + 1) + 1(y - 3)$$
  $$z = 2x + 2 + y - 3 = 2x + y - 1$$
* Therefore, the equation is $z = 2x + y - 1$ or $2x + y - z - 1 = 0$.

---

### Slide 25: Tangent Plane (Recall Previous Example)

**Example 2:** Recall $z = f(x,y) = xe^y + x^2y$ at $(2, 0)$, where $\nabla f(2, 0) = (1, 6)$ and $z_0 = f(2, 0) = 2$.

Obtain the tangent plane:
$$z - z_0 = \nabla f(2, 0) \cdot \begin{pmatrix} x - x_0 \\ y - y_0 \end{pmatrix}$$
$$z - 2 = \begin{pmatrix} 1 & 6 \end{pmatrix} \begin{pmatrix} x - 2 \\ y - 0 \end{pmatrix}$$
$$z - 2 = (x - 2) + 6y$$
$$z = x + 6y$$
Therefore, the equation at the given point is $z = x + 6y$ or $x + 6y - z = 0$.

---

### Slide 26: Exercises — Tangent Plane

**Obtain the tangent plane equation for:**
* **A.** $z = f(x,y) = 3 + \frac{x^2}{16} + \frac{y^2}{9}$ at $(-4, 3)$
* **B.** $z = f(x,y) = 2x^2 - xy^3$ at $(1, 2)$
* **C.** $z = f(x,y) = \ln(x^2 + y^2 + 1)$ at $(1, 2)$
* **D.** $z = f(x,y) = x^2 - y^2 + 3xy$ at $(1, 1)$

---

### Slide 27 & 28: IX. Application in Statistics — Multiple Linear Regression MLE

Suppose we have the linear model below:
$$y_i = \beta_0 + \beta_1 x_{1i} + \beta_2 x_{2i} + \varepsilon_i, \quad \text{where } \varepsilon_i \sim \mathcal{N}(0, \sigma^2)$$

The **likelihood function** for observing the data given the parameters $\beta_0, \beta_1, \beta_2$, and $\sigma^2$ is:
$$\mathcal{L}(\beta_0, \beta_1, \beta_2, \sigma^2 \mid y, x) = \prod_{i=1}^{n} \frac{1}{\sqrt{2\pi\sigma^2}} \exp\left\{ -\frac{(y_i - \beta_0 - \beta_1 x_{1i} - \beta_2 x_{2i})^2}{2\sigma^2} \right\}$$

**Notes:**
* $\prod_{i=1}^n$: Calculating the joint likelihood across all $n$ observations.
* $\frac{1}{\sqrt{2\pi\sigma^2}}$: Normalization constant for the Normal distribution, ensuring probabilities integrate to $1$.
* $\exp\{\dots\}$: The exponential part representing the likelihood of observing the actual outcome $y_i$ given the predicted value from the linear model.

The likelihood function can also be written as:
$$\mathcal{L}(\beta_0, \beta_1, \beta_2, \sigma^2 \mid y, x) = \frac{1}{(2\pi\sigma^2)^{n/2}} \exp\left\{ -\frac{1}{2\sigma^2} \sum_{i=1}^n (y_i - \beta_0 - \beta_1 x_{1i} - \beta_2 x_{2i})^2 \right\}$$
$$= (2\pi)^{-\frac{n}{2}} (\sigma^2)^{-\frac{n}{2}} e^{-\frac{1}{2\sigma^2} \sum_{i=1}^n (y_i - \beta_0 - \beta_1 x_{1i} - \beta_2 x_{2i})^2}$$

And the **log-likelihood** is given by:
$$L(\cdot) = \log \mathcal{L}(\cdot) = -\frac{n}{2}\log(2\pi) - \frac{n}{2}\log(\sigma^2) - \frac{1}{2\sigma^2}\sum_{i=1}^n (y_i - \beta_0 - \beta_1 x_{1i} - \beta_2 x_{2i})^2$$

**Task #1:** Find the gradient of the log-likelihood above:
$$\frac{\partial L}{\partial \beta_0} = \dots \quad \frac{\partial L}{\partial \beta_1} = \dots$$

---

### Slide 29, 30 & 31: Log-Likelihood Gradient & Hessian Matrix

$$\frac{\partial L}{\partial \beta_2} = \dots \quad \frac{\partial L}{\partial \sigma^2} = \dots$$

The gradient for the log-likelihood is:
$$\nabla L(\beta_0, \beta_1, \beta_2, \sigma^2) = \left( \frac{\partial L}{\partial \beta_0}, \frac{\partial L}{\partial \beta_1}, \frac{\partial L}{\partial \beta_2}, \frac{\partial L}{\partial \sigma^2} \right)$$

**Task #2:** Find the **Hessian Matrix** from the log-likelihood function.
The Hessian Matrix is constructed from the second-order partial derivatives:
$$H = \begin{bmatrix}
L_{\beta_0\beta_0} & L_{\beta_0\beta_1} & L_{\beta_0\beta_2} & L_{\beta_0\sigma^2} \\
L_{\beta_1\beta_0} & L_{\beta_1\beta_1} & L_{\beta_1\beta_2} & L_{\beta_1\sigma^2} \\
L_{\beta_2\beta_0} & L_{\beta_2\beta_1} & L_{\beta_2\beta_2} & L_{\beta_2\sigma^2} \\
L_{\sigma^2\beta_0} & L_{\sigma^2\beta_1} & L_{\sigma^2\beta_2} & L_{\sigma^2\sigma^2}
\end{bmatrix}$$
where, for example, $L_{\beta_2\beta_1} = \frac{\partial^2 L}{\partial \beta_1 \partial \beta_2}$.

Let the entries be denoted as:
* $A = \frac{\partial^2 L}{\partial \beta_0^2}$, $B = \frac{\partial^2 L}{\partial \beta_1^2}$, $C = \frac{\partial^2 L}{\partial \beta_2^2}$, $D = \frac{\partial^2 L}{\partial (\sigma^2)^2}$
* $E = \frac{\partial^2 L}{\partial \beta_1 \partial \beta_0}$, $F = \frac{\partial^2 L}{\partial \beta_2 \partial \beta_1}$, $G = \frac{\partial^2 L}{\partial \sigma^2 \partial \beta_2}$
* $H_{13} = \frac{\partial^2 L}{\partial \beta_2 \partial \beta_0}$, $I = \frac{\partial^2 L}{\partial \sigma^2 \partial \beta_1}$, $J = \frac{\partial^2 L}{\partial \sigma^2 \partial \beta_0}$

By symmetry of mixed partials ($L_{ij} = L_{ji}$):
$$H = \begin{bmatrix}
A & E & H_{13} & J \\
E & B & F & I \\
H_{13} & F & C & G \\
J & I & G & D
\end{bmatrix}$$

---

### Slide 32 & 33: X. Application in Statistics — Normal Distribution

**PDF of Normal Distribution** $X \sim \mathcal{N}(\mu, \sigma^2)$:
$$f(x \mid \mu, \sigma) = \frac{1}{\sqrt{2\pi}\sigma} \exp\left\{ -\frac{(x - \mu)^2}{2\sigma^2} \right\} = (2\pi)^{-\frac{1}{2}} \sigma^{-1} e^{-\frac{1}{2\sigma^2}(x - \mu)^2}$$

* **One-Sample Log-Likelihood:**
  $$\ell(\mu, \sigma) = \log\left\{ (2\pi)^{-\frac{1}{2}} \cdot \sigma^{-1} \cdot e^{-\frac{1}{2\sigma^2}(x - \mu)^2} \right\} = -\frac{1}{2}\log(2\pi) - \log\sigma - \frac{1}{2\sigma^2}(x - \mu)^2$$

* **$n$-Sample Likelihood & Log-Likelihood:**
  $$L(\mu, \sigma) = \left(\frac{1}{\sqrt{2\pi}\sigma}\right)^n \exp\left\{ -\sum_{i=1}^n \frac{(x_i - \mu)^2}{2\sigma^2} \right\}$$
  $$\ell(\mu, \sigma) = -\frac{n}{2}\log(2\pi) - n\log\sigma - \frac{1}{2\sigma^2}\sum_{i=1}^n (x_i - \mu)^2$$

**Exercises (One-Sample):**
1. Find the gradient from one-sample $\ell(\mu, \sigma)$:
   $$\nabla \ell(\cdot) = \begin{bmatrix} \frac{\partial \ell}{\partial \mu} \\ \frac{\partial \ell}{\partial \sigma} \end{bmatrix}$$
2. Find the Hessian from one-sample $\ell(\mu, \sigma)$:
   $$H\ell(\cdot) = \begin{bmatrix} A & B \\ B & C \end{bmatrix}, \quad \text{where } A = \frac{\partial^2 \ell}{\partial \mu^2}, \; B = \frac{\partial^2 \ell}{\partial \mu \partial \sigma}, \; C = \frac{\partial^2 \ell}{\partial \sigma^2}$$
3. Find the tangent plane when $\mu = 0$, $\sigma = 1$, and $x_0 = 2$.

---

### Slide 34: XI. Maxima & Minima

Recall from 1-dimensional calculus: to find the points of maxima and minima of a function, we first find the critical points where $f'(x) = 0$:
* (i) If $f''(x) > 0$, we have a **local minimum**.
* (ii) If $f''(x) < 0$, we have a **local maximum**.
* (iii) If $f''(x) = 0$, the test is **inconclusive**.

**Definition (Relative Extrema):**
A function $f(x,y)$ has a **relative minimum** (resp. **relative maximum**) at the point $(a, b)$ if $f(x,y) \ge f(a,b)$ (resp. $f(x,y) \le f(a,b)$) for all points $(x,y)$ in some open region around $(a, b)$.

**Definition (Critical Point):**
A point $(a,b)$ is a **critical point** of a function $f(x,y)$ if one of the following is true:
* (i) $f_x(a,b) = 0$ and $f_y(a,b) = 0$
* (ii) $f_x(a,b)$ and/or $f_y(a,b)$ does not exist.

---

### Slide 35: Classification of Critical Points (Second Derivative Test)

We need two quantities to classify the critical points of $f(x,y)$:
1. $f_{xx}$, the second partial derivative of $f$ with respect to $x$.
2. $H = f_{xx}f_{yy} - f_{xy}^2$, the determinant of the Hessian matrix.

If $H = 0$, then the critical point is **degenerate** (test is inconclusive). If $H \ne 0$, then the critical point is **non-degenerate** and we classify it as follows:
* **Case (i):** If $H > 0$ and $f_{xx} < 0$, then the critical point is a **relative maximum**.
* **Case (ii):** If $H > 0$ and $f_{xx} > 0$, then the critical point is a **relative minimum**.
* **Case (iii):** If $H < 0$, then the critical point is a **saddle point**.

---

### Slide 36 & 37: Example — Finding & Classifying Critical Points

**Example:** Find and classify the critical points of:
$$f(x,y) = 12x^3 + y^3 + 12x^2y - 75y$$

**Solution:**
1. **First-order partials:**
   $$f_x = 36x^2 + 24xy = 12x(3x + 2y)$$
   $$f_y = 3y^2 + 12x^2 - 75 = 3(4x^2 + y^2 - 25)$$

2. **Set $f_x = 0$ and $f_y = 0$:**
   From $12x(3x + 2y) = 0$, either $x = 0$ or $3x + 2y = 0$.
   * **Case (i) $x = 0$:**
     Substitute into $f_y = 0$: $3(y^2 - 25) = 0 \implies y = \pm 5$.
     Points: $(0, 5)$ and $(0, -5)$.
   * **Case (ii) $3x + 2y = 0 \implies y = -\frac{3}{2}x$:**
     Substitute into $f_y = 0$:
     $$3\left(4x^2 + \frac{9x^2}{4} - 25\right) = \frac{3}{4}(25x^2 - 100) = \frac{75}{4}(x^2 - 4) = 0 \implies x = \pm 2$$
     Points: $(2, -3)$ and $(-2, 3)$.

3. **Second-order partials & Hessian:**
   * $f_{xx} = 72x + 24y = 24(3x + y)$
   * $f_{xy} = 24x$
   * $f_{yy} = 6y$
   * $H = f_{xx}f_{yy} - f_{xy}^2 = 24(3x + y)(6y) - (24x)^2$

4. **Classification Summary Table:**

| Points | $f_{xx}$ | $H$ | Type |
| :--- | :---: | :---: | :--- |
| $(0, 5)$ | $120$ | $3600$ | **Relative Minimum** |
| $(0, -5)$ | $-120$ | $3600$ | **Relative Maximum** |
| $(2, -3)$ | $72$ | $-3600$ | **Saddle Point** |
| $(-2, 3)$ | $-72$ | $-3600$ | **Saddle Point** |

---

### Slide 38 & 39: Exercises & MLE vs OLS Concept

**Exercises: Find & classify the critical points**
1. $f(x,y) = x^3y + 3xy^2$
2. $f(x,y) = x^4 + 2y^4 - 4x^2y^2 + 6x^2 + 8y^2 - 10$

**Try This:**
3. Find the values of $\beta_0, \beta_1, \beta_2$, and $\sigma^2$ that maximize the log-likelihood function $L(\beta_0, \beta_1, \beta_2, \sigma^2)$.
4. **Advanced:** From problem #3, write $\hat{\beta}$ and $\hat{\sigma}^2$ as matrix/vector operations.

**Conceptual Note (Slide 39 — Scatterplot of Purchases vs Ads Seen):**
* **MLE (Maximum Likelihood Estimation):** Maximizing the log-likelihood function.
* **OLS (Ordinary Least Squares):** Minimizing the Sum of Squared Residuals:
  $$\min \sum_{i=1}^n (y_i - \hat{y}_i)^2 = \sum_{i=1}^n e_i^2, \quad \text{where } \hat{y}_i = \hat{\beta}_0 + \hat{\beta}_1 x_{1i}$$
* Under normality of errors, **MLE and OLS yield identical estimators** for $\beta$.

---

### Slide 40: XII. Lagrange Multiplier

Used for optimizing a function (finding maximum or minimum) subject to some equality constraints:
* Objective function: $f(x,y)$
* Constraint: $g(x,y) = 0$

**Condition:**
$$\nabla f = \lambda \nabla g \quad \text{and} \quad g(x,y) = 0$$
Using the Lagrangian function:
$$\mathcal{L}(x,y,\lambda) = f(x,y) - \lambda g(x,y) \quad (\text{or } f(x,y) + \lambda g(x,y))$$

**Quick Example:**
* $f(x,y) = xy + 1 \implies \nabla f = (y, x)$
* $g(x,y) = x^2 + y^2 - 1 = 0 \implies \nabla g = (2x, 2y)$
* System of equations:
  1. $y = 2\lambda x$
  2. $x = 2\lambda y$
  3. $x^2 + y^2 - 1 = 0$

---

### Slide 41 & 42: Worked Example — Lagrange Multiplier

**Example:** Find the optimum of $f(x,y) = xy$ subject to the constraint $g(x,y) = x^2 + y^2 - 25 = 0$.

**Solution:**
$$\nabla f = \begin{pmatrix} y \\ x \end{pmatrix}, \quad \nabla g = \begin{pmatrix} 2x \\ 2y \end{pmatrix}$$
Setting $\nabla f = \lambda \nabla g$ and $g = 0$:
* (i) $y = 2\lambda x$
* (ii) $x = 2\lambda y$
* (iii) $x^2 + y^2 = 25$

Substitute (i) into (ii):
$$x = 2\lambda(2\lambda x) = 4\lambda^2 x \implies 4\lambda^2 = 1 \implies \lambda = \pm \frac{1}{2}$$

* **Case 1: $\lambda = \frac{1}{2}$**
  * From (i): $y = 2\left(\frac{1}{2}\right)x \implies y = x$.
  * Substitute into (iii): $x^2 + x^2 = 25 \implies 2x^2 = 25 \implies x = \pm \frac{5}{\sqrt{2}}$.
  * Points: $\left(\frac{5}{\sqrt{2}}, \frac{5}{\sqrt{2}}\right)$ and $\left(-\frac{5}{\sqrt{2}}, -\frac{5}{\sqrt{2}}\right)$, giving $f(x,y) = \frac{25}{2}$.

* **Case 2: $\lambda = -\frac{1}{2}$**
  * From (i): $y = 2\left(-\frac{1}{2}\right)x \implies y = -x$.
  * Substitute into (iii): $x^2 + (-x)^2 = 25 \implies 2x^2 = 25 \implies x = \pm \frac{5}{\sqrt{2}}$.
  * Points: $\left(\frac{5}{\sqrt{2}}, -\frac{5}{\sqrt{2}}\right)$ and $\left(-\frac{5}{\sqrt{2}}, \frac{5}{\sqrt{2}}\right)$, giving $f(x,y) = -\frac{25}{2}$.

**Summary Table:**

| Critical Points | $f(x,y)$ | Classification |
| :--- | :---: | :--- |
| $\left(\frac{5}{\sqrt{2}}, \frac{5}{\sqrt{2}}\right)$ | $\frac{25}{2}$ | **Max** |
| $\left(-\frac{5}{\sqrt{2}}, -\frac{5}{\sqrt{2}}\right)$ | $\frac{25}{2}$ | **Max** |
| $\left(\frac{5}{\sqrt{2}}, -\frac{5}{\sqrt{2}}\right)$ | $-\frac{25}{2}$ | **Min** |
| $\left(-\frac{5}{\sqrt{2}}, \frac{5}{\sqrt{2}}\right)$ | $-\frac{25}{2}$ | **Min** |

---

### Slide 43: Exercises — Lagrange Multiplier

**Find the optimum of $f$ within the given constraint(s):**
1. $f(x,y) = 5x + 3y$ subject to $x^2 + y^2 = 136$
2. $f(x,y) = xy$ subject to $x + y = 16$
3. $f(x,y,z) = xz + yz$ subject to two constraints: $x^2 + z^2 = 2$ and $yz = 2$

---

### Slide 44 & 45: Statistics Application — Multinomial MLE

For multinomial observations $n = n_1 + n_2 + n_3$ with probabilities $p_1, p_2$, and $p_3$:
* **Likelihood function:**
  $$L(p_1, p_2, p_3) = p_1^{n_1} p_2^{n_2} p_3^{n_3}$$
* **Constraint:**
  $$p_1 + p_2 + p_3 = 1 \quad \text{--- (i)}$$
* **Log-likelihood:**
  $$\ell = n_1 \log p_1 + n_2 \log p_2 + n_3 \log p_3 \quad \text{--- (ii)}$$
* **Lagrange Function:**
  $$\mathcal{L}(p_1, p_2, p_3, \lambda) = n_1 \log p_1 + n_2 \log p_2 + n_3 \log p_3 + \lambda(1 - p_1 - p_2 - p_3)$$

Taking first-order derivatives:
$$\frac{\partial \mathcal{L}}{\partial p_i} = \frac{n_i}{p_i} - \lambda = 0 \implies p_i = \frac{n_i}{\lambda} \quad \text{--- (iii)}$$

Substitute (iii) into constraint (i):
$$\frac{n_1}{\lambda} + \frac{n_2}{\lambda} + \frac{n_3}{\lambda} = 1 \implies \lambda = n_1 + n_2 + n_3$$

Substitute $\lambda$ back into (iii):
$$\hat{p}_i = \frac{n_i}{n_1 + n_2 + n_3} \quad \text{is the MLE estimate for } p_i.$$

**Exercise (Slide 45):** Solve the same problem with an **additional constraint** $p_1 = 2p_2$:
* **Answers:**
  $$\lambda_1 = n, \quad \lambda_2 = n\left(1 - \frac{3n_1}{2(n_1 + n_2)}\right)$$
  $$p_1 = \frac{2(n_1 + n_2)}{3n}, \quad p_2 = \frac{n_1 + n_2}{3n}, \quad p_3 = \frac{n_3}{n}$$

---

### Slide 46 & 47: XIII. Series of Function of Several Variables

#### a. Taylor Series for One Variable
Let $f(x)$ be a function that is differentiable at $a$:
$$f(x) = f(a) + f'(a)(x - a) + \frac{f''(a)}{2!}(x - a)^2 + \frac{f^{(3)}(a)}{3!}(x - a)^3 + \cdots$$
When $a = 0$ (**Maclaurin Series**):
$$f(x) = f(0) + f'(0)x + \frac{f''(0)}{2!}x^2 + \frac{f^{(3)}(0)}{3!}x^3 + \cdots$$

#### b. Extending to Several Variables
Let $f(x_1, x_2, \dots, x_n)$ be differentiable at $\mathbf{a} = (a_1, a_2, \dots, a_n)$:
$$f(\mathbf{x}) = f(\mathbf{a}) + \nabla f(\mathbf{a}) \cdot (\mathbf{x} - \mathbf{a}) + \frac{1}{2!}(\mathbf{x} - \mathbf{a})^T H_f(\mathbf{a})(\mathbf{x} - \mathbf{a}) + \cdots$$
where:
* $\nabla f(\mathbf{a})$ is the **Gradient Vector** at $\mathbf{a}$.
* $H_f(\mathbf{a})$ is the **Hessian Matrix** at $\mathbf{a}$.

#### c. Expanded Version for Two Variables
Let $f(x,y)$ be differentiable at $(a, b)$:
$$\begin{aligned}
f(x,y) &= f(a,b) + (x - a)f_x(a,b) + (y - b)f_y(a,b) \\
&\quad + \frac{1}{2!}\left[(x - a)^2 f_{xx}(a,b) + 2(x - a)(y - b)f_{xy}(a,b) + (y - b)^2 f_{yy}(a,b)\right] + \text{higher-order terms.}
\end{aligned}$$

At $a = 0$ and $b = 0$:
$$f(x,y) = f(0,0) + x f_x(0,0) + y f_y(0,0) + \frac{1}{2!}\left(x^2 f_{xx}(0,0) + 2xy f_{xy}(0,0) + y^2 f_{yy}(0,0)\right) + \cdots$$

---

### Slide 48: Exercises — Taylor & Maclaurin Series

1. Find the Maclaurin Series for $f(x,y) = e^{x+y}$.
2. Find the Taylor series for $f(x,y) = x^2y + 3y$ and evaluate around the point $(1, 2)$.
3. Find the Taylor expansion for $f(x,y) = e^x \cos y$ and evaluate around $(0, 0)$.
4. Find the first-order Taylor expansion to linearize:
   $$f(x,y) = e^{\beta_0 + \beta_1 x + \beta_2 y} \quad \text{at } (x,y) = (0,0)$$

---

### Slide 49: Statistical Applications of Taylor / Maclaurin Series

1. **Delta Method:**
   Used to find the approximate asymptotic distribution of a function of an estimator $g(\hat{\theta})$ using a first-order Taylor expansion around $\theta$.
2. **Logistic Regression (Newton-Raphson / IRLS Optimization):**
   The log-likelihood function is a non-linear function:
   $$\ell(\beta) = \sum_{i=1}^n \left[ y_i \log(p_i) + (1 - y_i)\log(1 - p_i) \right], \quad \text{where } p_i = \frac{e^{\mathbf{x}_i^T \beta}}{1 + e^{\mathbf{x}_i^T \beta}}$$
   Approximated quadratically around $\beta^{(t)}$ via second-order Taylor expansion:
   $$\ell(\beta) \approx \ell(\beta^{(t)}) + (\beta - \beta^{(t)})^T \nabla \ell(\beta^{(t)}) + \frac{1}{2}(\beta - \beta^{(t)})^T H(\beta^{(t)})(\beta - \beta^{(t)})$$
3. **Likelihood Approximation:**
   Used when the log-likelihood function is too complicated (leading to derivations of the **Score Function** and **Fisher Information**).