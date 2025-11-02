## 🔷 Practical Implications

- The **multiplicative model** is more sensitive near boundaries (e.g., when one component is near zero).  
- A small deterioration in a weak area (say $L_r$ or $R$) has **disproportionate impact** on total sustainability.  
- Unlike the additive model, sensitivity here is **state-dependent** — it changes dynamically with the system’s current configuration.  

---

## 🔷 Summary Table

| **Model Type** | **Composite Sensitivity Function** | **Interpretation** |
|----------------|------------------------------------|--------------------|
| **Additive** | $S_A = \sum_i \omega_i \frac{\partial x_i}{\partial A}$ | Linear sum of direct effects |
| **Multiplicative** | $S_A = \text{SLI}_{mult} \sum_i \omega_i \frac{1}{x_i} \frac{\partial x_i}{\partial A}$ | Weighted sum of elasticities — nonlinear, state-dependent |
