# 📘 Hypothesis Testing – Complete & Clear Notes  

✨ Clean, corrected, and exam-ready!  

These notes cover:  
- 📊 Mean, Median, Mode  
- 📐 Skewness  
- 🔔 Normal & Standard Normal Distribution  
- 📏 Z-Score  
- 🧪 Hypothesis Testing  
- 📉 P-Value  
- 📈 Z-Test  
- 📚 T-Test  
- 🧮 Chi-Square Test  
- 📊 ANOVA  
- ➡️ One-tailed & Two-tailed tests  
- 🛠️ When to use each test  

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
Mean = (60 + 70 + 80) / 3 = **70**

---

### 🔢 Median (Middle Value)  

The middle value when data is ordered.

Example:  
60, 70, 80  
Median = **70**

---

### 🔁 Mode (Most Frequent Value)  

The value that appears most often.

Example:  
60, 70, 70, 80  
Mode = **70**

---

## 2️⃣ Skewness  

Skewness describes the **shape** of the data.

### ➡️ Right-Skewed (Positive Skew)  
- Tail on the right  
- Mean > Median > Mode  
- Example: 💰 Income data  

### ⬅️ Left-Skewed (Negative Skew)  
- Tail on the left  
- Mean < Median < Mode  
- Example: 📝 Easy exam scores  

### ⚖️ Symmetric  
- Mean = Median = Mode  
- Example: 🔔 Normal distribution  

---

## 3️⃣ Normal Distribution  

The normal distribution is a **bell-shaped curve** 🔔  

### Key Features  
- Symmetric  
- Mean = Median = Mode  
- Most values near the mean  

### 📏 68–95–99.7 Rule  

| Range | % of Data |
|------|-----------|
| μ ± 1σ | 68% |
| μ ± 2σ | 95% |
| μ ± 3σ | 99.7% |

Example:  
If Mean = 70, SD = 5  
- 68% → 65 to 75  
- 95% → 60 to 80  
- 99.7% → 55 to 85  

---

## 4️⃣ Z-Score  

Z = (x − μ) / σ  

Where:  
- x = observed value  
- μ = population mean  
- σ = population standard deviation  

Example:  
Z = (80 − 70) / 5 = **2**

---

## 5️⃣ Standard Normal Distribution  

- Mean = 0  
- SD = 1  

### 🔍 What does “Area to the Left” mean?

The **Area to the Left** shows the probability that a value is **LESS than** a given Z-score.

| Z | Area to Left | Meaning |
|---|--------------|---------|
| 0.00 | 0.5000 | 50% of data is below the mean |
| 1.00 | 0.8413 | 84.13% of data is below Z = 1 |
| 1.96 | 0.9750 | 97.5% of data is below Z = 1.96 |
| -1.00 | 0.1587 | 15.87% of data is below Z = -1 |

Example:  
If Z = 1.00, then **84.13%** of the data is less than that value.

---

## 📘 How to Read a Full Z-Table  

A Z-table shows the **area to the left** of a Z-score.

### Steps:

1. Find the **row** for the first two digits of Z  
2. Find the **column** for the second decimal  
3. The intersection gives the **area to the left**

### Example: Z = 1.23  

Row = 1.2  
Column = 0.03  
Area ≈ **0.8907**

Meaning:  
**89.07%** of the data is below Z = 1.23

---

## 📉 How to Find P-Values Using Z  

### Right-Tailed Test (H₁: μ > 70)

p-value = 1 − Area to Left  

Example:  
Z = 1.50  
Area = 0.9332  

p = 1 − 0.9332 = **0.0668**

---

### Left-Tailed Test (H₁: μ < 70)

p-value = Area to Left  

Example:  
Z = -1.20  
Area = **0.1151**

p = **0.1151**

---

### Two-Tailed Test (H₁: μ ≠ 70)

p-value = 2 × (Smaller tail area)

Example:  
Z = 1.96  
Area = 0.9750  

Tail = 1 − 0.9750 = 0.025  

p = 2 × 0.025 = **0.05**

---

## 6️⃣ Hypothesis Testing  

Null Hypothesis (H₀):  
H₀: μ = 70  

Alternative Hypothesis (H₁):  
H₁: μ ≠ 70  

---

## 7️⃣ P-Value  

- p ≤ 0.05 → ❌ Reject H₀  
- p > 0.05 → ✅ Do not reject H₀  

---

## 8️⃣ Z-Test (Large Sample, σ Known)  

Z = (x̄ − μ) / (σ / √n)  

Example:  
Z = (495 − 500) / (10 / √36)  
Z = -5 / 1.67 ≈ **-3**

---

## 9️⃣ T-Test (Small Sample, σ Unknown)  

t = (x̄ − μ) / (s / √n)  

Example:  
t ≈ **0.76**

---

## 🔟 T-Table (α = 0.05, Two-Tailed)  

| df | t |
|----|---|
| 4 | 2.776 |

---

## 1️⃣1️⃣ One-Tailed vs Two-Tailed  

Two-tailed:  
H₁: μ ≠ 70  

One-tailed:  
H₁: μ > 70  
or  
H₁: μ < 70  

---

## 1️⃣2️⃣ Chi-Square (χ²) Test  

χ² = Σ (O − E)² / E  

Where:  
- O = observed frequency  
- E = expected frequency  

---

## 1️⃣3️⃣ ANOVA  

Used to compare **3 or more group means**.

---

## 1️⃣4️⃣ When to Use Each Test  

| Situation | Test |
|----------|------|
| Large n, σ known | Z-test |
| Small n, σ unknown | T-test |
| Categorical data | Chi-square |
| 3+ group means | ANOVA |

---

## 1️⃣5️⃣ Final Summary  

- 📊 Mean, Median, Mode → Center  
- 📐 Skewness → Shape  
- 🔔 Normal distribution → Bell curve  
- 📏 Z-scores → Distance from mean  
- 🧪 Hypothesis testing → Check claims  
- 📉 P-value → Decision tool  
- 📈 Z & T-tests → Compare means  
- 🧮 Chi-square → Categories  
- 📊 ANOVA → Many groups  
