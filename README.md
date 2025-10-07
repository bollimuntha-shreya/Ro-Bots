# Robotics Projects Repository
Welcome to the **Ro-Bots** repository! These are projects I completed as part of the **Mobile Robotics** course. This collection showcases my work in robotics, computer vision, and sensor calibration. Each project is organized into its respective folder, containing all necessary code and resources.

## Table of Contents
- [ICP SLAM](#icp-slam-the-ro-bots)
- [Stereo Dense Reconstruction](#stereo-dense-reconstruction-the-ro-bots))
- [IMU Camera Calibration](#imu-camera-callibration-the-ro-bots)

---

## 1. Pose Graph Optimization for 2D SLAM

**Pose Graph Optimization for 2D Simultaneous Localization and Mapping (SLAM)**

### **Overview**
Implemented a 2D SLAM system utilizing pose graph optimization to accurately map environments and localize the robot within them. This project focuses on refining the robot's trajectory by optimizing the pose graph based on odometric and loop closure constraints.

### **Key Features**
- **Pose Graph Construction:** Built a graph where vertices represent robot poses and edges represent spatial constraints between poses, including odometry and loop closures.
- **Optimization Algorithms:** Applied nonlinear least squares optimization techniques to adjust the pose graph, minimizing errors and refining trajectory estimates.
- **Loop Closure Integration:** Incorporated loop closure detections to correct drift and enhance the accuracy of the global map.

### **Technologies & Tools**
- **Programming Languages:** Python
- **Libraries:** Open3D, NumPy, Matplotlib
- **Tools:** Jupyter Notebook, GitHub for version control

### **Outcomes**
- Achieved significant improvements in trajectory accuracy through effective pose graph optimization.
- Enhanced map consistency and reduced drift by integrating loop closure constraints.

### **Additional Documentation**
For a detailed explanation of the Iterative Closest Point (ICP) algorithm and its implementation in 3D-3D point cloud registration, refer to our [Notion page on Point Cloud Registration - ICP](https://saishubodh.notion.site/Point-Cloud-Registration-Iterative-Closest-Point-ICP-3D-3D-a25686ce1a11409d838d47bcac43ab4b).

---

## 2. Stereo Dense Reconstruction

**Stereo Vision for 3D Point Cloud Generation**

### **Overview**
Developed a dense 3D reconstruction pipeline using stereo vision techniques, leveraging the Semi-Global Block Matching (SGBM) algorithm to generate accurate disparity maps and detailed point clouds.

### **Key Features**
- **Disparity Map Computation:** Utilized OpenCV’s Semi-Global Block Matching (SGBM) to calculate disparity maps from rectified stereo image pairs.
- **3D Point Cloud Generation:** Transformed disparity maps into 3D point clouds using camera calibration parameters and baseline information.
- **Visualization & Registration:** Applied Open3D for visualizing and registering point clouds into a unified global frame based on ground truth poses.

### **Technologies & Tools**
- **Programming Languages:** Python
- **Libraries:** OpenCV, Open3D, NumPy, Matplotlib
- **Tools:** Jupyter Notebook, EVO for trajectory evaluation, GitHub for version control

### **Outcomes**
- Successfully reconstructed high-fidelity 3D models of environments, facilitating enhanced scene understanding.
- Conducted performance evaluation using EVO, demonstrating low trajectory error and precise roll-pitch-yaw estimations.

### **Additional Documentation**
For an in-depth overview of the Stereo Structure from Motion process, including implementation details and theoretical background, visit our [Notion page on Stereo Structure from Motion](https://saishubodh.notion.site/Stereo-Structure-from-Motion-9fdd81e4194f4803ac9ba7552df56470).

---

## 3. IMU Camera Calibration

**Inertial Measurement Unit (IMU) and Camera Sensor Fusion Calibration**

### **Overview**
Performed precise calibration of IMU and camera sensors to enable accurate sensor fusion for enhanced motion tracking and environmental perception.

### **Key Features**
- **Sensor Alignment:** Determined the spatial and temporal alignment between the IMU and camera sensors.
- **Calibration Algorithms:** Implemented calibration routines to estimate extrinsic parameters, ensuring synchronized and coherent data fusion.
- **Validation:** Verified calibration accuracy through motion estimation tasks and comparison with ground truth data.

### **Technologies & Tools**
- **Programming Languages:** Python
- **Libraries:** NumPy, OpenCV, SciPy
- **Tools:** Jupyter Notebook, GitHub for version control

### **Outcomes**
- Achieved high-precision calibration results, enabling reliable fusion of IMU and camera data.
- Enhanced the accuracy of motion tracking and 3D perception through effective sensor integration.
