Google Colab notebook can be found here https://colab.research.google.com/drive/1XOSH6bw4V-_wQKb1OBVYH0q5TelcyzsV?usp=sharing 

---

# Simulation to Test the Central Limit Theorem (CLT)

## Overview

This project explores the **Central Limit Theorem (CLT)** using a simulation-based approach. It demonstrates how the distribution of a large number sample means approximates a Normal distribution, regardless of the population's original distribution. 

Additionally, the project investigates:
- The **effect of sample size** on normality.
- A **random walk problem**, comparing solutions using **CLT vs. simulation**.
- A discussion on **confidence intervals** in statistical inference.

---

## Methodology

### **1️⃣ Testing the Central Limit Theorem (CLT)**
1. **Generate a Uniform Population**  
   - Create a **uniformly distributed population**.
2. **Sampling Process**  
   - Draw **10,000 samples**, each sample containing **100 observations**.  
   - Compute the **sample mean** for each sample.
3. **Standardisation**  
   - Compute the **mean (m) and standard deviation (s)** of the 10,000 sample means.  
   - Standardise each observation X using:
     ```
     Z = (X - m) / s
     ```
4. **Normality Verification**  
   - Analyse **skewness and kurtosis** of the resultant (mean-centred and std dev scaled) set of sample means.  
   - Plot **histograms** to visually confirm normality and use the **Jarque Bera** hypothesis test to test normality.

<img width="300" alt="Screenshot 2025-03-23 at 4 07 00 PM" src="https://github.com/user-attachments/assets/37a7d818-2f5e-4bf2-98e8-e799d7917bf9" /> <img width="300" alt="Screenshot 2025-03-23 at 4 07 26 PM" src="https://github.com/user-attachments/assets/8df4c39a-5dff-41ec-aacd-175af6453738" /> <img width="300" alt="Screenshot 2025-03-23 at 4 07 36 PM" src="https://github.com/user-attachments/assets/5ed157bf-f66e-4e69-839b-bf21be7ffc01" />

---

### **2️⃣ Effect of Sample Size on Normality**
- Investigates how **changing sample size** affects normality.
- Multiple simulations are conducted with **varying sample sizes** from a Uniformly distributed population.
- Helps visualise how CLT holds as **n increases**, reinforcing its practical significance.

<img width="450" alt="Screenshot 2025-03-23 at 4 20 19 PM" src="https://github.com/user-attachments/assets/68ba90eb-eae4-4373-8c64-db7b23e554ed" />


---

### **3️⃣ Example Problem - Comparing CLT with a Simulation**
A **random walk problem** using a **6-sided fair die**:
- **Rules:**
  - Roll the die **100 times**.
  - Movement rules:
    - `-1 step` if `1,2` appear.
    - `+1 step` if `3,4,5` appear.
    - If `6` appears, reroll and move accordingly.
   
   <img width="400" alt="Screenshot 2025-03-23 at 4 24 38 PM" src="https://github.com/user-attachments/assets/1a86acf9-c626-40cc-8574-1b16e773fdd9" />


- **Objective:**
  - Determine **the probability of reaching 60+ steps**.

**Two Approaches to Solve the Problem**:
1. **Approach 1 - Using Central Limit Theorem**  
   - Applies **CLT-based probability calculations**.
2. **Approach 2 - Monte Carlo Simulation**  
   - Simulates **thousands of trials** to approximate the probability.

**Includes a Random Walk Visualisation** to illustrate movement patterns.

<img width="350" alt="Screenshot 2025-03-23 at 4 26 12 PM" src="https://github.com/user-attachments/assets/fcb15f83-84c4-4ddc-b749-a8c20e8e6d71" />
<img width="300" alt="Screenshot 2025-03-23 at 4 26 43 PM" src="https://github.com/user-attachments/assets/748a119e-6df8-487b-b495-448b762de7d8" /> <img width="700" alt="Screenshot 2025-03-23 at 4 27 01 PM" src="https://github.com/user-attachments/assets/fc2fc2e4-393e-4b2b-8abd-4e3f80c70d4d" />


---

### **4️⃣ Percentiles vs. Confidence Intervals**
- Discusses the **differences between percentiles & confidence intervals**.
- **Percentiles** help rank data points in a dataset.
- **Confidence Intervals** help provide interval estimates for **population parameters** from a sample.
- Clarifies **why confidence intervals are crucial in statistical inference** and **how CLT is useful for statitistical inference**.

---

## Results & Insights

- The **sample means distribution** follows a **bell curve**, confirming **CLT**.
- **Larger sample sizes** improve normality, showcasing **CLT’s dependence on n**.
- The **random walk problem** validates **CLT-based probability estimates** using **simulation**.
- The **percentiles vs. confidence intervals discussion** highlights key differences in **descriptive vs. inferential statistics** and the **role of CLT in statistical inference**.
