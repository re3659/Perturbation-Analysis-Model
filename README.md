# Model-for-perturbation-analysis
This repository contains the code used in the master's thesis "Expanding a Stance Model to Scale Impulse and Analyze Passive Stability" by Joshua Goldberg. Featured is the model used for perturbation analysis. There is one code Jupyter Notebook code file (Working_model.ipynb), featuring four code blocks, and a folder (Data For Analysis) which houses the csv files used for analysis.
![Model](flySplayModel.png)

### Simulating the Models
These models can be simulated by choosing which models you want to run, setting the model masses, leg lengths, number of pairs of legs, and other anatomical values. It is also possible to show a video of each simulation, plot natural frequencies and periods, and select perturbation time and force. It isn't possible to run a perturbation sweep while running multiple models at once.

If choosing to run a parameter sweep, it is possible to set the factor (f) for parameter sweep step sizes. For example, a factor of 0.1 would mean that the model will be run with a perturbation force and time 1/10th of its maximum, and will iterate through until it reaches its maximum perturbation force and time. To analyze the results of parameter sweeps, the second code block can be used to store the data from the parameter sweep into a csv file, and the 3rd code block can be used to analyze the data from csv files. The 4th code block can be used to find how mass scales with leg length.

### Necessary Packages
MuJoCo must be installed in order to run this model. We have verified the code is compatible up to MuJoCo 3.7. Currently, MuJoCo only supports up through Python 3.13.

[https://github.com/deepmind/mujoco/releases](url)

### Associated Work
[1] Goldberg JD. Expanding a Stance Model to Scale Impulse and Analyze Passive Stability, In-proceedings
