## 3.3 Sensitivity Analysis — Local Effects of AI

Sensitivity analysis in the SLI framework examines **how small, isolated changes in a single variable** influence the overall sustainability state.  
This provides insight into which components of the system are most responsive—or most fragile—under AI-driven change.

Let the Sustainable Life Index be expressed as a function of its six principal components:

$$
\text{SLI} = f(L_r, C_r, W_r, R, E_r, G)
$$

where  

| Symbol | Description |
|---------|--------------|
| $L_r$ | Employment rate (labor participation ratio) |
| $C_r$ | Consumer demand or consumption ratio |
| $W_r$ | Wage equity ratio (fair income distribution) |
| $R$ | Renewable energy capacity or share |
| $E_r$ | Environmental resilience indicator |
| $G$ | Inequality or governance index (inverse measure of equity) |

For compactness, these components are represented as  
$$
x_i \in \{L_r, C_r, W_r, R, E_r, G\}.
$$

### Local Sensitivity to AI

Each component $x_i$ can itself depend on the intensity or adoption level of AI, denoted $A$.  
The **local sensitivity** of SLI to AI is then defined by the partial derivative:

$$
\frac{\partial \text{SLI}}{\partial A}
   = \sum_i \frac{\partial \text{SLI}}{\partial x_i}
     \frac{\partial x_i}{\partial A}.
$$

Here:

- $\frac{\partial \text{SLI}}{\partial x_i}$ measures how much SLI changes when a specific sustainability component varies, assuming all others remain fixed.  
- $\frac{\partial x_i}{\partial A}$ captures how strongly AI affects that component (for example, how automation shifts $L_r$ or how AI-driven energy optimization improves $R$).  
- Their product reflects the **localized contribution of AI** through that variable to the system’s overall sustainability.

Together, these terms describe the **instantaneous direction and magnitude** of AI’s influence, forming the **local gradient field** that drives SLI dynamics.

### Relation to Dynamic Equilibrium

While the **total derivative**

$$
\frac{d(\text{SLI})}{dt}
  = \sum_i \frac{\partial \text{SLI}}{\partial x_i}\frac{dx_i}{dt}
$$

captures how SLI actually evolves over time as all components co-change,  
the **partial derivatives** $\frac{\partial \text{SLI}}{\partial x_i}$ represent its **local sensitivities**—the individual “pushes” that each subsystem contributes.

Dynamic equilibrium, defined by $d(\text{SLI})/dt \approx 0$, is achieved when these localized influences balance such that their net temporal effect cancels out.  

In practice, equilibrium implies that **the sum of AI-induced positive and negative local sensitivities stabilizes the system**, yielding a sustainable trajectory where productivity, equity, and environmental health evolve in concert.
