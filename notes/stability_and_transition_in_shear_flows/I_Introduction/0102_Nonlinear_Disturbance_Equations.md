## Nonlinear Disturbance Equations

For incompressible fluid, the equation governing the general evolution of fluid flow are known as the Navier-Stokes equations,
$$
\begin{align}
\frac{\partial u_i}{\partial t} = - u_j \frac{\partial u_i}{\partial x_j} - \frac{\partial p}{\partial x_i} + \frac{1}{\text{Re}} \nabla^2 u_i,\\
\frac{\partial u_i}{\partial x_i} = 0.
\end{align}
$$

Equation for the disturbance can be derived by considering a basic state $(U_i, P)$ and a perturbed state $(U_i+u'_i, P+p')$, both satisfying the Navier-Stokes equations. Subtracting the equations for the basic and perturbed state and omitting the primes for the disturbance quantities, we find the following **nonlinear disturbance equations**,
$$
\frac{\partial u_i}{\partial t} = - U_j \frac{\partial u_i}{\partial x_j}
$$

