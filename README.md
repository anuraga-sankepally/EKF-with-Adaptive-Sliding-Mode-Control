# State Estimation and Robust Control using Kalman Filter and Adaptive Sliding Mode Control

## Description  
This project demonstrates the integration of a **Kalman Filter** for state estimation and an **Adaptive Sliding Mode Controller (ASMC)** for robust control in the presence of wind disturbances. The system is designed to handle noisy measurements and external disturbances, making it suitable for applications in robotics, autonomous vehicles, and aerospace.

### Key Components:
1. **Kalman Filter**:  
   - Estimates the state of a dynamic system (e.g., position, velocity) based on noisy measurements.  
   - Handles process and measurement noise to provide accurate state estimates.  
   - Visualizes the true state, noisy measurements, and Kalman Filter estimates.  

2. **Adaptive Sliding Mode Controller (ASMC)**:  
   - Provides robust control in the presence of wind disturbances and model uncertainties.  
   - Uses a sliding surface to drive the system state to a desired trajectory.  
   - Adapts to changing conditions (e.g., varying wind disturbances) to maintain stability and performance.  

This project is ideal for those interested in **state estimation**, **robust control**, and **disturbance rejection**, and serves as a practical introduction to advanced control techniques.

## Demo  
Here’s a demo GIF showcasing the system in action:  

![demo_AdaptiveSMC GIF](./demo_AdaptiveSMC.gif)

*Note: If the GIF doesn't load, you can download it [here](./demo.gif).*

## Error Plots and 3-Sigma Bounds  
The following plots show the **error covariance** and **3-sigma bounds** for the estimated states over time. These plots help visualize the performance and uncertainty of the Kalman Filter.

![Error Covariance Plots](./err_cov_3sig_asmc.png)

# Error Covariance:

-The error covariance represents the uncertainty in the state estimates (North, East, and Down positions).

-Lower values indicate more accurate estimates, while higher values suggest increased uncertainty.

# 3-Sigma Bounds:

-The 3-sigma bounds define the confidence interval for the estimates. If the error stays within these bounds, the system is performing well.

-These bounds are derived from the Kalman Filter's covariance matrix and reflect the filter's reliability.

# System Performance:

-The plots demonstrate the system's ability to maintain accurate state estimates despite external disturbances (e.g., wind).

-The error remains within the 3-sigma bounds for most of the time, indicating robust performance and reliable state estimation.



## Packages Required  
To run this project, you’ll need the following Python packages:  
- `numpy`  
- `matplotlib`  
- `scipy`  

These packages are commonly used for numerical computations, visualization, and scientific computing.

## How to Run  

### 1. Open in Google Colab  
Click the link below to open the notebook directly in Google Colab:  
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1ZHbnG8qDobRliNeZJ2yeug6ak6jDQXeW#scrollTo=50XN6K6F3Kx_)
