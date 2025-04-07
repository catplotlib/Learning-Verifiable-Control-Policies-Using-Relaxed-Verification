# Learning-Verifiable-Control-Policies-Using-Relaxed-Verification

## Parameter Visualizer

A unified controller verification  notebook that compares different control strategies.

The visualizer (`Visualizer/Parameter_Visualiser.ipynb`) provides:
- CROWN-based verification for linear and neural network controllers
- Gradient-based verification for linear and neural network controllers
- Visualization of reachable sets and sample trajectories

The tool loads pre-trained controllers from:
- `crown_*.pkl`: CROWN-verified controllers
- `gradient_*.pkl`: Gradient-based controllers

Results are saved as plots (e.g., `unicycle_navigation_crown_linear.png`) for analysis.
