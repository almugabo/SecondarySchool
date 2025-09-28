# A Guide to Quadratic Equations

## From Lines to Curves: An Introduction to Quadratics

Do you remember linear equations? They are the ones that follow the general form $$y = mx + c$$. When you graph them, you always get a perfectly straight line.

Now, what happens if we take it a step further and add a more powerful term to our equation? What if we add an $$x^2$$ term?

That’s exactly what a **quadratic equation** is. The standard form of a quadratic equation is:

$$
ax^2 + bx + c = 0
$$

* That little $$x^2$$ term completely changes the game.
* Instead of a straight line, we now get a beautiful, symmetrical U-shaped curve called a **parabola**.

The whole goal of "solving" a quadratic equation is to find the exact points where this parabola crosses the horizontal x-axis. These points are called the **roots** or **solutions** of the equation.

---

## 1. Solving a Quadratic Equation Using Factoring

This is often the quickest method. The idea is to break the quadratic expression down into two simpler expressions (binomials) that are multiplied together. The key principle is the **Zero Product Property**: If $$A \times B = 0$$, then either $$A = 0$$ or $$B = 0$$.

**Example:** Solve $$x^2 + 5x + 6 = 0$$.

1. **Find the factors:** We need two numbers that multiply to give $$c = 6$$ and add to give $$b = 5$$. The numbers are 2 and 3.
2. **Rewrite the equation:**
   $(x + 2)(x + 3) = 0$
3. **Apply the Zero Product Property:**

   * Either $$(x + 2) = 0$$, which gives $$x = -2$$.
   * Or $$(x + 3) = 0$$, which gives $$x = -3$$.

**Solutions:** $$-2$$ and $$-3$$.



---

## 2. Solving with the Quadratic Formula

Factoring doesn’t always work easily. The **quadratic formula** is the universal tool that works for any quadratic equation:

$$
x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}
$$

**Example:** Solve $$2x^2 + 9x - 5 = 0$$.

1. Identify $$a, b, c$$:

   * $$a = 2$$
   * $$b = 9$$
   * $$c = -5$$
2. Plug them into the formula:
   $x = \frac{-9 \pm \sqrt{9^2 - 4(2)(-5)}}{2(2)} = \frac{-9 \pm \sqrt{81 + 40}}{4} = \frac{-9 \pm \sqrt{121}}{4}$
3. Find the two solutions:

   * $$x = \frac{-9 + 11}{4} = 0.5$$
   * $$x = \frac{-9 - 11}{4} = -5$$

**Solutions:** $$0.5$$ and $$-5$$.



---

## 3. Interpreting the Points of Intersection

The **solutions (or roots)** of a quadratic equation are the x-coordinates of the points where the parabola intersects the x-axis:

* **Two solutions:** The parabola crosses the x-axis at two different points.
* **One solution:** The parabola touches the x-axis at one point (the vertex).
* **No real solutions:** The parabola is entirely above or below the x-axis.

---

## 4. Forming an Equation from its Roots

If you know the roots, you can build the original equation. If the roots are $$r_1$$ and $$r_2$$, the equation can be written as:

$(x - r_1)(x - r_2) = 0$

**Example:** Form a quadratic equation whose roots are 4 and -1.

1. Set up the factors:
   $(x - 4)(x + 1) = 0$
2. Multiply out:
   $x^2 - 3x - 4 = 0$

**Equation:** $x^2 - 3x - 4 = 0$.



---

## 5. Solving Word Problems

Quadratics often appear in real-world contexts.

**Strategy:**

1. **Define:** Assign a variable (like $$x$$) to the unknown.
2. **Translate:** Convert words into a mathematical equation.
3. **Solve:** Use factoring or the quadratic formula.
4. **Check:** Ensure the answer makes sense in context.

**Example:** A rectangular garden has an area of $50 \text{ m}^2$. The length is 5 m longer than the width. Find the dimensions.

1. Define: Let the width = $w$. Then length = $w + 5$.
2. Translate: Area = length × width → $50 = w(w + 5)$.
3. Solve:
   $w^2 + 5w - 50 = 0$
   Factor:
   $(w + 10)(w - 5) = 0$
   Solutions: $w = -10$ or $w = 5$.
4. Check: Width can’t be negative → $w = 5$.

   * Width = 5 m
   * Length = 10 m

**Answer:** The garden is **5 m wide** and **10 m long**.


