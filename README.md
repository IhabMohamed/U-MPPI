# U-MPPI

This repository contains the ROS implementation of the U-MPPI control strategy, a novel methodology that enhances the classical sampling-based **Model Predictive Path Integral [(MPPI)](https://arc.aiaa.org/doi/pdf/10.2514/1.G001921)** algorithm by combining the `Unscented Transform (UT)` with `standard optimal control theory` to effectively manage system uncertainties while integrating a more efficient trajectory sampling strategy. 

Such a control strategy leverages the UT to propagate not only the mean but also the covariance of the system dynamics (as demonstrated in the following gif), going beyond the traditional MPPI method. As a result, it introduces a novel and more efficient trajectory sampling strategy, significantly enhancing state-space exploration and ultimately reducing the risk of being trapped in local minima. Furthermore, by leveraging the uncertainty information provided by UT, we incorporate a risk-sensitive cost function that explicitly accounts for risk or uncertainty throughout the trajectory evaluation process, resulting in a more resilient control system capable of handling uncertain conditions.

<img src="media/sampling-strategy.gif" width="500" height="300"/>

## Paper:

Ihab S. Mohamed, Junhong Xu, Gaurav S Sukhatme, Lantao Liu "Towards Efficient MPPI Trajectory Generation with Unscented Guidance: U-MPPI Control Strategy." arXiv preprint arXiv:2306.12369 (2023).

Paper: https://arxiv.org/abs/2306.12369 OR https://ieeexplore.ieee.org/abstract/document/10824881

Bibtex:
```
@article{mohamed2025towards,
  title={Towards efficient MPPI trajectory generation with unscented guidance: U-MPPI control strategy},
  author={Mohamed, Ihab S and Xu, Junhong and Sukhatme, Gaurav S and Liu, Lantao},
  journal={IEEE Transactions on Robotics},
  year={2025},
}
```

## Media:
**Video**: https://youtu.be/1xsh4BxIrng

## ROS Packages:

We will upload the complete project as soon as we finish polishing and upgrading the base code. In the meantime, please refer to our repository, namely [log-MPPI_ros](https://github.com/IhabMohamed/log-MPPI_ros), which serves as our baseline. Please follow the installation instructions there if you haven't already done so :wink:

### Primary code maintainer:
Ihab S. Mohamed and Junhong Xu (e-mail: {mohamedi, xu14}@iu.edu)\
Vehicle Autonomy and Intelligence Lab ([VAIL](https://vail.sice.indiana.edu/))\
Indiana University - Bloomington, USA



