# 📘 Hypothesis Testing – Complete & Clear Notes  

These notes explain the core ideas of **statistics and hypothesis testing** in a simple, clear, and exam-friendly way.

---

## 1️⃣ Mean, Median & Mode  

These describe the **center** of a dataset.

### ➗ Mean (Average)  
Mean = (Σx) / n  

Where:  
- Σx = sum of all values  
- n = number of values  

Example:  
60, 70, 80  
Mean = (60 + 70 + 80) / 3 = 70  

---

### 🔢 Median (Middle Value)  
The middle value after arranging data in order.

Example:  
60, 70, 80  
Median = 70  

---

### 🔁 Mode (Most Frequent Value)  
The value that appears most often.

Example:  
60, 70, 70, 80  
Mode = 70  

---

## 2️⃣ Skewness (Shape of Data)

Skewness describes how data is distributed.

### ➡️ Right-Skewed  
- Tail on the right  
- Mean > Median > Mode  
- Example: Income  

### ⬅️ Left-Skewed  
- Tail on the left  
- Mean < Median < Mode  
- Example: Easy exams  

### ⚖️ Symmetric  
- Mean = Median = Mode  
- Example: Normal distribution  

---

## 3️⃣ Normal Distribution  

A **bell-shaped curve** where most values are near the mean.

### Properties  
- Symmetric  
- Mean = Median = Mode  

### 68–95–99.7 Rule  

| Range | % of Data |
|------|-----------|
| Mean ± 1 SD | 68% |
| Mean ± 2 SD | 95% |
| Mean ± 3 SD | 99.7% |

Example (Mean = 70, SD = 5):  
65–75 → 68%  
60–80 → 95%  
55–85 → 99.7%  

---

## 4️⃣ Z-Score  

Z shows how far a value is from the mean.

Z = (x − μ) / σ  

Example:  
Z = (80 − 70) / 5 = 2  

---

## 5️⃣ Standard Normal Distribution  

Mean = 0  
SD = 1  

| Z | Area to Left |
|---|--------------|
| 0.00 | 0.5000 |
| 1.00 | 0.8413 |
| 1.96 | 0.9750 |
| -1.00 | 0.1587 |

---

## 📘 How to Read a Z-Table  

1. Find the row (first two digits of Z)  
2. Find the column (second decimal)  
3. The value is the **area to the left**  

Example:  
Z = 1.23 → Area = 0.8907  

Meaning: 89.07% of values are below Z = 1.23  

---

## 📉 How to Find P-Values Using Z  

Right-tailed:  
p = 1 − (area to left)

Left-tailed:  
p = area to left  

Two-tailed:  
p = 2 × (smaller tail)

---

## 6️⃣ What is a Hypothesis?

A **hypothesis** is a claim about a population.

Example:  
"The average score is 70."

---

## 7️⃣ What is Hypothesis Testing?

Hypothesis testing uses **sample data** to decide whether a claim is likely true.

---

## 8️⃣ Types of Hypotheses  

### Null Hypothesis (H₀)  
No change / no difference  

Example:  
H₀: μ = 70  

### Alternative Hypothesis (H₁)  
There is a difference  

Two-tailed:  
H₁: μ ≠ 70  

Right-tailed:  
H₁: μ > 70  

Left-tailed:  
H₁: μ < 70  

---

## 9️⃣ Alpha (α) – Significance Level  

Alpha is the **risk of rejecting a true H₀**.

Common value:  
α = 0.05  

Meaning:  
5% chance of making a wrong decision.

---

## 🔟 P-Value  

The p-value tells us how likely our result is **if H₀ is true**.

### Decision Rule  

- p ≤ α → Reject H₀  
- p > α → Do not reject H₀  

Small p → Strong evidence  
Large p → Weak evidence  

---

## 1️⃣1️⃣ Z-Test (Large Sample, Known SD)

Use when:  
- n ≥ 30  
- σ known  
- Testing a mean  

Z = (x̄ − μ) / (σ / √n)

Example:  
Z = (495 − 500) / (10 / 6)  
Z = -3  

p ≈ 0.0026 → Reject H₀  

Conclusion: Bottles are underfilled.

---

## 1️⃣2️⃣ T-Test (Small Sample, Unknown SD)

Use when:  
- n < 30  
- σ unknown  

t = (x̄ − μ) / (s / √n)

Example:  
t = 0.76  

p > 0.05 → Do not reject H₀  

---

## 1️⃣3️⃣ T-Table (α = 0.05)

| df | t |
|----|---|
| 4 | 2.776 |

Since 0.76 < 2.776 → Do not reject H₀  

---

## 1️⃣4️⃣ One-Tailed vs Two-Tailed  

Two-tailed:  
H₁: μ ≠ 70  

One-tailed:  
H₁: μ > 70  
or  
H₁: μ < 70  

---

## 1️⃣5️⃣ Chi-Square (χ²) Test  

Used for **categorical data**.

χ² = Σ (O − E)² / E  

Used for:  
- Goodness of fit  
- Independence  

Large χ² → Reject H₀  

---

## 1️⃣6️⃣ ANOVA  

Used to compare **3 or more means**.

Checks if at least one group is different.

---

## 1️⃣7️⃣ When to Use Each Test  

| Situation | Test |
|----------|------|
| Large n, σ known | Z-test |
| Small n, σ unknown | T-test |
| Categorical data | Chi-square |
| 3+ group means | ANOVA |

---

## 1️⃣8️⃣ Final Summary  

- Mean, Median, Mode → Center  
- Skewness → Shape  
- Normal distribution → Bell curve  
- Z-score → Distance from mean  
- Hypothesis → Claim  
- H₀ → No change  
- H₁ → There is change  
- Alpha → Risk  
- P-value → Evidence  
- Z/T-tests → Compare means  
- Chi-square → Categories  
- ANOVA → Many groups  

---

## 📌 Want More?

I can also:  
📘 Create a 1-page cheat sheet  
📝 Add MCQs + answers  
🎯 Make a mock exam paper  
📄 Convert to PDF / Word  

Just tell me what you want 😊  
