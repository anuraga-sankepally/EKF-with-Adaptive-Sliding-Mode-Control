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

![Error Covariance Plots](./error_cov_plots_kf.png)

### Explanation of the Plots:
- **Error Covariance (\(P\))**: The plots show the error covariance for different states (e.g., position, velocity) over time. The error covariance represents the uncertainty in the Kalman Filter's estimates.
- **3-Sigma Bounds**: The shaded regions represent the **3-sigma bounds**, which indicate the confidence interval for the estimates. If the errors stay within these bounds, the filter is performing well.
- **States Tracked**: The states include position (\(x\)), velocity (\(v\)), and other relevant variables. Each plot corresponds to a specific state, showing how the error and uncertainty evolve over time.

## Control Performance  
The following plots show the performance of the **Adaptive Sliding Mode Controller (ASMC)** in the presence of wind disturbances:

![Control Performance Plots](./control_performance_plots.png)

### Explanation of the Plots:
- **Sliding Surface**: The controller drives the system state to the sliding surface, ensuring robustness against disturbances.
- **Control Input**: The control input adapts to wind disturbances, maintaining stability and performance.
- **State Trajectory**: The system state converges to the desired trajectory despite the presence of disturbances.

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
