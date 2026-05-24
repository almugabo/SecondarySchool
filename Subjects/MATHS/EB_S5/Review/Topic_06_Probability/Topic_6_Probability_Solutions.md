# Topic 6 — Probability
## Detailed Solutions

---

## Exercise 1 — Completing the Contingency Table

**Reading off the given information:**
- Total members = 150; Swimming (N) = 90 → Tennis (T) = 150 − 90 = **60**
- N ∩ Y = 30 (given)
- T ∩ A = 50% of 60 = **30**
- S total = 45; N ∩ S = 45 ÷ 3 = **15** → T ∩ S = 45 − 15 = **30**

**Filling in the remaining cells by subtraction:**

For Swimming row: 30 (Y) + A + 15 (S) = 90 → N ∩ A = 90 − 30 − 15 = **45**

For Tennis row: T ∩ Y + 30 (A) + 30 (S) = 60 → T ∩ Y = 60 − 30 − 30 = **0**

Column totals: Y = 30 + 0 = **30** | A = 45 + 30 = **75**

**Completed table:**

|  | Y | A | S | Total |
|---|---|---|---|---|
| Swimming (N) | 30 | 45 | 15 | 90 |
| Tennis (T) | 0 | 30 | 30 | 60 |
| **Total** | **30** | **75** | **45** | **150** |

---

## Exercise 2 — Basic Probabilities

All probabilities = (favourable outcomes) / (total outcomes)

**a) P(N)** — probability the selected person does swimming:
> P(N) = 90/150 = **3/5**

**b) P(S)** — probability the selected person is in the senior group:
> P(S) = 45/150 = **3/10**

---

## Exercise 3 — Conditional Probability from the Table

### Part a) — Describe and calculate P(N ∩ Y)

**N ∩ Y** is the event: *"The selected member does swimming AND is in the under-18 (Y) age group."*

From the table, there are 30 members in both N and Y:
> P(N ∩ Y) = 30/150 = **1/5**

---

### Part b) — Conditional Probability P(N | Y)

**P(N | Y)** = probability that the person does swimming, **given** they are in group Y.

We use the conditional probability formula:
> P(N | Y) = P(N ∩ Y) / P(Y)

From the table:
- P(N ∩ Y) = 30/150
- P(Y) = 30/150

> P(N | Y) = (30/150) / (30/150) = **1**

**Interpretation:** Given that a member is under 18, they are **certain** to be a swimmer. This makes sense because, according to the table, there are **no young tennis players** (T ∩ Y = 0) — all 30 young members swim.

---

### Part c) — Conditional Probability P(S | T)

**P(S | T)** = probability that the person is senior, **given** they play tennis.

> P(S | T) = P(S ∩ T) / P(T)

From the table:
- P(S ∩ T) = 30/150
- P(T) = 60/150

> P(S | T) = (30/150) / (60/150) = 30/60 = **1/2**

**Interpretation:** Among tennis players, exactly **50% are seniors**. If we know someone plays tennis, there is an equal chance that they are or are not a senior member.

---

## Exercise 4 — Tree Diagram and Independence

**Given:**
- P(W) = 0.60, so P(M) = 0.40 (60% women, 40% men)
- P(E | W) = 0.30 (30% of women exercise frequently)
- P(E | M) = 0.20 (20% of men exercise frequently)

---

### Part a) — Probability Tree

```
                            ┌── E  (0.30) ─── P(W ∩ E) = 0.60 × 0.30 = 0.18
               ┌── W (0.60)─┤
               │            └── E' (0.70) ─── P(W ∩ E') = 0.60 × 0.70 = 0.42
Start ─────────┤
               │            ┌── E  (0.20) ─── P(M ∩ E) = 0.40 × 0.20 = 0.08
               └── M (0.40)─┤
                            └── E' (0.80) ─── P(M ∩ E') = 0.40 × 0.80 = 0.32
```

Check: 0.18 + 0.42 + 0.08 + 0.32 = 1.00 ✓

---

### Part b) — P(W ∩ E)

We read directly from the tree (or use the multiplication rule):

> P(W ∩ E) = P(W) × P(E | W) = 0.60 × 0.30 = **0.18**

*Meaning: 18% of all members are women who exercise frequently.*

---

### Part c) — P(E)

A member exercises frequently if they are **either** a woman who exercises frequently **or** a man who exercises frequently. We use the **total probability formula**:

> P(E) = P(W ∩ E) + P(M ∩ E)

We already know P(W ∩ E) = 0.18. From the tree:
> P(M ∩ E) = P(M) × P(E | M) = 0.40 × 0.20 = 0.08

Therefore:
> P(E) = 0.18 + 0.08 = **0.26**

*Meaning: 26% of all members exercise more than 3 times per week.*

---

### Part d) — Are W and E Independent?

**Definition:** Two events are **independent** if knowing one occurs does not change the probability of the other. Formally:

> W and E are independent   ⟺   P(W ∩ E) = P(W) × P(E)

**Step 1: Calculate P(W) × P(E).**
> P(W) × P(E) = 0.60 × 0.26 = **0.156**

**Step 2: Compare with P(W ∩ E).**
> P(W ∩ E) = 0.18

**Step 3: Draw the conclusion.**
Since 0.18 ≠ 0.156, the condition is **not satisfied**.

> **W and E are NOT independent.**

**Interpretation:** Knowing that a member is a woman changes the probability that they exercise frequently — it increases from 26% (the overall rate) to 30% (the rate among women). Because the gender of the member affects the probability of exercising frequently, the two events are **dependent**.

---

## Key Formulas for Probability

| Concept | Formula |
|---|---|
| Conditional probability | P(A \| B) = P(A ∩ B) / P(B) |
| Multiplication rule | P(A ∩ B) = P(B) × P(A \| B) |
| Total probability | P(A) = P(A ∩ B) + P(A ∩ B') |
| Independence condition | P(A ∩ B) = P(A) × P(B) |
| Complementary event | P(A') = 1 − P(A) |
