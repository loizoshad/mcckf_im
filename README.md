# MCCKFuIM: Maximum Correntropy Criterion Kalman Filter for Indoor Quadrotor Navigation under Intermittent Measurements

This repository contains the source-code developed and used to generate all the results in the research paper MCCKFuIM

If you use our code or data in your work, please cite our research paper:

    @inproceedings{
        hadjiloizou202Maximum,
        title = {Maximum Correntropy Criterion Kalman Filter for Indoor Quadrotor Navigation under Intermittent Measurements},
        author = {Hadjiloizou, Loizos and Makridis, Evagoras and Deliparaschos, Kyriakos  and Charalambous, Themistoklis},
        booktitle = {IEEE Mediterranean Conference on Control and Automation (MED)},
        year = {2023},
        pages = {170--175}
    }

> **Abstract**: We present a multisensor fusion framework for the onboard real-time navigation of a quadrotor in an indoor environment. The framework integrates sensor readings from an Inertial Measurement Unit (IMU), a camera-based object detection algorithm, and an Ultra-WideBand (UWB) localisation system. Often the sensor readings are not always readily available, leading to inaccurate pose estimation and hence poor navigation performance. To effectively handle and fuse sensor readings, and accurately estimate the pose of the quadrotor for tracking a predefined trajectory, we design a Maximum Correntropy Criterion Kalman Filter (MCC-KF) that can manage intermittent observations. The MCC-KF is designed to improve the performance of the estimation process when is done with a Kalman Filter (KF), since KFs are likely to degrade dramatically in practical scenarios in which noise is non-Gaussian (especially when the noise is heavy-tailed). To evaluate the performance of the MCC-KF, we compare it with a previously designed Kalman filter by the authors. Through this comparison, we aim to demonstrate the effectiveness of the MCC-KF in handling indoor navigation missions. The simulation results show that our presented framework offers low positioning errors, while effectively handling intermittent sensor measurements.

## Dependencies

* Ubuntu 20.04 LTS
* ROS Noetic
* Webots

## Demo

* roslaunch demo.launch
* rosrun mcc_kf path_generator.py


This project is released under a GPLv3 license
