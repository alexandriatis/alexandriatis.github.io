## Asset Tracking

[Data](data/hello_world.txt)

**Introduction:** The goal of this project is to learn about the numerics of MITgcm. Specifically, I look at the dynamics of the one-dimensional wave equation. A numerical solution for the simple second-order wave equation is compared to an MITgcm-style solution of the shallow water equations. The pressure method of MITgcm with Adams-Bashforth time stepping and finite difference spatial discretization is used to solve the shallow water equations with a linearized free surface. Simple initial conditions such as a Gaussian pulse and a Gaussian wave packet are simulated and compared. For details and references, a writeup of the project can be found in [andriatis_224_project.pdf](https://github.com/alexandriatis/Projects/blob/master/NUMERICAL_WAVES/andriatis_224_project.pdf).

### The 1-D Wave equation:

The 1-dimensional wave equation is a simple model ubiquitous in physics classes. Here, I solve the 1-D wave equation numerically for a Gaussian initial condition with a Dirichlet boundary condition on the left and a Neumann boundary condition on the right of the domain. For Matlab code see [wave1d_dist.m](https://github.com/alexandriatis/Projects/blob/master/NUMERICAL_WAVES/wave1d_dist.m).

<img src="movies/phi_pulse.mp4?raw=true"/>


### 1-D Surface Waves in MITgcm:

To learn about MITgcm, I solve the shallow water wave equations in one dimension using the pressure method with an implicit linear free surface. Here, a Gaussian initial condition propagates in a closed domain with constant water depth on the left and a linearly sloping bottom on the right. The bottom depth is not represented to scale; the maximum depth is `h=100` while the minimum depth is `h=5`. For Matlab code see [mit1d_dist.m](https://github.com/alexandriatis/Projects/blob/master/NUMERICAL_WAVES/mit1d_dist.m).

<img src="movies/eta_pulse_long.mp4?raw=true"/>
