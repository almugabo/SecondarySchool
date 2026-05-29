# S5.6 Mathematics Mock Exam - Semester 2 2026
## Solutions & Marking Scheme (Pedagogical Guide)

---

## Topic 1: Quadratics and the Parabola

### Question 1
Consider the quadratic function $y = 2x^2 - 12x + 10$.

#### Part a) Write in vertex form $y = a(x - p)^2 + q$.
**Step-by-step Solution:**
1. **Factor the leading coefficient ($a = 2$)** out of the terms containing $x$:
   $$y = 2(x^2 - 6x) + 10$$
2. **Complete the square** inside the parentheses. To do this, take the coefficient of $x$ (which is $-6$), divide it by 2 to get $-3$, and square it to get $9$. We add and subtract $9$ inside the parentheses to maintain equality:
   $$y = 2(x^2 - 6x + 9 - 9) + 10$$
3. **Rewrite the perfect square trinomial** $(x^2 - 6x + 9)$ as a squared binomial $(x - 3)^2$:
   $$y = 2\left[(x - 3)^2 - 9\right] + 10$$
4. **Distribute the 2** back and simplify the constant terms:
   $$y = 2(x - 3)^2 - 18 + 10$$
   $$y = 2(x - 3)^2 - 8$$

*   **Marking Rubric (3 Marks total):**
    *   **1 Mark**: Correctly factoring out $a = 2$.
    *   **1 Mark**: Correctly completing the square inside the brackets.
    *   **1 Mark**: Correct final vertex form $2(x-3)^2 - 8$.

---

#### Part b) State the vertex coordinates and the line of symmetry equation.
**Step-by-step Solution:**
1. The vertex form is $y = a(x - p)^2 + q$, where $(p, q)$ is the vertex.
   * Here, $p = 3$ and $q = -8$. So, the **vertex coordinates** are $(3, -8)$.
2. The **line of symmetry** is the vertical line passing through the vertex $x = p$.
   * Therefore, the equation of the line of symmetry is $x = 3$.

*   **Marking Rubric (2 Marks total):**
    *   **1 Mark**: Vertex coordinates $(3, -8)$ written correctly.
    *   **1 Mark**: Equation of line of symmetry written as $x = 3$ (must be an equation, not just the number 3).

---

#### Part c) Find the roots (zeros) of the parabola by solving $y = 0$.
**Step-by-step Solution:**
1. Set the vertex form equal to zero:
   $$2(x - 3)^2 - 8 = 0$$
2. Add $8$ to both sides and divide by $2$:
   $$2(x - 3)^2 = 8$$
   $$(x - 3)^2 = 4$$
3. Take the square root of both sides, remembering both positive and negative roots:
   $$x - 3 = \pm \sqrt{4}$$
   $$x - 3 = \pm 2$$
4. Solve for $x$:
   * **Case 1:** $x - 3 = 2 \implies x = 5$
   * **Case 2:** $x - 3 = -2 \implies x = 1$
   * The roots are $x = 1$ and $x = 5$.

*   **Marking Rubric (2 Marks total):**
    *   **1 Mark**: Setting up the equation and isolating $(x-3)^2 = 4$.
    *   **1 Mark**: Finding both correct roots ($x=1$ and $x=5$).

---

### Question 2
Solve the quadratic inequality $x^2 - 5x - 6 < 0$.

**Step-by-step Solution:**
1. **Factor the quadratic expression** to find the critical boundary points:
   $$(x - 6)(x + 1) < 0$$
2. **Identify critical points** where the expression equals zero:
   $$x = 6 \quad \text{and} \quad x = -1$$
3. **Analyze the intervals** created by these points ($x < -1$, $-1 < x < 6$, and $x > 6$):
   * Since the quadratic graph $y = x^2 - 5x - 6$ is a parabola opening upwards (coefficient of $x^2$ is positive), the graph lies below the x-axis ($y < 0$) *between* the roots.
   * Alternatively, we can use test values:
     * For $x = -2$ (Interval $x < -1$): $(-2 - 6)(-2 + 1) = (-8)(-1) = 8 > 0$ (does not satisfy inequality).
     * For $x = 0$ (Interval $-1 < x < 6$): $(0 - 6)(0 + 1) = -6 < 0$ (satisfies inequality).
     * For $x = 7$ (Interval $x > 6$): $(7 - 6)(7 + 1) = 8 > 0$ (does not satisfy inequality).
