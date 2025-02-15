# AI-paper-discussion
Memo for weekly AI paper discussion

## 2024-09-27
Graph Neural Networks for temporal graphs: State of the art, open challenges, and opportunities
- paper: https://doi.org/10.48550/arXiv.2302.01018, [slide](slides/2024-09-27_gnn.pdf)
- Methods for snapshot-based GNN: model evolution / embedding evolution


## 2024-10-11
Spectral Temporal Graph Neural Network for Multivariate Time-series Forecasting
- paper: https://doi.org/10.48550/arXiv.2103.07719
- A combine of GFT and DFT of both inter-serial and intra-serial spectral knowledge
- Attention for detect graph structure

## 2024-10-25
PHYMPGN: PHYSICS-ENCODED MESSAGE PASSING GRAPH NETWORK FOR SPATIOTEMPORAL PDE SYSTEMS
- paper: https://doi.org/10.48550/arXiv.2410.01337
- For PDE/ODE system, to find y(t1) = G(y(t0)), y(t1) = y(t0) + intergal of y'(t) between t0 and t1. y'(t) is a function of system state of time t, i.e, y'(t) = F(y(t)).
- Numerical methods (Runge-Kutta) to approximate integral, so we only need to find y'(t) = F(y(t)), instead of find y(t1) = G(y(t0)).

## 2024-11-01
Scalable and Consistent Graph Neural Networks for Distributed Mesh-based Data-driven Modeling
- paper: https://doi.org/10.48550/arXiv.2103.07719, [slide](slides/2024-11-01_distributed.pdf)
- Neural message passing across different compute node to scale GNN to billions of nodes

## 2024-11-08
Parameter estimation and modeling of nonlinear dynamical systems based on Runge–Kutta physics-informed neural network
- paper: https://doi.org/10.1007/s11071-023-08933-6, [slide](slides/2024-11-08_RK-PINN.pdf)
- Neural ODE + RK4 as ODE solver
- Physical loss: output gradient wrt input should be consistent

## 2025-02-14
Training stiff neural ordinary differential equations in data-driven wastewater process modelling
- paper: https://doi.org/10.1016/j.compchemeng.2005.11.008, [slide](slides/2025-02-14_coll.pdf)
- Normalization using mean of y and dy/dt on input and output of network
- Use smoothed regression of y and dy/dt to pretrain the network, help later Neural ODE training converge faster.


## Contribute

Start a new [pull request](https://github.com/AMC-Lahti/AI-paper-discussion/pulls)

Checklist:
- [ ] Include a [DOI link](https://library.centre.edu/citing_sources/DOI) to the paper in the slides
- [ ] Only upload a pdf copy of the slides, do not upload papers (https://github.com/AMC-Lahti/AI-paper-discussion/issues/1)
- [ ] Update README with links to paper and slides
