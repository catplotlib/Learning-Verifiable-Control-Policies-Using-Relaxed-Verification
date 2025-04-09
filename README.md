# Learning-Verifiable-Control-Policies-Using-Relaxed-Verification

## Parameter Visualizer

![Combined controller comparison showing CROWN and gradient-based approaches for both neural network and linear controllers](images/combined.png)

A unified controller verification notebook that compares different control strategies.

The visualizer (`Visualizer/Parameter_Visualiser.ipynb`) provides:
- CROWN-based verification for linear and neural network controllers
- Gradient-based verification for linear and neural network controllers
- Visualization of reachable sets and sample trajectories

The tool loads pre-trained controllers from:
- `crown_*.pkl`: CROWN-verified controllers
- `gradient_*.pkl`: Gradient-based controllers

Results are saved as plots (e.g., `unicycle_navigation_crown_linear.png`) for analysis.

## Invariant Set Training and Verification

![Unicycle navigation with invariant set highlighted](images/invariant.png)

An approach that explicitly trains neural network controllers to induce invariant behavior:


**Definition**: An invariant set $S$ is a region where once a system enters, it remains forever:

$$x_t \in S \implies x_{t+1} = f(x_t) \in S \text{ for all } t \geq 0$$

The notebook (`Invariant_Set_Training_for_Safe_Unicycle_Navigation.ipynb`) demonstrates:
- Training neural network controllers with invariance objectives
- Visualizing and verifying the resulting invariant regions
- Evaluating the controller's reach-avoid performance with safety guarantees