4. **State the solution**:
   * The inequality is satisfied for values of $x$ strictly between $-1$ and $6$.
   * In interval notation, the solution is: **$(-1, 6)$**.

*   **Marking Rubric (4 Marks total):**
    *   **1 Mark**: Correct factorization $(x-6)(x+1)$.
    *   **1 Mark**: Correctly identifying boundary values $x = -1$ and $x = 6$.
    *   **1 Mark**: Logical testing of intervals (algebraic tests or graphical reasoning).
    *   **1 Mark**: Correct solution written in interval notation $(-1, 6)$ or inequality form $-1 < x < 6$.

\pagebreak

## Topic 2: Log Equations

### Question 3
Solve the logarithmic equation: $\log_2(x) + \log_2(x - 2) = 3$.

**Step-by-step Solution:**
1. **Apply the product rule of logarithms** ($\log_b(A) + \log_b(B) = \log_b(A \cdot B)$):
   $$\log_2\left[x(x - 2)\right] = 3$$
2. **Convert the logarithmic equation to exponential form** ($y = \log_b(x) \iff b^y = x$):
   $$x(x - 2) = 2^3$$
   $$x^2 - 2x = 8$$
3. **Rearrange into standard quadratic form** ($ax^2 + bx + c = 0$):
   $$x^2 - 2x - 8 = 0$$
4. **Factor the quadratic equation**:
   $$(x - 4)(x + 2) = 0$$
   * Giving potential solutions: $x = 4$ and $x = -2$.
5. **Check for extraneous solutions** (the argument of a logarithm must be strictly positive):
   * For $x = 4$:
     * $\log_2(4)$ is valid (argument $4 > 0$).
     * $\log_2(4-2) = \log_2(2)$ is valid (argument $2 > 0$).
   * For $x = -2$:
     * $\log_2(-2)$ is invalid (argument $-2 \le 0$). Thus, $x = -2$ is extraneous.
   * The only valid solution is **$x = 4$**.

*   **Marking Rubric (4 Marks total):**
    *   **1 Mark**: Correctly combining logs into $\log_2(x(x-2))$.
    *   **1 Mark**: Converting to exponential form $x^2 - 2x = 8$.
    *   **1 Mark**: Solving the quadratic equation to get $x = 4$ and $x = -2$.
    *   **1 Mark**: Explicitly rejecting $x = -2$ due to domain constraints and stating final answer $x = 4$.

---

### Question 4
Using the laws of logarithms, solve: $2\log_3(x) - \log_3(x + 6) = 1$.

**Step-by-step Solution:**
1. **Apply the power rule** to the first term ($k\log_b(A) = \log_b(A^k)$):
   $$\log_3(x^2) - \log_3(x + 6) = 1$$
2. **Apply the quotient rule** ($\log_b(A) - \log_b(B) = \log_b(\frac{A}{B})$):
   $$\log_3\left(\frac{x^2}{x + 6}\right) = 1$$
3. **Convert to exponential form**:
   $$\frac{x^2}{x + 6} = 3^1$$
   $$\frac{x^2}{x + 6} = 3$$
4. **Solve the resulting equation**:
   $$x^2 = 3(x + 6)$$
   $$x^2 = 3x + 18$$
   $$x^2 - 3x - 18 = 0$$
5. **Factor the quadratic**:
   $$(x - 6)(x + 3) = 0$$
   * Giving potential solutions: $x = 6$ and $x = -3$.
6. **Check domain constraints**:
   * For $x = 6$: Both $\log_3(6)$ and $\log_3(12)$ are defined (valid).
   * For $x = -3$: $\log_3(-3)$ is undefined (invalid).
   * Therefore, the only valid solution is **$x = 6$**.

*   **Marking Rubric (4 Marks total):**
    *   **1 Mark**: Applying the power rule to write $\log_3(x^2)$.
    *   **1 Mark**: Applying the quotient rule to obtain $\log_3(\frac{x^2}{x+6}) = 1$.
    *   **1 Mark**: Converting to a quadratic equation $x^2 - 3x - 18 = 0$ and finding $x = 6$ and $x = -3$.
    *   **1 Mark**: Rejecting the extraneous root $x = -3$ and stating final solution $x = 6$.

