# Quadratic Equations and Their Graphs

## 1. From Lines to Curves: Introduction to Quadratics

Do you remember **linear equations**? They follow the form \(y = mx + c\) and always produce a **straight line** when graphed. The number \(m\) represents the slope (how steep the line is), and \(c\) is the y-intercept (where the line crosses the y-axis).

Now, what happens if we take this a step further and add a more powerful term to our equation — an \(x^2\) term?

That gives us a **quadratic equation**, which is generally written as:

\[
ax^2 + bx + c = 0
\]

Here:
- \(a\) determines how wide or narrow the curve is, and whether it opens upward or downward.
- \(b\) affects the position of the vertex (the turning point).
- \(c\) is the y-intercept — where the curve crosses the y-axis.

Unlike a straight line, a quadratic equation produces a **U-shaped curve** called a **parabola**. If \(a > 0\), the parabola opens upward; if \(a < 0\), it opens downward.

Quadratic equations appear in many real-world contexts: the path of a thrown ball, the shape of a satellite dish, or the profit of a business depending on price changes. The main goal when solving a quadratic is usually to find its **roots** — the x-values where it crosses the x-axis.

---

## 2. Solving Quadratic Equations

There are three main methods for solving quadratic equations: **factoring**, **completing the square**, and the **quadratic formula**.

### 2.1 Solving by Factoring

This is often the quickest method when the quadratic can be neatly factored.

**Key Idea:** If \(A \times B = 0\), then either \(A = 0\) or \(B = 0\). This is called the **Zero Product Property**.

**Example:** Solve \(x^2 + 5x + 6 = 0\).

1. **Find two numbers** that multiply to \(6\) (the constant term) and add to \(5\) (the coefficient of \(x\)).  
   → The numbers are **2** and **3**.
2. **Write as a product:**  
   \((x + 2)(x + 3) = 0\)
3. **Apply the Zero Product Property:**  
   \(x + 2 = 0\) or \(x + 3 = 0\)

✅ **Solutions:** \(x = -2\) and \(x = -3\).

This method works best when coefficients are integers and the quadratic is easily factorable.

---

### 2.2 Solving by Completing the Square

When factoring is difficult or impossible with integers, completing the square is a powerful alternative. It transforms the quadratic into a **perfect square trinomial**.

#### Reminder: Special Algebraic Identities
- \((a+b)^2 = a^2 + 2ab + b^2\)
- \((a-b)^2 = a^2 - 2ab + b^2\)
- \((a+b)(a-b) = a^2 - b^2\)

#### The Goal
To rewrite an expression like \(x^2 + bx\) into a form like \((x + p)^2\) by adding a specific number that completes the square.

#### Worked Example 1
Solve: \(x^2 + 6x - 16 = 0\)

1. Move the constant to the right: \(x^2 + 6x = 16\)  
2. Take half of 6 (→ 3), square it (→ 9), and add to both sides:  
   \(x^2 + 6x + 9 = 16 + 9\)
3. Left side becomes a perfect square:  
   \((x + 3)^2 = 25\)
4. Take the square root: \(x + 3 = \pm 5\)
5. Solve: \(x = 2\) or \(x = -8\)

✅ **Solutions:** \(x = 2, -8\)

#### Worked Example 2 (with negative \(b\))
Solve: \(x^2 - 10x + 1 = 0\)

1. Move the constant: \(x^2 - 10x = -1\)
2. Half of -10 is -5; square it (→ 25); add to both sides:  
   \(x^2 - 10x + 25 = 24\)
3. Factor: \((x - 5)^2 = 24\)
4. Take square root: \(x - 5 = \pm \sqrt{24} = \pm 2\sqrt{6}\)
5. Solve: \(x = 5 \pm 2\sqrt{6}\)

✅ **Solutions:** \(x = 5 + 2\sqrt{6},\; x = 5 - 2\sqrt{6}\)

#### Worked Example 3 (fractional case)
Solve: \(x^2 + 3x - 4 = 0\)

1. Move constant: \(x^2 + 3x = 4\)
2. Half of 3 is \(\tfrac{3}{2}\); square it (→ \(\tfrac{9}{4}\)); add to both sides:  
   \(x^2 + 3x + \tfrac{9}{4} = \tfrac{25}{4}\)
3. Factor: \((x + \tfrac{3}{2})^2 = \tfrac{25}{4}\)
4. Take square root: \(x + \tfrac{3}{2} = \pm \tfrac{5}{2}\)
5. Solve: \(x = 1\) or \(x = -4\)

✅ **Solutions:** \(x = 1, -4\)

#### Steps to Follow
1. Write in standard form \(ax^2 + bx + c = 0\). If \(a \neq 1\), divide everything by \(a\).
2. Move \(c\) to the other side.
3. Take half of \(b\), square it, and add to both sides.
4. Factor the left-hand side.
5. Take the square root of both sides (remember \(\pm\)).
6. Solve for \(x\).

