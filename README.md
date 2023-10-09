# U-MPPI

This repository contains the ROS implementation of the U-MPPI control strategy, a novel methodology that enhances the classical sampling-based **Model Predictive Path Integral [(MPPI)](https://arc.aiaa.org/doi/pdf/10.2514/1.G001921)** algorithm by combining the `Unscented Transform (UT)` with `standard optimal control theory` to effectively manage system uncertainties while integrating a more efficient trajectory sampling strategy. 

Such a control strategy leverages the UT to propagate not only the mean but also the covariance of the system dynamics (as demonstrated in the following gif), going beyond the traditional MPPI method. As a result, it introduces a novel and more efficient trajectory sampling strategy, significantly enhancing state-space exploration and ultimately reducing the risk of being trapped in local minima. Furthermore, by leveraging the uncertainty information provided by UT, we incorporate a risk-sensitive cost function that explicitly accounts for risk or uncertainty throughout the trajectory evaluation process, resulting in a more resilient control system capable of handling uncertain conditions.

<img src="media/sampling-strategy.gif" width="500" height="300"/>

## Media:
**Video**: https://youtu.be/et9t8X1wHKI OR https://youtu.be/yDBaRLvAejk.

## ROS Packages:

The entire project will be uploaded soon; however, we are currently referring to our related repositories for the baselines [(namely, MPPI and log-MPPI)](https://github.com/IhabMohamed/log-MPPI_ros) and [GP perception model](https://github.com/mahmoud-a-ali/vsgp_pcl).


### Primary code maintainer:
Ihab S. Mohamed and Mahmoud Ali (e-mail: {mohamedi, alimaa}@iu.edu)\
Vehicle Autonomy and Intelligence Lab ([VAIL](https://vail.sice.indiana.edu/))\
Indiana University - Bloomington, USA