\pagebreak

## Topic 3: Trigonometry

### Question 5
Triangle $PAB$ with $P = 65^\circ$, $PA = 8\text{ m}$, and $PB = 12\text{ m}$.

#### Part a) Calculate the distance from $A$ to $B$ (to 3 s.f.).
**Step-by-step Solution:**
1. Since we know two sides and the included angle (SAS), we use the **Cosine Rule**:
   $$c^2 = a^2 + b^2 - 2ab\cos(C)$$
   Let $c = AB$, $a = 12\text{ m}$ (side opposite $A$), $b = 8\text{ m}$ (side opposite $B$), and $C = 65^\circ$.
2. Substitute the values:
   $$AB^2 = 12^2 + 8^2 - 2(12)(8)\cos(65^\circ)$$
   $$AB^2 = 144 + 64 - 192\cos(65^\circ)$$
   $$AB^2 = 208 - 192(0.422618)$$
   $$AB^2 \approx 208 - 81.1427$$
   $$AB^2 \approx 126.8573$$
3. Take the square root:
   $$AB = \sqrt{126.8573} \approx 11.263\text{ m}$$
4. Round to 3 significant figures: **$AB \approx 11.3\text{ m}$**.

*   **Marking Rubric (3 Marks total):**
    *   **1 Mark**: Selecting and stating the correct Cosine Rule formula.
    *   **1 Mark**: Correct substitution of values into the formula.
    *   **1 Mark**: Correct calculation and rounding to $11.3\text{ m}$ (with units).

---

#### Part b) Find the area of the triangular piece of land $PAB$ (to 1 d.p.).
**Step-by-step Solution:**
1. Use the **sine area formula** ($\text{Area} = \frac{1}{2}ab\sin(C)$):
   $$\text{Area} = \frac{1}{2} \cdot PB \cdot PA \cdot \sin(65^\circ)$$
2. Substitute the values:
   $$\text{Area} = \frac{1}{2} \cdot 12 \cdot 8 \cdot \sin(65^\circ)$$
   $$\text{Area} = 48 \cdot \sin(65^\circ)$$
   $$\text{Area} \approx 48 \cdot 0.906308$$
   $$\text{Area} \approx 43.5028\text{ m}^2$$
3. Round to 1 decimal place: **$\text{Area} \approx 43.5\text{ m}^2$**.

*   **Marking Rubric (2 Marks total):**
    *   **1 Mark**: Stating the correct area formula and substituting values.
    *   **1 Mark**: Correct calculations and rounding to $43.5\text{ m}^2$ (with units).

---

### Question 6
#### Part a) Solve $2\sin(2x - \frac{\pi}{3}) = \sqrt{3}$ for $0 \le x \le \pi$.
**Step-by-step Solution:**
1. **Isolate the trigonometric term**:
   $$\sin\left(2x - \frac{\pi}{3}\right) = \frac{\sqrt{3}}{2}$$
2. **Find the range for the compound angle** $u = 2x - \frac{\pi}{3}$:
   Since $0 \le x \le \pi \implies 0 \le 2x \le 2\pi$, subtracting $\frac{\pi}{3}$ gives:
   $$-\frac{\pi}{3} \le u \le \frac{5\pi}{3}$$
3. **Find principal values** of $u$ in this range where $\sin(u) = \frac{\sqrt{3}}{2}$:
   * In Quadrant I: $u = \frac{\pi}{3}$
   * In Quadrant II: $u = \pi - \frac{\pi}{3} = \frac{2\pi}{3}$
4. **Solve for $x$ in each case**:
   * **Case 1:** $2x - \frac{\pi}{3} = \frac{\pi}{3} \implies 2x = \frac{2\pi}{3} \implies x = \frac{\pi}{3}$
   * **Case 2:** $2x - \frac{\pi}{3} = \frac{2\pi}{3} \implies 2x = \pi \implies x = \frac{\pi}{2}$
   * Both solutions lie in the interval $[0, \pi]$.
   * Solutions: **$x = \frac{\pi}{3}, \frac{\pi}{2}$**.

