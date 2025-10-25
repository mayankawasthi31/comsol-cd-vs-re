# Project-III: Simulation of uniform flow past a sphere

Consider a flow of an incompressible, viscous fluid (density $\rho$, viscosity $\mu$) around a sphere of radius $a$ placed in a uniform stream $U$. The fluid will exert a drag force on the sphere, which is denoted as, say, $F_D$. The drag coefficient, defined as the drag force nondimensionalized by $\rho U^2/2$ and the projected area $\pi a^2$, is $C_D = F_D / (\rho U^2 \pi a^2 / 2)$.

Simulate the flow around the sphere using computational fluid dynamics (CFD) software such as ANSYS, COMSOL or OpenFOAM (your choice). Plot the variation of drag coefficient ($C_D$) as a function of the Reynolds number ($Re$) in the range of $Re = 0.01 - 100$. Clearly indicate how to compute the drag force from the results of the velocity and pressure field ($\mathbf{v}, p$) that the CFD package will give as output.

For small values of the Reynolds number ($Re \ll 1$), the drag force may be found analytically and has the expression:

$$
F_D = F_{D,s} \{1 + \frac{3}{8}Re + \frac{9}{40}Re^2(\log Re + \gamma + \frac{5}{6}\log 2 - \frac{323}{360}) + \frac{27}{80}Re^3 \log Re + O(Re^4)\}
$$

where $F_{D,s} = 6\pi\mu U a$ is the Stoke's drag and $\gamma = 0.57721$ is Euler's constant. Compare the simulated results for $C_D$ with the above analytical result (after writing it in terms of $C_D$ instead of $F_D$).

---

## Final Report Requirements

In your final report, you have to clearly outline the equations, boundary conditions, the domain chosen for the numerical simulation, mesh size and type, along with mesh-independence test.
