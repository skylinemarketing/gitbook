---
description: Use W&B Sweeps to manage hyperparameter search and hyperparameter optimization
---

# Sweeps Overview

Automate hyperparameter optimization and exploration with Sweeps.

### Benefits of using W&B Sweeps 

1. **Quick setup**: With just a few lines of code you can run W&B sweeps.
2.  **Transparent**: We cite all the algorithms we're using, and [our code is open source](https://github.com/wandb/client/tree/master/wandb/sweeps).
3. **Powerful**: Our sweeps are completely customizable and configurable. You can launch a sweep across dozens of machines, and it's just as easy as starting a sweep on your laptop.

### Common Use Cases

1. **Explore**: Efficiently sample the space of hyperparameter combinations to discover promising regions and build an intuition about your model.
2. **Optimize**:  Use sweeps to achieve the next level of model performance.

### Approach

1. **Add wandb**: In your Python script, add a couple lines of code to log hyperparameters and output metrics from your script. [Get started now →](quickstart.md)
2.  **Write config**: Define the variables and ranges to sweep over. Pick a search strategy— we support grid, random, and Bayesian search, as well as early stopping.
3. **Initialize sweep**: Launch the sweep server. We host this central controller and coordinate between the agents that execute the sweep.
4. **Launch agent\(s\)**: Run this command on each machine you'd like to use to train models in the sweep. The agents ask the central sweep server what hyperparameters to try next, and then they execute the runs.
5. **Visualize results**: Open our live dashboard to see all your results in one central place.

![](../../.gitbook/assets/central-sweep-server-3%20%281%29.png)

{% page-ref page="quickstart.md" %}

{% page-ref page="add-to-existing.md" %}

{% page-ref page="../configuration.md" %}

{% page-ref page="../local-controller.md" %}

{% page-ref page="../python-api.md" %}