*   **Marking Rubric (3 Marks total):**
    *   **1 Mark**: Isolating the sine term to obtain $\sin(2x - \frac{\pi}{3}) = \frac{\sqrt{3}}{2}$.
    *   **1 Mark**: Determining the two angles for the compound angle ($\frac{\pi}{3}$ and $\frac{2\pi}{3}$).
    *   **1 Mark**: Finding both correct values for $x$ within the interval.

---

#### Part b) Solve $2\cos^2(x) - \sin(x) - 1 = 0$ for $0 \le x \le 2\pi$.
**Step-by-step Solution:**
1. **Use the Pythagorean Identity** $\cos^2(x) = 1 - \sin^2(x)$ to convert the equation to a quadratic in terms of $\sin(x)$:
   $$2(1 - \sin^2(x)) - \sin(x) - 1 = 0$$
   $$2 - 2\sin^2(x) - \sin(x) - 1 = 0$$
   $$-2\sin^2(x) - \sin(x) + 1 = 0$$
2. **Multiply by $-1$** to get standard form:
   $$2\sin^2(x) + \sin(x) - 1 = 0$$
3. **Factor the quadratic expression** (let $s = \sin(x)$ so $2s^2 + s - 1 = 0$):
   $$(2\sin(x) - 1)(\sin(x) + 1) = 0$$
4. **Solve the separate equations**:
   * **Equation 1:** $2\sin(x) - 1 = 0 \implies \sin(x) = \frac{1}{2}$
     * In the interval $0 \le x \le 2\pi$: $x = \frac{\pi}{6}$ and $x = \frac{5\pi}{6}$.
   * **Equation 2:** $\sin(x) + 1 = 0 \implies \sin(x) = -1$
     * In the interval $0 \le x \le 2\pi$: $x = \frac{3\pi}{2}$.
5. Solutions: **$x = \frac{\pi}{6}, \frac{5\pi}{6}, \frac{3\pi}{2}$**.

*   **Marking Rubric (4 Marks total):**
    *   **1 Mark**: Using the identity to convert the equation to terms of $\sin(x)$.
    *   **1 Mark**: Correctly factoring the quadratic equation into $(2\sin(x)-1)(\sin(x)+1)=0$.
    *   **1 Mark**: Solving $\sin(x) = \frac{1}{2}$ to get $x = \frac{\pi}{6}, \frac{5\pi}{6}$.
    *   **1 Mark**: Solving $\sin(x) = -1$ to get $x = \frac{3\pi}{2}$.

\pagebreak

## Topic 4: Probability

### Question 7
Total students $N = 50$, Math ($M$) = 30, Physics ($P$) = 25, Both ($M \cap P$) = 10.

#### Part a) Construct a Venn diagram.
**Step-by-step Solution:**
1. Start with the intersection: $M \cap P = 10$.
2. Calculate the number of students who study *only* Mathematics:
   $$\text{Only Math} = N(M) - N(M \cap P) = 30 - 10 = 20$$
3. Calculate the number of students who study *only* Physics:
   $$\text{Only Physics} = N(P) - N(M \cap P) = 25 - 10 = 15$$
4. Calculate the number of students who study *neither*:
   $$\text{Neither} = 50 - (\text{Only Math} + \text{Intersection} + \text{Only Physics}) = 50 - (20 + 10 + 15) = 5$$
5. Draw two overlapping circles labeled $M$ and $P$ inside a rectangular box $U$:
   * $M$ circle (exclusive area): 20
   * Overlap area: 10
   * $P$ circle (exclusive area): 15
   * Box area (outside circles): 5

*   **Marking Rubric (3 Marks total):**
    *   **1 Mark**: Putting 10 in the intersection.
    *   **1 Mark**: Calculating and placing 20 and 15 in the respective outer circles.
    *   **1 Mark**: Placing 5 in the bounding box outside the circles.

---

#### Part b) Find the probability they study Mathematics, given they study Physics.
**Step-by-step Solution:**
1. Use the **conditional probability formula** ($P(A|B) = \frac{P(A \cap B)}{P(B)}$):
   $$P(M|P) = \frac{N(M \cap P)}{N(P)}$$
