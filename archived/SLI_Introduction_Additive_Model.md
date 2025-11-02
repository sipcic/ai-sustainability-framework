# 1. Introduction

Technological progress, particularly in **automation and artificial intelligence (AI)**, is rapidly reshaping the foundations of economic productivity and social organization. Global output continues to rise, yet indicators of **well-being, equality, and environmental stability** are increasingly decoupled from traditional measures of growth such as GDP or productivity per worker.  

This widening gap raises a fundamental question:  
> **Can we define and measure progress in a way that remains aligned with the sustainability of life itself?**

To address this question, we introduce the concept of a **Sustainable Life Index (SLI)** — a composite indicator designed to measure the equilibrium between **economic productivity, social inclusion, and ecological integrity**. The SLI links six interdependent variables:
- Employment (labor participation)  
- Consumption (aggregate demand adequacy)  
- Median income (income distribution)  
- Renewable energy share (ecological transition)  
- Carbon emissions (environmental cost)  
- Inequality (social cohesion)

---

## 1.1 Modeling Sustainability: Additive vs. Multiplicative Approaches

Formally representing sustainability requires combining these variables into a single function that can be evaluated and compared across scenarios. Two principal approaches exist:

### (a) Additive Models

The **additive formulation** expresses sustainability as a *weighted sum* of normalized components:

$$
\text{SLI}_{\text{add}} =
\omega_1 \frac{L}{L^*}
+ \omega_2 \frac{C}{Y}
+ \omega_3 \frac{W}{W^*}
+ \omega_4 R
- \omega_5 \frac{\text{CO}_2}{\text{CO}_2^{\text{budget}}}
- \omega_6 G
$$

Each term contributes linearly to the overall index, with its own weight $\omega_i$ representing relative importance.

**Advantages:**
- Simple and transparent — directly interpretable as a *weighted balance* of factors.  
- Suitable for comparative policy analysis (e.g., evaluating changes in employment, income, or emissions).  
- Easy to calibrate using real-world data and linear regression methods.  

**Limitations:**
- Implies **perfect substitutability**: improvements in one area can compensate for deterioration in another (e.g., higher income offsetting higher emissions).  
- Fails to represent **threshold effects** — such as irreversible environmental damage once carbon budgets are exceeded.  

---

### (b) Multiplicative Models

The **multiplicative formulation** combines normalized terms as products rather than sums:

$$
\text{SLI}_{\text{mult}} =
\left(\frac{L}{L^*}\right)^{\omega_1}
\left(\frac{C}{Y}\right)^{\omega_2}
\left(\frac{W}{W^*}\right)^{\omega_3}
R^{\omega_4}
\left(\frac{\text{CO}_2^{\text{budget}}}{\text{CO}_2}\right)^{\omega_5}
(1-G)^{\omega_6}
$$

This approach is conceptually closer to a **geometric mean**, emphasizing **interdependence** among variables: if one component collapses (e.g., $R \to 0$ or $G \to 1$), the entire index approaches zero.

**Advantages:**
- Captures the reality that sustainability dimensions are **non-compensatory** — strong performance in one cannot fully offset failure in another.  
- Aligns with systems and ecological models that emphasize *joint viability* of economic, social, and environmental subsystems.  

**Limitations:**
- More complex to calibrate and interpret (weights act as elasticities rather than linear coefficients).  
- Requires careful normalization (all inputs strictly positive and ≤1).  
- Less transparent for policymakers or non-technical readers.

---

## 1.2 Choice of Framework for This Article

This article focuses on the **additive formulation** of the Sustainable Life Index.  
The additive model provides a clear, first-order approximation that is analytically tractable and well-suited for:
- establishing conceptual relationships among automation, labor, and sustainability, and  
- performing **partial derivative analysis** to understand how changes in automation or energy policy affect the system.

Subsequent work will extend the model into **multiplicative** and **nonlinear hybrid forms**, where sustainability depends on the **joint survival** of all components — reflecting threshold effects, feedback loops, and irreversibility (e.g., climate tipping points).

The additive SLI thus serves as a **baseline framework** — a transparent starting point for quantifying the balance between **technological progress** and **the conditions that make life itself sustainable.**
