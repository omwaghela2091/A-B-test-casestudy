# 🦸‍♂️ A/B Testing Case Study: Superhero Masterclass Conversion Optimization

Ever dreamed of becoming a superhero?

At our **Superhero Masterclass Agency**, we connect aspiring heroes with real mentors — from tech-savvy vigilantes to intergalactic warriors, even legends from Temu! Our website boldly asks:

> *"Want to be a superhero?"*

To guide users toward their transformation journey, we offer two clear options:
1. **Enroll Now!**
2. **Secure Free Trial**

But which of these call-to-action buttons leads to more clicks? That’s the core question behind this A/B testing case study. In this project, we dive deep into data to discover which message resonates more and drives higher user engagement.

---

## 🧪 Objective

To determine whether the "Enroll Now!" button or the "Secure Free Trial" button results in a higher **Click-Through Rate (CTR)**. The test aims to evaluate:
- **Statistical significance**: Is the difference in performance real or just due to random chance?
- **Practical significance**: Is the improvement meaningful enough to act on?

---

## 🧠 Hypotheses

- **Null Hypothesis (H₀)**: The click-through rates for both buttons are the same (p_con = p_exp).
- **Alternative Hypothesis (H₁)**: The click-through rates are different (p_con ≠ p_exp).

---

## 🔧 Tools & Libraries Used

- **Python** (data manipulation & analysis)
- **Pandas** (data wrangling)
- **NumPy** (numerical operations)
- **Matplotlib & Seaborn** (visualizations)
- **SciPy** (statistical testing)

---

## 📁 Dataset Overview

Each row in the dataset represents a user session. Key columns include:
- `user_id`: Unique user identifier
- `click`: Binary indicator of whether the button was clicked
- `group`: "control" (Enroll Now) or "experiment" (Secure Free Trial)
- `timestamp`: Time of interaction

---

## 📊 Analysis Steps

1. **Data Loading & Inspection**
   - Read data from CSV
   - Checked distribution of clicks across groups

2. **Visual Exploration**
   - Grouped bar chart showing click vs no-click by variant
   - Annotated with percentage labels for easy comparison

3. **Z-Test for Proportions**
   - Computed sample proportions and pooled click probability
   - Calculated standard error, test statistic, and p-value
   - Visualized the rejection region on the standard normal distribution

4. **Confidence Interval**
   - Calculated 95% confidence interval for difference in proportions

5. **Practical Significance**
   - Compared confidence interval to predefined **Minimum Detectable Effect (MDE = 0.1)**

---

## 📈 Results Summary

- **Z-test statistic**: -59.44  
- **p-value**: < 0.001  
- **95% Confidence Interval**: [0.399, 0.426]  
- **Conclusion**:
  - ✅ **Statistically significant**
  - ❌ **Not practically significant** (based on MDE = 0.1)

---

## 🧠 What I Demonstrated
- How to run and interpret a full A/B test from hypothesis to conclusion
- Application of core statistical concepts including p-values, confidence intervals, and effect sizes
- Use of Python libraries to visualize and compute metrics for real-world experiments
- Distinction between statistical and **practical** significance in decision-making