2. Substitute the values:
   $$P(M|P) = \frac{10}{25} = \frac{2}{5} = 0.4$$

*   **Marking Rubric (2 Marks total):**
    *   **1 Mark**: Showing correct probability definition/fraction $\frac{10}{25}$.
    *   **1 Mark**: Stating the correct final answer ($0.4$ or $\frac{2}{5}$).

---

#### Part c) Find the probability they do not study Mathematics, given they study Physics.
**Step-by-step Solution:**
1. The probability of the complement event under the same condition is:
   $$P(M'|P) = 1 - P(M|P) = 1 - 0.4 = 0.6$$
2. Alternatively, read directly from the Venn diagram:
   $$P(M'|P) = \frac{\text{Only Physics}}{P} = \frac{15}{25} = \frac{3}{5} = 0.6$$

*   **Marking Rubric (2 Marks total):**
    *   **1 Mark**: Stating relationship $1 - P(M|P)$ or fraction $\frac{15}{25}$.
    *   **1 Mark**: Finding the final correct value ($0.6$ or $\frac{3}{5}$).

---

### Question 8
Box with 5 red, 3 green balls. Two draws without replacement.

#### Part a) Draw a tree diagram.
**Step-by-step Solution:**
1. **First Draw** (8 balls in total):
   * Branch 1: Red ($R_1$) with probability $\frac{5}{8}$
   * Branch 2: Green ($G_1$) with probability $\frac{3}{8}$
2. **Second Draw** (7 balls remaining):
   * If first was Red ($R_1$, leaves 4 Red, 3 Green):
     * Branch 1a: Red ($R_2$) with probability $\frac{4}{7}$
     * Branch 1b: Green ($G_2$) with probability $\frac{3}{7}$
   * If first was Green ($G_1$, leaves 5 Red, 2 Green):
     * Branch 2a: Red ($R_2$) with probability $\frac{5}{7}$
     * Branch 2b: Green ($G_2$) with probability $\frac{2}{7}$

*   **Marking Rubric (3 Marks total):**
    *   **1 Mark**: Correct structure (two branches splitting into two).
    *   **1 Mark**: Correct probabilities for the first draw branches.
    *   **1 Mark**: Correct conditional probabilities for the second draw branches.

---

#### Part b) Calculate the probability that the two balls drawn are of different colors.
**Step-by-step Solution:**
1. The outcome "different colors" corresponds to two mutually exclusive paths:
   * **Path 1:** Red then Green ($R_1 \cap G_2$)
     $$P(R_1 \cap G_2) = \frac{5}{8} \times \frac{3}{7} = \frac{15}{56}$$
   * **Path 2:** Green then Red ($G_1 \cap R_2$)
     $$P(G_1 \cap R_2) = \frac{3}{8} \times \frac{5}{7} = \frac{15}{56}$$
2. Add the probabilities of the two paths:
   $$P(\text{Different Colors}) = P(R_1 \cap G_2) + P(G_1 \cap R_2)$$
   $$P(\text{Different Colors}) = \frac{15}{56} + \frac{15}{56} = \frac{30}{56} = \frac{15}{28} \approx 0.536$$

*   **Marking Rubric (3 Marks total):**
    *   **1 Mark**: Correct calculations for $P(RG) = \frac{15}{56}$.
    *   **1 Mark**: Correct calculations for $P(GR) = \frac{15}{56}$.
    *   **1 Mark**: Summing the paths to get the correct final answer $\frac{15}{28}$ (or $\approx 0.536$).

\pagebreak

## Topic 5: Vectors in 2D

### Question 9
$\vec{u} = \begin{pmatrix} 4 \\ -3 \end{pmatrix}, \vec{v} = \begin{pmatrix} -2 \\ 5 \end{pmatrix}$.

#### Part a) Calculate the resultant vector $\vec{w} = 3\vec{u} + 2\vec{v}$.
**Step-by-step Solution:**
1. Perform scalar multiplication on each vector:
   $$3\vec{u} = 3\begin{pmatrix} 4 \\ -3 \end{pmatrix} = \begin{pmatrix} 12 \\ -9 \end{pmatrix}$$
   $$2\vec{v} = 2\begin{pmatrix} -2 \\ 5 \end{pmatrix} = \begin{pmatrix} -4 \\ 10 \end{pmatrix}$$
2. Add the component values:
   $$\vec{w} = \begin{pmatrix} 12 \\ -9 \end{pmatrix} + \begin{pmatrix} -4 \\ 10 \end{pmatrix} = \begin{pmatrix} 12 + (-4) \\ -9 + 10 \end{pmatrix} = \begin{pmatrix} 8 \\ 1 \end{pmatrix}$$

*   **Marking Rubric (2 Marks total):**
    *   **1 Mark**: Showing correct scalar multiplication.
    *   **1 Mark**: Correct addition to find $\vec{w} = \begin{pmatrix} 8 \\ 1 \end{pmatrix}$.

---

#### Part b) Calculate the magnitude of vector $\vec{u}$ and vector $\vec{w}$.
**Step-by-step Solution:**
1. The magnitude of a vector $\vec{a} = \begin{pmatrix} x \\ y \end{pmatrix}$ is given by $|\vec{a}| = \sqrt{x^2 + y^2}$.
2. Calculate $|\vec{u}|$:
   $$|\vec{u}| = \sqrt{4^2 + (-3)^2} = \sqrt{16 + 9} = \sqrt{25} = 5$$
3. Calculate $|\vec{w}|$:
   $$|\vec{w}| = \sqrt{8^2 + 1^2} = \sqrt{64 + 1} = \sqrt{65} \approx 8.06$$

*   **Marking Rubric (3 Marks total):**
    *   **1 Mark**: Stating the correct formula for magnitude (Pythagoras).
    *   **1 Mark**: Finding $|\vec{u}| = 5$.
    *   **1 Mark**: Finding $|\vec{w}| = \sqrt{65} \approx 8.06$.

---

### Question 10
Vectors $\vec{a} = 3\vec{i} + 4\vec{j}$ and $\vec{b} = 12\vec{i} - 5\vec{j}$.

#### Part a) Calculate the scalar product (dot product) $\vec{a} \cdot \vec{b}$.
**Step-by-step Solution:**
1. Use components multiplication formula $\vec{a} \cdot \vec{b} = a_x b_x + a_y b_y$:
   $$\vec{a} \cdot \vec{b} = (3)(12) + (4)(-5)$$
   $$\vec{a} \cdot \vec{b} = 36 - 20 = 16$$

*   **Marking Rubric (2 Marks total):**
    *   **1 Mark**: Showing step $(3)(12) + (4)(-5)$.
    *   **1 Mark**: Correct final scalar product value ($16$).

---

#### Part b) Find the angle $\theta$ between vectors $\vec{a}$ and $\vec{b}$ (to nearest degree).
**Step-by-step Solution:**
1. Use the geometric definition of the scalar product:
   $$\vec{a} \cdot \vec{b} = |\vec{a}||\vec{b}|\cos(\theta) \implies \cos(\theta) = \frac{\vec{a} \cdot \vec{b}}{|\vec{a}||\vec{b}|}$$
2. Calculate the magnitudes of vectors $\vec{a}$ and $\vec{b}$:
   $$|\vec{a}| = \sqrt{3^2 + 4^2} = \sqrt{25} = 5$$
   $$|\vec{b}| = \sqrt{12^2 + (-5)^2} = \sqrt{169} = 13$$
3. Substitute into the cosine formula:
   $$\cos(\theta) = \frac{16}{5 \times 13} = \frac{16}{65} \approx 0.24615$$
4. Take the inverse cosine:
   $$\theta = \arccos(0.24615) \approx 75.75^\circ$$
5. Round to the nearest degree: **$\theta \approx 76^\circ$**.

*   **Marking Rubric (3 Marks total):**
    *   **1 Mark**: Finding magnitudes $|\vec{a}| = 5$ and $|\vec{b}| = 13$.
    *   **1 Mark**: Substituting values into equation to find $\cos(\theta) = \frac{16}{65}$.
    *   **1 Mark**: Correct inverse calculation and rounding to $76^\circ$.

\pagebreak

## Topic 6: 3D Shapes

### Question 11
Cuboid with $AB = 3\text{ cm}$, $BC = 4\text{ cm}$, and height $CG = 12\text{ cm}$.

#### Part a) Calculate the length of the base diagonal, $AC$.
**Step-by-step Solution:**
1. The base of the cuboid is a rectangle $ABCD$ with sides $AB = 3\text{ cm}$ and $BC = 4\text{ cm}$. The diagonal $AC$ forms a right-angled triangle $ABC$.
2. Apply Pythagoras theorem in 2D:
   $$AC = \sqrt{AB^2 + BC^2}$$
   $$AC = \sqrt{3^2 + 4^2} = \sqrt{9 + 16} = \sqrt{25} = 5\text{ cm}$$

*   **Marking Rubric (2 Marks total):**
    *   **1 Mark**: Setting up the Pythagorean relationship $AC^2 = 3^2 + 4^2$.
    *   **1 Mark**: Correct calculation to get $5\text{ cm}$ (with units).

---

#### Part b) Calculate the length of the space diagonal of the cuboid, $AG$.
**Step-by-step Solution:**
1. The space diagonal $AG$ forms a right-angled triangle $ACG$ where $AC = 5\text{ cm}$ (base diagonal) and $CG = 12\text{ cm}$ (vertical height).
2. Apply Pythagoras theorem:
   $$AG = \sqrt{AC^2 + CG^2}$$
   $$AG = \sqrt{5^2 + 12^2} = \sqrt{25 + 144} = \sqrt{169} = 13\text{ cm}$$
   *(Note: Alternatively, we can use the direct 3D Pythagoras formula $AG = \sqrt{x^2 + y^2 + z^2} = \sqrt{3^2 + 4^2 + 12^2} = 13\text{ cm}$).*

*   **Marking Rubric (2 Marks total):**
    *   **1 Mark**: Setting up the Pythagorean equation with either 2D intermediate or direct 3D variables.
    *   **1 Mark**: Correct calculation to get $13\text{ cm}$ (with units).

---

### Question 12
#### Part a) Cylinder total surface area ($r = 3\text{ cm}$, $h = 8\text{ cm}$) in terms of $\pi$.
**Step-by-step Solution:**
1. State the formula for the **total surface area of a closed cylinder**:
   $$\text{Area} = 2\pi r^2 + 2\pi rh$$
   *   $2\pi r^2$ represents the area of the top and bottom circular bases.
   *   $2\pi rh$ represents the curved surface area (circumference multiplied by height).
2. Substitute the given values $r = 3\text{ cm}$ and $h = 8\text{ cm}$:
   $$\text{Area} = 2\pi(3)^2 + 2\pi(3)(8)$$
   $$\text{Area} = 2\pi(9) + 2\pi(24)$$
   $$\text{Area} = 18\pi + 48\pi$$
3. Combine terms (leaving in terms of $\pi$ as requested):
   $$\text{Area} = 66\pi\text{ cm}^2$$

*   **Marking Rubric (3 Marks total):**
    *   **1 Mark**: Stating the correct formula for total surface area.
    *   **1 Mark**: Correct substitution of values.
    *   **1 Mark**: Correct simplification to $66\pi\text{ cm}^2$ (with units).

---

#### Part b) Volume of a right pyramid (square base side $6\text{ cm}$, vertical height $10\text{ cm}$).
**Step-by-step Solution:**
1. State the formula for the **volume of a pyramid**:
   $$\text{Volume} = \frac{1}{3} \times \text{Base Area} \times \text{Height}$$
2. Calculate the base area of the square base ($s = 6\text{ cm}$):
   $$\text{Base Area} = s^2 = 6^2 = 36\text{ cm}^2$$
3. Substitute the base area and vertical height ($h = 10\text{ cm}$) into the volume formula:
   $$\text{Volume} = \frac{1}{3} \times 36 \times 10$$
   $$\text{Volume} = 12 \times 10 = 120\text{ cm}^3$$

*   **Marking Rubric (2 Marks total):**
    *   **1 Mark**: Calculating correct base area ($36\text{ cm}^2$) and stating the volume formula.
    *   **1 Mark**: Correct final volume calculation of $120\text{ cm}^3$ (with units).