---

### 2.3 Solving by the Quadratic Formula

Factoring and completing the square both lead to a general solution — the **quadratic formula**:

\[
x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}
\]

This formula works for **all quadratic equations**, regardless of whether they factor nicely.

**Example:** Solve \(2x^2 + 9x - 5 = 0\)

1. Identify \(a = 2\), \(b = 9\), \(c = -5\)
2. Substitute into the formula:  
   \(x = \frac{-9 \pm \sqrt{9^2 - 4(2)(-5)}}{4} = \frac{-9 \pm \sqrt{121}}{4}\)
3. Simplify: \(x = \frac{-9 \pm 11}{4}\)

✅ **Solutions:** \(x = 0.5\) and \(x = -5\)

**The Discriminant:**  
\(\Delta = b^2 - 4ac\)
- If \(\Delta > 0\): two distinct real roots.  
- If \(\Delta = 0\): one repeated real root.  
- If \(\Delta < 0\): no real roots (the parabola never crosses the x-axis).

---

### 2.4 Summary: Methods of Solving Quadratic Equations

| Method | Key Idea | Works Best When | Example |
|--------|-----------|----------------|----------|
| **Factoring** | Split into binomial factors | Integers factor neatly | \(x^2 + 5x + 6 = 0\) |
| **Completing the Square** | Create a perfect square trinomial | \(a=1\) or for deriving the formula | \(x^2 + 6x - 16 = 0\) |
| **Quadratic Formula** | Substitute into general formula | Always applicable | \(2x^2 + 9x - 5 = 0\) |

---

## 3. Building and Interpreting Quadratic Equations

Sometimes we know the **roots** and want to find the **equation**. If the roots are \(r_1\) and \(r_2\), the corresponding quadratic is:

\[
(x - r_1)(x - r_2) = 0
\]

Expanding gives \(x^2 - (r_1 + r_2)x + r_1r_2 = 0\).

**Example:** Roots 4 and -1  
→ \((x - 4)(x + 1) = 0\)  
→ \(x^2 - 3x - 4 = 0\)

✅ **Equation:** \(x^2 - 3x - 4 = 0\)

Quadratic equations also appear in practical problems — such as finding dimensions, time, or speed — when quantities are related by multiplication.

---

## 4. Graphs of Quadratic Equations

### 4.1 Key Features of the Parabola

For a quadratic equation \(y = ax^2 + bx + c\):

- **Shape:** U-shaped curve called a parabola.
- **Axis of Symmetry:** Vertical line \(x = -\tfrac{b}{2a}\).
- **Vertex (Turning Point):** The minimum or maximum point of the curve.
- **Y-intercept:** The point where \(x = 0\), i.e., \((0, c)\).
- **X-intercepts:** The roots of the quadratic — where the graph crosses the x-axis.

---

### 4.2 Step-by-Step Graph Construction

Let’s use the example \(y = x^2 + 5x + 6\).

1. **Find the roots (x-intercepts):**  
   \(x^2 + 5x + 6 = (x + 2)(x + 3) = 0\)  
   → \(x = -2, -3\)
2. **Find the y-intercept:**  
   Substitute \(x = 0\): \(y = 6\)  
   → Point: \((0, 6)\)
3. **Find the vertex:**  
   \(x_v = -\tfrac{b}{2a} = -\tfrac{5}{2}\)  
   Substitute \(x = -2.5\) into the equation:  
   \(y_v = (-2.5)^2 + 5(-2.5) + 6 = -0.25\)  
   → Vertex: \((-2.5, -0.25)\)
4. **Axis of symmetry:** \(x = -2.5\)
5. **Shape:** Opens upward (since \(a = 1 > 0\)).

✅ **Graph Summary:**
- Roots: (-2, 0) and (-3, 0)
- Y-intercept: (0, 6)
- Vertex: (-2.5, -0.25)
- Axis of symmetry: x = -2.5

---

### 4.3 Connecting Algebra and Geometry

Each algebraic element of a quadratic corresponds to a geometric feature of its graph:

| Algebraic Form | Geometric Meaning |
|----------------|------------------|
| \(a\) | Controls the direction and width of the parabola |
| \(b\) | Determines the position of the vertex and symmetry |
| \(c\) | Gives the y-intercept (when \(x = 0\)) |
| \(b^2 - 4ac\) | Determines number of x-intercepts (the discriminant) |

The **vertex form** of a quadratic equation, obtained by completing the square, is:

\[
y = a(x - h)^2 + k
\]

Here, \((h, k)\) is the **vertex** of the parabola. This form is especially useful for graphing and visualizing transformations.

---

**In summary**, quadratic equations provide one of the most beautiful links between algebra and geometry — showing how changes in numbers reshape curves and how visual patterns reveal deep mathematical relationships.

