# 📘 Hypothesis Testing – Complete, Clear & Exam-Ready Notes  

---

## 1️⃣ Mean, Median & Mode  

These describe the **center** of data.

### Mean (Average)  
Mean = (Sum of all values) / Number of values  

Example:  
60, 70, 80  
Mean = (60 + 70 + 80) / 3 = **70**

### Median  
Middle value when data is ordered.  
60, 70, 80 → Median = **70**

### Mode  
Most frequent value.  
60, 70, 70, 80 → Mode = **70**

---

## 2️⃣ Skewness (Shape of Data)

| Type | Description | Example |
|------|------------|---------|
| Right-skewed | Tail on right, Mean > Median | Income |
| Left-skewed | Tail on left, Mean < Median | Easy exam |
| Symmetric | Mean = Median = Mode | Normal curve |

---

## 3️⃣ Normal Distribution  

Bell-shaped curve 🔔  
Mean = Median = Mode  

### 68–95–99.7 Rule  

| Range | % of Data |
|------|-----------|
| μ ± 1σ | 68% |
| μ ± 2σ | 95% |
| μ ± 3σ | 99.7% |

---

## 4️⃣ Z-Score  

Measures distance from the mean.

Z = (x − μ) / σ  

Example:  
Z = (80 − 70) / 5 = **2**

---

## 5️⃣ Standard Normal Distribution (Z-Table)

Mean = 0, SD = 1  

| Z | Area to Left |
|---|--------------|
| 0.00 | 0.5000 |
| 1.00 | 0.8413 |
| 1.96 | 0.9750 |
| -1.00 | 0.1587 |

### How to Read Z-Table  
1. Row = first two digits  
2. Column = second decimal  
3. Value = area to the left  

---

## 6️⃣ What is a Hypothesis?  

A **hypothesis** is a claim about a population.

Example:  
"The average score is 70."

---

## 7️⃣ Hypothesis Testing  

Uses **sample data** to test a population claim.

---

## 8️⃣ Null & Alternative Hypotheses  

### Null Hypothesis (H₀)  
No change / no difference  
H₀: μ = 70  

### Alternative Hypothesis (H₁)

| Type | Form | Meaning |
|------|------|---------|
| Two-tailed | μ ≠ 70 | Any difference |
| Right-tailed | μ > 70 | Increase |
| Left-tailed | μ < 70 | Decrease |

---

## 9️⃣ Alpha (α)  

Significance level  
Common value: **0.05**

Means:  
5% risk of rejecting a true H₀

---

## 🔟 P-Value  

Probability of getting the result **if H₀ is true**.

| p-value | Decision |
|--------|----------|
| p ≤ 0.05 | Reject H₀ |
| p > 0.05 | Do not reject H₀ |

Small p → Strong evidence  
Large p → Weak evidence  

---

## 1️⃣1️⃣ Z-Test (Large Sample, σ Known)

### When to Use  
- n ≥ 30  
- σ known  
- Testing a mean  

Z = (x̄ − μ) / (σ / √n)

### Example  
Claim: μ = 500  
Sample mean = 495  
σ = 10, n = 36  

Z = (495 − 500) / (10 / 6)  
Z ≈ **−3**  

p ≈ 0.0026 → Reject H₀  
Conclusion: Bottles are underfilled.

---

## 1️⃣2️⃣ T-Test (Small Sample, σ Unknown)

t = (x̄ − μ) / (s / √n)

---

## 1️⃣3️⃣ Types of T-Tests  

| Type | Purpose |
|------|---------|
| One-sample | Compare to known mean |
| Independent | Compare two groups |
| Paired | Before vs After |

---

## 1️⃣4️⃣ One-Sample T-Test Example  

Scores: 65, 68, 75, 80, 72  

Mean = 72  
SD ≈ 5.87  
n = 5  

t = (72 − 70) / (5.87 / √5)  
t ≈ **0.76**

df = 5 − 1 = 4  

From t-table:  
t-critical = **2.776**

0.76 < 2.776  
Conclusion: Do not reject H₀  

---

## 1️⃣5️⃣ Independent T-Test  

Compares **two different groups**.

Example:  
Class A vs Class B  

H₀: μ₁ = μ₂  
H₁: μ₁ ≠ μ₂  

---

## 1️⃣6️⃣ Paired T-Test  

Compares **before & after**.

Example:  
Before: 60, 65  
After: 70, 75  

---

## 1️⃣7️⃣ T-Table (α = 0.05, Two-Tailed)

| df | t |
|----|----|
| 1 | 12.706 |
| 2 | 4.303 |
| 3 | 3.182 |
| 4 | 2.776 |
| 5 | 2.571 |
| 10 | 2.228 |
| ∞ | 1.960 |

### How to Read  
1. Find df  
2. Choose α  
3. Pick tail type  
4. Compare |t| with t-critical  

---

## 1️⃣8️⃣ One-Tailed vs Two-Tailed  

| Test | Hypothesis |
|------|------------|
| Two-tailed | μ ≠ 70 |
| Right-tailed | μ > 70 |
| Left-tailed | μ < 70 |

---

## 1️⃣9️⃣ Chi-Square (χ²) Test  

For **categorical data**.

χ² = Σ (O − E)² / E  

Used for:  
- Goodness of fit  
- Independence  

---

## 2️⃣0️⃣ ANOVA  

Compares **3+ group means**.

Example:  
3 class scores  

If p ≤ 0.05 → At least one group differs.

---

## 2️⃣1️⃣ When to Use Each Test  

| Situation | Test |
|----------|------|
| Large n, σ known | Z-test |
| Small n, σ unknown | T-test |
| Categorical data | Chi-square |
| 3+ means | ANOVA |

---

## 2️⃣2️⃣ Final Summary  

• Mean, Median, Mode → Center  
• Skewness → Shape  
• Normal curve → Bell-shaped  
• Z-scores → Distance  
• Hypothesis testing → Check claims  
• Alpha → Significance level  
• P-value → Decision  
• Z-test & T-test → Compare means  
• Chi-square → Categories  
• ANOVA → Many groups  

---
