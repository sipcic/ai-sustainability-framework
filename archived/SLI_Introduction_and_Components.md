# 1. Introduction

Technological progress, particularly in **automation and artificial intelligence (AI)**, is rapidly reshaping the foundations of economic productivity and social organization. Global output continues to rise, yet indicators of **well-being, equality, and environmental stability** are increasingly decoupled from traditional measures of growth such as GDP or productivity per worker.  

This widening gap raises a fundamental question:  
> **Can we define and measure progress in a way that remains aligned with the sustainability of life itself?**

To address this question, we introduce the concept of a **Sustainable Life Index (SLI)** — a composite indicator designed to quantify the balance between **economic productivity, social inclusion, and ecological integrity**.  
The SLI links six interdependent variables, each representing a necessary pillar of sustainable life.

---

## 1.1 Components of the Sustainable Life Index

This section defines the six variables that compose the SLI framework. Each component is normalized (scaled between 0 and 1) relative to a desirable target level or sustainability boundary.

---

### (a) Employment Ratio – Economic Participation
Employment reflects the proportion of the labor force actively engaged in productive work.

$$
L_r = \frac{L}{L^*}
$$

where  
- $L$ = actual employment rate,  
- $L^*$ = target (full-employment) rate.  

A value $L_r \approx 1$ indicates high labor participation and economic inclusion. Lower values suggest under-utilized human capital.

---

### (b) Consumption Adequacy – Aggregate Demand
Consumption represents the fraction of national output (GDP) that translates into household demand.

$$
C_r = \frac{C}{Y}
$$

where  
- $C$ = household consumption,  
- $Y$ = total economic output (GDP).  

A stable $C_r$ ensures that production is matched by effective demand, avoiding structural stagnation.

---

### (c) Median Income Ratio – Distribution of Productivity Gains
Median real income reflects the purchasing power of the average worker.

$$
W_r = \frac{W}{W^*}
$$

where  
- $W$ = actual median real wage,  
- $W^*$ = target or living-wage benchmark.  

This term captures whether productivity improvements are transmitted to the median household.

---

### (d) Renewable Energy Share – Ecological Transition
Renewable share measures the fraction of total energy derived from renewable sources.

$$
R \in [0,1]
$$

A higher $R$ indicates progress toward decarbonization and energy sustainability. $R = 1$ represents full reliance on renewables.

---

### (e) Emission Burden – Environmental Cost
This term penalizes the system based on greenhouse-gas emissions relative to the allowable planetary budget.

$$
E_r = \frac{\text{CO}_2}{\text{CO}_2^{\text{budget}}}
$$

where  
- $\text{CO}_2$ = actual emissions,  
- $\text{CO}_2^{\text{budget}}$ = sustainable annual or cumulative carbon budget.  

Values $E_r > 1$ represent ecological overshoot.

---

### (f) Inequality Index – Social Cohesion
Inequality is expressed through the Gini coefficient or a comparable inequality metric.

$$
G \in [0,1]
$$

Higher $G$ indicates greater disparity in income distribution.  
For interpretive symmetry, $(1 − G)$ can be viewed as a measure of equality.

---

## 1.2 Modeling Sustainability: Additive vs. Multiplicative Formulations

Having defined the components, we now consider how they can be mathematically integrated into a single sustainability index. Two principal approaches are possible: **additive** and **multiplicative** formulations.

---

### (a) Additive Models

The **additive formulation** represents SLI as a *weighted linear combination* of normalized components:

$$
\text{SLI}_{\text{add}} =
\omega_1 L_r
+ \omega_2 C_r
+ \omega_3 W_r
+ \omega_4 R
- \omega_5 E_r
- \omega_6 G
$$

Each weight $\omega_i \ge 0$ quantifies the relative importance of its domain, with $\sum_i \omega_i = 1$.

**Advantages**
- Transparent and easy to interpret.  
- Suitable for empirical calibration and policy benchmarking.  
- Enables linear sensitivity analysis (e.g., $∂SLI/∂R$, $∂SLI/∂G$).  

**Limitations**
- Assumes perfect substitutability (gains in one area can offset losses elsewhere).  
- Lacks representation of thresholds or nonlinear tipping behavior.

---

### (b) Multiplicative Models

A multiplicative (geometric-mean) formulation captures **interdependence** and **non-compensability** among components:

$$
\text{SLI}_{\text{mult}} =
L_r^{\omega_1}
C_r^{\omega_2}
W_r^{\omega_3}
R^{\omega_4}
E_r^{\omega_5}
(1 − G)^{\omega_6}
$$

Here, strong performance in one domain cannot compensate for collapse in another (e.g., if $R → 0$, the index → 0).

**Advantages**
- Represents the “weakest-link” nature of sustainability.  
- Aligns with ecological models where system viability requires all components above critical thresholds.  

**Limitations**
- More complex calibration (weights act as elasticities).  
- Sensitive to normalization and data uncertainty.  
- Less intuitive for policy communication.

---

## 1.3 Choice of Framework for This Article

This paper adopts the **additive formulation** as the analytical baseline.  
The additive SLI serves as a first-order model for quantifying trade-offs between **automation, labor, and environmental integrity**. Its linearity facilitates direct sensitivity analysis and empirical implementation.  

Future work will explore **multiplicative** and **hybrid nonlinear models** that incorporate threshold effects, feedback loops, and irreversible ecological boundaries, extending the SLI toward a fully coupled systems framework.
