## Introduction

### Introduction
```{prf:definition} Stability Theory
“Stability theory deals with the mathematical analysis of the evolution of disturbances superposed on a laminar base flow.” {cite}`schmidStabilityTransitionShear2001`
```

### Nonlinear Disturbance Equations

For incompressible fluid, the equation governing the general evolution of fluid flow are known as the Navier-Stokes equations,

$$
\begin{align}
\frac{\partial u_i}{\partial t} = - u_j \frac{\partial u_i}{\partial x_j} - \frac{\partial p}{\partial x_i} + \frac{1}{\text{Re}} \nabla^2 u_i,\\
\frac{\partial u_i}{\partial x_i} = 0.
\end{align}
$$

````{margin} 
```{admonition} *Why the basic state also satisfies Navier-Stokes equations?*
> “Stability theory deals with the mathematical analysis of the evolution of disturbances superposed on a laminar base flow.” {cite}`schmidStabilityTransitionShear2001`

Thus, in the laminar flow nonlinear term is negligible.
```
````

Equation for the disturbance can be derived by considering a basic state $(U_i, P)$ and a perturbed state $(U_i+u'_i, P+p')$, both satisfying the Navier-Stokes equations. Subtracting the equations for the basic and perturbed state, we find the following **nonlinear disturbance equations**,

$$
\begin{align}
    \frac{\partial u_i'}{\partial t} &= - U_j \frac{\partial u_i'}{\partial x_j} - u_j'\frac{\partial (U_i + u_i')}{\partial x_j} - \frac{\partial p'}{\partial x_i} + \frac{1}{\text{Re}} \nabla^2 u_i'\\
    \frac{\partial u_i'}{\partial x_i} & = 0
\end{align}
$$

Introduce kinetic energy of the disturbance contained in a volume $V$, 

$$
\begin{equation}
E_V = \frac{1}{2} \int_V u_iu_i \mathrm{d}V,
\end{equation}
$$

to measure development of an initial perturbation.


### Definition of Stability and Critical Reynolds Numbers

#### Definition of Stability

**Stability**

**Conditional Stability**

**Global Stability**

**Monotonic Stability**

#### Critical Reynolds Numbers

```{prf:definition} $\text{Re}_E$
For $\text{Re}< \text{Re}_E$ the flow is monotonically stable.
```

```{prf:definition} $\text{Re}_G$
For $\text{Re}< \text{Re}_G$ the flow is globally stable.
```

```{prf:definition} $\text{Re}_L$
For $\text{Re}> \text{Re}_L$ the flow is linearly unstable or not conditionally stable.
```
````{margin}
```{prf:definition} Bifurcation Analysis
[WorkingOn]
```
````

> “In region I, that is, for Re < ReE, all disturbances exhibit monotonic decay. Region II is characterized by global, but not necessarily monotonic stability. In this region, disturbances may grow, but they will ultimately decay as time evolves. For Re > Reo we can encounter instabilities. For Re between Reo and ReL we have a conditionally stable flow: for energies below the curve separating regions III and IV the disturbance will decay; for energies above this curve we observe instabilities. The intersection of this curve with the Re-axis defines the Reynolds number above which there exist instabilities of infinitesimal disturbances.” {cite}`schmidStabilityTransitionShear2001`




#### Spatial Evolution of Disturbances

### The Reynolds-Orr Equation

#### Derivation of the Reynolds-Orr Equation
```{prf:proof} **Reynolds-Orr Equation**

$$
\begin{align}
    \left[\frac{\partial u_i'}{\partial t} \right.=& \left.- U_j \frac{\partial u_i'}{\partial x_j} - u_j'\frac{\partial (U_i + u_i')}{\partial x_j} - \frac{\partial p'}{\partial x_i} + \frac{1}{\text{Re}} \nabla^2 u_i'\right] \times u_i'\\
    u_i'\frac{\partial u_i'}{\partial t} =& - \left(\frac{\partial \frac{1}{2}u_i'u_i' U_j}{\partial x_j} - 0\right) - u_i'u_j'\frac{\partial U_i}{\partial x_j} -\left(\frac{\partial  \frac{1}{2}u_i'u_i'u_j'}{\partial x_j} - 0\right) \\
    &- \left(\frac{\partial p'u_i'}{\partial x_i} - 0\right) + \frac{1}{\text{Re}} \left(\frac{\partial}{\partial x_j}\left(u_i'\frac{\partial u_i'}{\partial x_j}\right) -\frac{\partial u_i'}{\partial x_j}\frac{\partial u_i'}{\partial x_j}\right)\\
    \int_V\left[ \frac{\partial \frac{1}{2}u_i'u_i'}{\partial t} \right. = & - u_i'u_j'\frac{\partial U_i}{\partial x_j} - \frac{1}{\text{Re}}\frac{\partial u_i'}{\partial x_j}\frac{\partial u_i'}{\partial x_j}+ \frac{\partial }{\partial x_j}\left( - \frac{1}{2}u_i'u_i' U_j - \frac{1}{2}u_i'u_i'u_j'\right.\\
    & \left.\left. -u_ip\delta_{ij} + \frac{1}{\text{Re}}u_i'\frac{\partial u_i'}{\partial x_j}\right)\right] \mathrm{d}V\\
    \frac{\mathrm{d} E_V}{\mathrm{d} t} = & - \int_V u_i'u_j'\frac{\partial U_i}{\partial x_j}\mathrm{d}V - \frac{1}{\text{Re}}\int_V\frac{\partial u_i'}{\partial x_j}\frac{\partial u_i'}{\partial x_j}\mathrm{d}V
\end{align}
$$
```



#### The Need for Linear Growth Mechanisms
The instantaneous growth rate, $\frac{1}{E_V}\frac{\mathrm{d}E_V}{dt}$, is independent of the disturbance amplitude.

> “instantaneous growth rate of a finite-amplitude disturbance is given by mechanisms that are present in the linearized equations, and the total growth of a finite-amplitude disturbance can be regarded as a sum of growth rates associated with the linear mechanisms.” {cite}`schmidStabilityTransitionShear2001`