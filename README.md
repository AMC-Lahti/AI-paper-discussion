# AI-paper-discussion
Memo for weekly AI paper discussion

## [2024-09-27](slides/2024-09-27.pdf)
Graph Neural Networks for temporal graphs: State of the art, open challenges, and opportunities

- https://doi.org/10.48550/arXiv.2302.01018
- Methods for snapshot-based GNN: model evolution / embedding evolution


## 2024-10-11
Spectral Temporal Graph Neural Network for Multivariate Time-series Forecasting

- https://doi.org/10.48550/arXiv.2103.07719
- A combine of GFT and DFT of both inter-serial and intra-serial spectral knowledge
- Attention for detect graph structure

## 2024-10-25

PHYMPGN: PHYSICS-ENCODED MESSAGE PASSING GRAPH NETWORK FOR SPATIOTEMPORAL PDE SYSTEMS

- https://doi.org/10.48550/arXiv.2410.01337
- For PDE/ODE system, to find y(t1) = G(y(t0)), y(t1) = y(t0) + intergal of y'(t) between t0 and t1. y'(t) is a function of system state of time t, i.e, y'(t) = F(y(t)).
- Numerical methods (Runge-Kutta) to approximate integral, so we only need to find y'(t) = F(y(t)), instead of find y(t1) = G(y(t0)).

## [2024-11-01](slides/2024-11-01.pdf)

Scalable and Consistent Graph Neural Networks for Distributed Mesh-based Data-driven Modeling

- https://doi.org/10.48550/arXiv.2103.07719
- Neural message passing across different compute node to scale GNN to billions of nodes

## [2024-11-08](slides/2024-11-08.pdf)

Parameter estimation and modeling of nonlinear dynamical systems based on Runge–Kutta physics-informed neural network

- [https://](https://doi.org/10.1007/s11071-023-08933-6)[doi.org](https://doi.org/10.1007/s11071-023-08933-6)[/10.1007/s11071-023-08933-6](https://doi.org/10.1007/s11071-023-08933-6)
- Neural ODE + RK4 as ODE solver
- Physical loss: output gradient wrt input should be consistent

## [2025-02-14](slides/2025-02-14.pdf)

Training stiff neural ordinary differential equations in data-driven wastewater process modelling

- https://doi.org/10.1016/j.compchemeng.2005.11.008
- Normalization using mean of y and dy/dt on input and output of network
- Use smoothed regression of y and dy/dt to pretrain the network, help later Neural ODE training converge faster.