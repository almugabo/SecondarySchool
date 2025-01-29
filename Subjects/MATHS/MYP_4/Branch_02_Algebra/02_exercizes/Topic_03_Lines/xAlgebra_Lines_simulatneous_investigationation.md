
## investigation 1 

Below is one example of a follow‐on activity that reinforces the same big ideas (one solution / no solutions / infinitely many solutions) but lets students *actively* discover the patterns by “playing” with parameters. The idea is for them to see directly how changing slopes and intercepts affects solutions, and then articulate the rules they discover.

---

### **Proposed Exercise: Exploring Families of Lines**

**Objective:**  
Help students discover (and then state) the conditions for one solution, no solutions, and infinitely many solutions by systematically manipulating parameters in linear equations.

1. **Set up parameters with sliders**  
   - In Desmos, type:
     
     $$y = m_1x + b_1$$
     
     $$y = m_2x + b_2$$
   - Click “add slider” for each of $m_1, b_1, m_2, b_2$.  
   - This creates four sliders that students can move.

2. **Experiment and Observe**  
   - ** 2.1. Vary the Slopes**: Move $m_1$ and $m_2$ while keeping $b_1$ and $b_2$ fixed.  
     - **What do you notice if $m_1 \neq m_2$?**  
     - **How many intersection points appear on the graph?**  
   - **2.2 Same Slopes, Different Intercepts**: Try setting $m_1 = m_2$ but make $b_1 \neq b_2$  
     - **What do you notice about the lines now?**  
     - **How many intersection points appear?**  
   - **2.3. Same Slopes, Same Intercepts**: Now set $m_1 = m_2$ and $b_1 = b_2$.  
     - **What do you notice about the lines?**  
     - **How many points of intersection do they have?**  

3. **Record Your Findings**  
   Create a small table or list in which students record:  
   - **Case 1**: $m_1 \neq m_2$
   - **Case 2**: $m_1 = m_2$ but $b_1 \neq b_2$  
   - **Case 3**: $m_1 = m_2$ and $b_1 = b_2$  

   For each case, have them write:
   - **Are the lines parallel, coincident, or intersecting in exactly one point?**  
   - **How many solutions does the system have?**  

4. **Verbalize the Rule**  
   Finally, have them write down in words the general “rules” they have discovered:
   1. **Different slopes** \(\implies\) exactly one intersection point (one solution).  
   2. **Same slope, different intercept** \(\implies\) parallel lines (no solutions).  
   3. **Same slope, same intercept** \(\implies\) same line (infinitely many solutions).



### Extensions and Additional Variations

1. **Challenge Extension**  
   - *create* your own pairs $m_1, b_1$ and $m_2, b_2$ that fall under each case and verify the number of solutions by looking at the graph.  
   - express each set of lines in *both* slope-intercept form and standard form. compare how the algebraic condition (e.g., same slope means same coefficients $A, B$ in standard form) matches what they see in the graph.  


2. **Three Lines**  
   Add a third line \(y = m_3 x + b_3\). Ask:  
   - Under what conditions do all three lines meet at a single point (one common intersection)?  
   - Is it possible for all three lines to coincide? (Infinitely many solutions.)  
   - Can you arrange them to have no common intersection?

---

## Invesigation 2 

**Exercise Title:  Exploring the Impact of Coefficients on Solutions of Simultaneous Equations**

**Introduction:**

In the previous exercise, you used graphs to understand different types of solutions for simultaneous equations – one solution, no solution, and infinite solutions. Now, we will explore how changing the **coefficients** in the equations affects these solutions and the lines they represent. This exercise will help you discover the rules that determine the type of solution based on the numbers in the equations themselves.

**Instructions:**

Use algebraic manipulation and Desmos (optional for verification, but encouraged) to answer the following questions.

**Part 1:  Manipulating Coefficients for One Solution**

1. **Start with a pair of equations that have one solution:**  Let's use:
   * Equation 1:  y = x + 2
   * Equation 2:  y = -2x + 8

   a. Solve these equations simultaneously (using substitution or elimination) to find the coordinates of the intersection point.

   b. Now, **change only the coefficient of 'x' in Equation 2.** Keep the constant term (8) and the coefficient of 'x' in Equation 1 (which is 1) and the constant term in Equation 1 (which is 2) the same.  Try a few different values for the coefficient of 'x' in Equation 2 (e.g., -x, -3x, 0.5x). For each change, solve the new pair of equations and observe what happens to the solution.

   c. What do you notice about the number of solutions when you change only the coefficient of 'x' in Equation 2 (while keeping other coefficients and constants the same)?

   d. **Now, go back to the original pair of equations (y = x + 2 and y = -2x + 8). This time, change only the constant term in Equation 2.** Keep the coefficients of 'x' and 'y' the same as the original equations. Try a few different constant terms (e.g., 5, 10, 0). For each change, solve the new pair of equations and observe what happens to the solution.

   e. What do you notice about the number of solutions when you change only the constant term in Equation 2 (while keeping other coefficients the same)?

**Part 2:  Creating Equations with No Solution**

2. **Start again with Equation 1: y = x + 2.**

   a.  Think about what makes two lines parallel.  What needs to be the same about their equations? (Hint: think about slope-intercept form y = mx + c).

   b.  Write a new Equation 2 that has **the same coefficient of 'x'** as Equation 1 but a **different constant term.** For example, y = x + 5.

   c. Solve the system of equations you created in step 2b. What do you find?

   d. Graph both equations in Desmos. What do you observe about the lines?

   e.  Can you create other pairs of equations that have no solution by following a similar pattern of coefficients and constant terms? Try a few and test them.

**Part 3: Creating Equations with Infinite Solutions**

3. **Start again with Equation 1: y = x + 2.**

   a. Think about what it means for two lines to be the same line. What must be true about their equations?

   b. Write a new Equation 2 that is essentially the same as Equation 1 but looks slightly different. You can do this by multiplying Equation 1 by a constant number. For example, multiply Equation 1 by 2 to get 2y = 2x + 4.  (Rewrite this in the form y = ...).

   c. Solve the system of equations you created in step 3b. What do you find?

   d. Graph both equations in Desmos. What do you observe about the lines?

   e. Can you create other pairs of equations that have infinite solutions by following a similar pattern of manipulating Equation 1? Try a few and test them.

**Part 4:  Generalizing the Rules**

4.  Based on your observations in Parts 1, 2, and 3, try to formulate general rules about how the coefficients and constant terms in a pair of linear equations determine:

    a. When there will be **one unique solution**.  What must be different or the same about the coefficients?
    b. When there will be **no solution**. What must be the same or different about the coefficients and constant terms?
    c. When there will be **infinite solutions**. What must be the relationship between the two equations?

5. **Challenge:**  Can you express these rules using ratios of the coefficients and constant terms?  Consider the general form of linear equations:

   * Equation 1:  a₁x + b₁y = c₁
   * Equation 2:  a₂x + b₂y = c₂

   Can you find relationships between a₁, b₁, c₁, a₂, b₂, and c₂ that predict the number of solutions? (This is more advanced, but encourage students to think about it if they are ready).






