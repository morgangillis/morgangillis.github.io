---
layout: post
title: The Quick Brown Fox Jumps Over the Lazy Dog The Quick Brown Fox Jumps Over the Lazy Dog
---

Macroscopic swimmers experience an interplay of forces vastly different than that of microscopic swimmers, even in the same fluid (a common example being water). The distinction between these two realms of fluid dynamics is frequently encapsulated in the relative size of a quantity dependent on the fluid parameters, known as the Reynolds number  Re, which is defined as

$$\text{Re} = \frac{\rho v L}{\mu}$$

where $\rho$ is the density of the fluid, $v$ is the swimmer’s speed relative to the fluid, $L$ is the length scale of the swimmer, and $\mu$ is the viscosity of the fluid. The usefulness of the Reynolds number for characterizing swimming behavior is that it grows large for large $L$ (macroscopic swimmers) and vanishes for small $L$ (microscopic swimmers).

One way it’s often put is that a large Reynolds number causes inertial forces to dominate for swimmers, while a small Reynolds number instead favors viscous forces. To see why this is the case, we consider one particular form of the Navier-Stokes equation, which governs incompressible fluids:
$$\mu\laplacian{\vectorbold{v}} - \grad{p} = \rho\pdv{\vectorbold{v}}{t} + \rho(\vectorbold{v} \cdot \grad)\vectorbold{v} ,$$
or, substituting $\rho = \text{Re}\mu / v L$,
$$\mu\laplacian{\vectorbold{v}} - \grad{p} = \frac{\text{Re}\mu}{v L} \left(\pdv{\vectorbold{v}}{t} + (\vectorbold{v} \cdot \grad)\vectorbold{v}\right)$$
where the left-hand side corresponds to viscous forces and something called hydraulic head (which is pretty much the fluid pressure), and the right-hand side represents contributions from inertia. When the Reynolds number is sufficiently small, the right-hand side approaches zero relative to the left-hand side, and we are left with a simplified expression involving only viscosity and pressure terms:
$$\mu\laplacian{\vectorbold{v}} = \grad{p} .$$

The inertial forces in the macroscopic case should be familiar to anyone who has spent time swimming or rowing: large, repeated strokes are able to give us enough momentum to glide through the water without slowing down significantly. Microscopic swimmers do not have this same luxury---instead, their world is dominated by viscous forces which require them to employ different propulsion strategies. One of the main consequences of low Reynolds number is that time-reversible motions, such as rowing motions, do very little to propel the swimmer in any given direction. This is because low inertia at the micro scale causes these motions to push swimmers as much in one direction as in the other, for a net zero effect. (This fact is often referred to as the scallop theorem.) I imagine it's something akin to a human trying to swim through a ball pit or a pool of beads, where the ``molecules'' of the fluid are much closer in scale to the human.

Thus, micro swimmers must use motions which are not time-reversible, such as sinusoidal flagellum-whipping or rotating a structure with chirality. A real-life example of the former kind is a sperm cell, which creates a sinusoidal wave with its flagellum in order to propel itself. Played in reverse, this sinusoidal wave would appear to travel in the opposite direction, allowing the sperm cell to use it successfully for swimming. The second kind appears in certain organisms which, for example, have helical tails that can spin. Because a helix possesses a specific chirality, spinning it one way will look distinct from spinning it the other way.

Researchers have attempted to replicate these sorts of micro-swimming strategies to create tiny drug carriers which can maneuver easily through bodily fluids. Specifically, they have looked into creating small devices which have chiral tails and can bind to specific drugs. While these devices don’t use anything near the intricacy of a helical tail, anything with some bit of chirality can get the job done. The researchers are able to steer these devices using an external magnetic field so that they can be directed, for instance, toward sites which need delivery of the drug being carried.
