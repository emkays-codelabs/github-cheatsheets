# 📘 Hypothesis Testing – Complete, Elaborated & Exam-Ready Notes  

---

## 1️⃣ Mean, Median & Mode  

These describe the **center** of a dataset.

### Mean (Average)  
Mean = (Sum of all values) / Number of values  

Example:  
60, 70, 80  
Mean = (60 + 70 + 80) / 3 = 70  

### Median  
Middle value when data is ordered.  
60, 70, 80 → Median = 70  

### Mode  
Most frequent value.  
60, 70, 70, 80 → Mode = 70  

---

## 2️⃣ Skewness (Shape of Data)

| Type | Description | Example |
|----|----|----|
| Right-skewed | Mean > Median > Mode | Income |
| Left-skewed | Mean < Median < Mode | Easy exam |
| Symmetric | Mean = Median = Mode | Normal curve |

---

## 3️⃣ Normal Distribution  

Bell-shaped curve 🔔  
Mean = Median = Mode  

### 68–95–99.7 Rule

| Range | % of Data |
|----|----|
| μ ± 1σ | 68% |
| μ ± 2σ | 95% |
| μ ± 3σ | 99.7% |

---

## 4️⃣ Z-Score  

Measures distance from mean.

Z = (x − μ) / σ  

Example:  
Z = (80 − 70) / 5 = 2  

Meaning:  
Score is **2 SDs above mean**.

---

## 5️⃣ Standard Normal Distribution & Z-Table  

Mean = 0, SD = 1  

| Z | Area to Left |
|----|----|
| 0.00 | 0.5000 |
| 1.00 | 0.8413 |
| 1.96 | 0.9750 |
| -1.00 | 0.1587 |

### How to Read Z-Table  
1. Row → first two digits  
2. Column → second decimal  
3. Value → probability to the left  

---

## 6️⃣ What is a Hypothesis?

A **hypothesis** is a statement about a population parameter.

Example:  
"The average score is 70."

---

## 7️⃣ Hypothesis Testing  

Hypothesis testing uses **sample data** to decide whether a population claim is likely true.

Steps:
1. State H₀ and H₁  
2. Choose test  
3. Compute statistic (z, t, χ²)  
4. Find p-value  
5. Make conclusion  

---

## 8️⃣ Null Hypothesis (H₀)

H₀ represents **no change or no difference**.

Example:  
H₀: μ = 70  

Meaning:  
Assume nothing unusual is happening.

---

## 9️⃣ Alternative Hypothesis (H₁)

Represents a **difference or effect**.

| Type | Form | Meaning |
|----|----|----|
| Two-tailed | μ ≠ 70 | Any difference |
| Right-tailed | μ > 70 | Increase |
| Left-tailed | μ < 70 | Decrease |

---

## 🔟 Significance Level (Alpha, α)

Alpha is the **probability of rejecting a true H₀**.

Common value:  
α = 0.05  

Meaning:  
5% risk of making a wrong decision.

---

## 1️⃣1️⃣ P-Value  

Probability of getting the sample result **if H₀ is true**.

### Decision Rule

| p-value | Decision |
|----|----|
| p ≤ 0.05 | Reject H₀ |
| p > 0.05 | Do not reject H₀ |

Small p → strong evidence  
Large p → weak evidence  

---

## 1️⃣2️⃣ Z-Test (Large Sample, σ Known)

### When to Use  
- n ≥ 30  
- σ known  
- Testing a mean  

Z = (x̄ − μ) / (σ / √n)

### Example  
μ = 500  
x̄ = 495  
σ = 10, n = 36  

Z ≈ −3  
p ≈ 0.0026  

### Conclusion  
p < 0.05 → Reject H₀  
Bottles are underfilled.

---

## 1️⃣3️⃣ T-Test (Small Sample, σ Unknown)

t = (x̄ − μ) / (s / √n)

---

## 1️⃣4️⃣ Types of T-Tests  

| Type | Purpose |
|----|----|
| One-sample | Compare with known mean |
| Independent | Compare two groups |
| Paired | Before vs After |

---

## 1️⃣5️⃣ One-Sample T-Test Example  

Scores: 65, 68, 75, 80, 72  

Mean = 72  
SD ≈ 5.87  
n = 5  

t ≈ 0.76  
df = 4  

t-critical = 2.776  

### Conclusion  
|t| < t-critical → Do not reject H₀  
No significant difference from 70.

---

## 1️⃣6️⃣ Independent T-Test  

Used to compare **two independent groups**.

H₀: μ₁ = μ₂  
H₁: μ₁ ≠ μ₂  

### Conclusion  
Reject H₀ → Groups differ  
Do not reject → Groups similar  

---

## 1️⃣7️⃣ Paired T-Test  

Used for **before-after comparisons**.

H₀: μd = 0  

### Conclusion  
Reject H₀ → Change occurred  
Do not reject → No clear effect  

---

## 1️⃣8️⃣ T-Test Conclusion Summary  

| Test | Reject H₀ Means |
|----|----|
| One-sample | Mean differs |
| Independent | Groups differ |
| Paired | Change occurred |

---

## 1️⃣9️⃣ T-Table (α = 0.05)

| df | t |
|----|----|
| 1 | 12.706 |
| 2 | 4.303 |
| 3 | 3.182 |
| 4 | 2.776 |
| 5 | 2.571 |
| 10 | 2.228 |
| ∞ | 1.960 |

---

## 2️⃣0️⃣ Chi-Square Test  

Used for **categorical data**.

χ² = Σ (O − E)² / E  

### Conclusion  
Large χ² → Reject H₀  
Small χ² → Do not reject  

---

## 2️⃣1️⃣ ANOVA  

Compares **3 or more group means**.

H₀: All means equal  
H₁: At least one differs  

### Conclusion  
p ≤ 0.05 → Groups differ  

---

## 2️⃣2️⃣ When to Use Each Test  

| Situation | Test |
|----|----|
| Large n, σ known | Z-test |
| Small n, σ unknown | T-test |
| Categorical data | Chi-square |
| 3+ means | ANOVA |

---

## 2️⃣3️⃣ Final Exam Summary  

• H₀ = No effect  
• H₁ = Effect exists  
• α = Significance level  
• p-value = Evidence strength  
• Reject H₀ = Significant result  
• Z-test = Large sample  
• T-test = Small sample  
• Chi-square = Categories  
• ANOVA = Many groups  

---
