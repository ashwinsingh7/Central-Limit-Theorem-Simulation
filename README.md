Colab link can be found here https://colab.research.google.com/drive/1XOSH6bw4V-_wQKb1OBVYH0q5TelcyzsV?usp=sharing 

# 📌 Simulation to Test the Central Limit Theorem (CLT)

## 🔍 Overview

This project explores the **Central Limit Theorem (CLT)** using a simulation-based approach. It demonstrates how the distribution of sample means approximates normality, regardless of the population's original distribution. 

Additionally, the project investigates:
- The **effect of sample size** on normality.
- A **random walk problem**, comparing solutions via **CLT vs. simulation**.
- A discussion on **percentiles vs. confidence intervals** in statistical inference.

---

## 🛠 Methodology

### **1️⃣ Testing the Central Limit Theorem (CLT)**
1. **Generate a Uniform Population**  
   - Create a **uniformly distributed population**.
2. **Sampling Process**  
   - Draw **10,000 samples**, each containing **100 observations**.  
   - Compute the **sample mean** for each sample.
3. **Standardization**  
   - Compute the **mean (m) and standard deviation (s)** of the sample means.  
   - Standardize using **Z-score transformation**:
     ```
     Z = (X - m) / s
     ```
4. **Normality Verification**  
   - Analyze **skewness and kurtosis**.  
   - Plot **histograms** to visually confirm normality and use the **Jarque Bera** hypothesis test to test normality.

---

### **2️⃣ Effect of Sample Size on Normality**
- Investigates how **changing sample size** affects normality.
- Multiple simulations are conducted with **varying sample sizes** from a Uniformly distributed population.
- Helps visualize how CLT holds as **n increases**, reinforcing its practical significance.

---

### **3️⃣ Example Problem - Comparing CLT with a Simulation**
A **random walk problem** using a **6-sided fair die**:
- **Rules:**
  - Roll the die **100 times**.
  - Movement rules:
    - `-1 step` if `1,2` appear.
    - `+1 step` if `3,4,5` appear.
    - If `6` appears, reroll and move accordingly.
- **Objective:**
  - Determine **the probability of reaching 60+ steps**.

📌 **Two Approaches to Solve the Problem**:
1. **Approach 1 - Using Central Limit Theorem**  
   - Applies **CLT-based probability calculations**.
2. **Approach 2 - Monte Carlo Simulation**  
   - Simulates **thousands of trials** to approximate the probability.

📊 **Includes a Random Walk Visualization** to illustrate movement patterns.

---

### **4️⃣ Percentiles vs. Confidence Intervals**
- Discusses the **differences between percentiles & confidence intervals**.
- **Percentiles** help rank data points in a dataset.
- **Confidence Intervals** estimate **population parameters** from a sample.
- Clarifies **why confidence intervals are crucial in statistical inference**.

---

## 🎯 Results & Insights

- The **sample means distribution** follows a **bell curve**, confirming **CLT**.
- **Larger sample sizes** improve normality, showcasing **CLT’s dependence on n**.
- The **random walk problem** validates **CLT-based probability estimates** using **simulation**.
- The **percentiles vs. confidence intervals discussion** highlights key differences in **descriptive vs. inferential statistics**.

---
