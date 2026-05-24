# Topic 6 — Probability
## Detailed Solutions — Sheet 2

---

## Exercise 1 — Completing the Contingency Table

**Step 1: Fill in what is given directly.**
- S1 total = 120 → S2 total = 200 − 120 = **80**
- S1 ∩ C = 40
- SE total = 30; S2 ∩ SE = 30 ÷ 3 = **10** → S1 ∩ SE = 30 − 10 = **20**
- S2 ∩ A = 50% × 80 = **40**

**Step 2: Fill in the remaining cells by subtraction.**

For the Screen 1 row:
> S1 ∩ A = 120 − 40 (C) − 20 (SE) = **60**

For the Screen 2 row:
> S2 ∩ C = 80 − 40 (A) − 10 (SE) = **30**

Column totals:
> C total = 40 + 30 = **70**
> A total = 60 + 40 = **100**

**Completed table:**

|  | C | A | SE | Total |
|---|---|---|---|---|
| Screen 1 (S1) | 40 | 60 | 20 | 120 |
| Screen 2 (S2) | 30 | 40 | 10 | 80 |
| **Total** | **70** | **100** | **30** | **200** |

**Final check:** 70 + 100 + 30 = 200 ✓

---

## Exercise 2 — Basic Probabilities

**a) P(S1)** — probability the selected viewer watches Screen 1:
> P(S1) = 120/200 = **3/5**

**b) P(A)** — probability the selected viewer is an adult:
> P(A) = 100/200 = **1/2**

---

## Exercise 3 — Conditional Probability from the Table

### Part a) — Describe and calculate P(S1 ∩ C)

**The event S1 ∩ C** is: *"The selected viewer is watching Screen 1 AND is a child."*

From the table, 40 viewers are both on Screen 1 and children:
> P(S1 ∩ C) = 40/200 = **1/5**

---

### Part b) — Conditional Probability P(S1 | A)

**P(S1 | A)** = probability the viewer is on Screen 1, **given** they are an adult.

We use the conditional probability formula:
> P(S1 | A) = P(S1 ∩ A) / P(A)

From the table:
- S1 ∩ A = 60 viewers → P(S1 ∩ A) = 60/200
- A total = 100 viewers → P(A) = 100/200

> P(S1 | A) = (60/200) / (100/200) = 60/100 = **3/5**

**Interpretation:** Among adult viewers, **60% are watching Screen 1**. This is the same as the overall proportion of viewers on Screen 1 (also 3/5 = 60%), which suggests that being an adult does not change the likelihood of watching Screen 1.

*(This hints that events S1 and A may be independent — something worth exploring!)*

---

### Part c) — Conditional Probability P(C | S2)

**P(C | S2)** = probability the viewer is a child, **given** they are on Screen 2.

> P(C | S2) = P(C ∩ S2) / P(S2)

From the table:
- S2 ∩ C = 30 → P(C ∩ S2) = 30/200
- S2 total = 80 → P(S2) = 80/200

> P(C | S2) = (30/200) / (80/200) = 30/80 = **3/8**

**Interpretation:** Among viewers on Screen 2, **37.5% are children** (3 out of every 8). This is higher than the overall proportion of children (70/200 = 35%), suggesting Screen 2's film slightly attracts more children proportionally.

---

## Exercise 4 — Tree Diagram, Total Probability and Bayes' Theorem

**Given:**
- P(A) = 0.35, so P(B) = 0.65
- P(D | A) = 0.04 (4% of Machine A's output is defective)
- P(D | B) = 0.02 (2% of Machine B's output is defective)

---

### Part a) — Probability Tree

```
                              ┌── D  (0.04) ──→ P(A ∩ D) = 0.35 × 0.04 = 0.014
             ┌── A (0.35) ───┤
             │               └── D' (0.96) ──→ P(A ∩ D') = 0.35 × 0.96 = 0.336
Start ───────┤
             │               ┌── D  (0.02) ──→ P(B ∩ D) = 0.65 × 0.02 = 0.013
             └── B (0.65) ───┤
                             └── D' (0.98) ──→ P(B ∩ D') = 0.65 × 0.98 = 0.637
```

**Check:** 0.014 + 0.336 + 0.013 + 0.637 = **1.000** ✓

---

### Part b) — P(A ∩ D)

Using the **multiplication rule** (read directly from the top branch of the tree):

> P(A ∩ D) = P(A) × P(D | A) = 0.35 × 0.04 = **0.014**

*Meaning: 1.4% of all components are both from Machine A and defective.*

---

### Part c) — P(D) using the Total Probability Formula

A component can be defective in two distinct, mutually exclusive ways:
1. It comes from Machine A AND is defective
2. It comes from Machine B AND is defective

So we add both possibilities:
> P(D) = P(A ∩ D) + P(B ∩ D)

We already have P(A ∩ D) = 0.014. For P(B ∩ D):
> P(B ∩ D) = P(B) × P(D | B) = 0.65 × 0.02 = 0.013

Therefore:
> P(D) = 0.014 + 0.013 = **0.027**

*Meaning: 2.7% of all components coming off the production line are defective.*

---

### Part d) — P(A | D): Reverse Conditional Probability (Bayes' Theorem)

**P(A | D)** = probability the component came from Machine A, **given** that it is defective.

This is a **reverse** conditional: we know the component is defective, and we want to trace it back to its source.

We use the conditional probability formula:
> P(A | D) = P(A ∩ D) / P(D)

> P(A | D) = 0.014 / 0.027 ≈ **0.519**

*(As a fraction: 14/27)*

**Interpretation:** If a defective component is found, there is approximately a **52% chance** it came from Machine A, even though Machine A only produces 35% of all components. This seems surprising at first — but it makes sense because Machine A has a **higher defect rate** (4%) than Machine B (2%), so defective components are proportionally more likely to come from Machine A.

---

### Part e) — Are A and D Independent?

**Definition:** A and D are independent if and only if:
> P(A ∩ D) = P(A) × P(D)

**Step 1: Calculate P(A) × P(D).**
> P(A) × P(D) = 0.35 × 0.027 = **0.00945**

**Step 2: Compare with P(A ∩ D).**
> P(A ∩ D) = 0.014

**Step 3: Conclusion.**
Since 0.014 ≠ 0.00945:

> **A and D are NOT independent.**

**Interpretation:** Knowing which machine produced a component **does** affect the probability of it being defective (4% for Machine A vs 2% for Machine B). Because the defect rate differs between machines, the two events are dependent.

---

## Summary: The Three Key Ideas in This Sheet

| Concept | What it means | Formula |
|---|---|---|
| **Joint probability P(A ∩ B)** | Both events happen at the same time | P(A) × P(B \| A) |
| **Total probability P(D)** | Event D can happen via multiple paths | P(A∩D) + P(B∩D) |
| **Reverse conditional P(A \| D)** | Given the outcome, which cause was it? | P(A∩D) / P(D) |
| **Independence test** | Does one event affect the other? | Check: P(A∩B) = P(A)×P(B) |
