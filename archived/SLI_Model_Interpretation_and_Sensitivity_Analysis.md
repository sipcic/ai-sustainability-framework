# 3. Model Interpretation and Sensitivity Analysis

This section explores how the **Sustainable Life Index (SLI)** behaves under different economic and environmental conditions, and how each component influences the overall outcome. It bridges theoretical formulation and policy interpretation, showing how SLI serves as a dynamic tool for understanding the trade-offs between technological progress, social equity, and environmental sustainability.

---

## 3.1 Functional Behavior of SLI Components

Each variable in the SLI contributes positively or negatively to the index, depending on its direction of influence on sustainability.

- **Employment ratio ($L_r$):** Higher employment increases SLI, reflecting inclusive economic participation.  
- **Consumption adequacy ($C_r$):** A stable ratio indicates balanced demand and production, supporting sustainable growth.  
- **Median income ratio ($W_r$):** Rising median wages strengthen SLI by distributing productivity gains equitably.  
- **Renewable share ($R$):** Expansion of renewables directly enhances ecological sustainability.  
- **Emission burden ($E_r$):** Higher emissions reduce SLI, capturing environmental cost.  
- **Inequality ($G$):** Greater inequality weakens social cohesion and lowers SLI.

The relative importance of these effects depends on the weighting coefficients ($\omega_i$), which reflect policy priorities or societal values.

---

## 3.2 Sensitivity and Elasticity Analysis

**Sensitivity analysis** examines how small changes in each component affect the overall SLI value. This approach is **independent of model type**, though the mathematical form of sensitivity differs between additive and multiplicative models.

### Additive Model Sensitivity

For the additive formulation:
$$
\text{SLI}_{\text{add}} = \sum_i \omega_i x_i
$$

the sensitivity with respect to each variable is constant:
$$
\frac{\partial \text{SLI}}{\partial x_i} = \omega_i
$$

Thus, a one-unit change in any variable contributes directly in proportion to its weight. This linearity makes the additive model simple to interpret and calibrate.

### Multiplicative Model Elasticity

For the multiplicative formulation:
$$
\text{SLI}_{\text{mult}} = \prod_i x_i^{\omega_i}
$$

the relative sensitivity (elasticity) is state-dependent:
$$
\frac{\partial \text{SLI}}{\partial x_i} = \omega_i \frac{\text{SLI}_{\text{mult}}}{x_i}
$$

A 1% change in variable $x_i$ results in a $\omega_i$% change in SLI, meaning the influence of each factor depends on its current level. Variables near zero have disproportionately large impacts — a reflection of systemic fragility.

> **Interpretation:** Sensitivity analysis applies universally across model types; in the additive model, sensitivities are constant, whereas in multiplicative models they vary with state variables.

---

## 3.3 Equilibrium and Trade-Off Scenarios

The SLI framework enables exploration of **trade-offs** among its components — for example, between automation and employment, or between energy transition and economic inequality.

- **Case 1 – Automation and Labor:** Increased automation may raise productivity but reduce employment ($L_r$), lowering SLI unless offset by wage growth or retraining policies.  
- **Case 2 – Energy Transition:** Expanding renewables ($R$) boosts SLI, but if accompanied by higher inequality ($G$) or consumption emissions ($E_r$), net sustainability may still fall.  
- **Case 3 – Balanced Growth:** When gains in income and renewables occur alongside reductions in emissions and inequality, SLI increases across both formulations, reflecting genuine progress.

These scenarios highlight SLI’s role as a **policy compass**: it quantifies how competing objectives interact in shaping long-term sustainability.

---

## 3.4 Dynamic Simulation Framework

The SLI can also be modeled as a **time-dependent function** to study sustainability trajectories:

$$
\text{SLI}_t = f(L_t, C_t, W_t, R_t, E_t, G_t)
$$

The rate of change over time is given by:
$$
\frac{d(\text{SLI})}{dt} = \sum_i \frac{\partial \text{SLI}}{\partial x_i} \frac{dx_i}{dt}
$$

This formulation captures **sustainability momentum** — how quickly the system improves or deteriorates under policy or technological shifts.

Dynamic simulation of the SLI over time enables scenario comparison, such as:  
- Rapid automation with slow renewable adoption,  
- Inclusive green transition with equitable income growth, or  
- Carbon-intensive recovery with widening inequality.

---

## 3.5 Policy Interpretation

From a policy perspective, the SLI provides a **systemic early-warning mechanism**. Declining values signal unsustainable trajectories — either from ecological overshoot, social inequity, or underemployment.

- **Additive model:** Indicates incremental progress and trade-offs; improvements in one domain can offset declines in another.  
- **Multiplicative model:** Reflects **systemic coherence**; it remains high only when all pillars — employment, fair income, demand, clean energy, and equality — are simultaneously strong. Weakness in any one area lowers the overall index, reflecting the interdependence of social and ecological sustainability.

Together, these interpretations make the SLI a bridge between economic modeling and sustainability policy, suitable for empirical calibration, comparative analysis, and forward simulation.

---
