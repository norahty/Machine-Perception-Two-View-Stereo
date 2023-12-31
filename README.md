# Machine-Perception-Project-Two-View-Stereo-Algorithm-Implementation
# Stereo 3D Reconstruction Project

## Overview

This project involved the development of a robust two-view stereo algorithm capable of transforming multiple 2D viewpoints into a comprehensive 3D reconstruction of a scene. The project required extensive work with Python and various associated libraries. Key features of this project included the utilization of the K3D library, enabling the visualization of 3D point clouds generated by the stereo algorithm. The project tasks were broken down as follows:

### Rectify Two View

The initial step encompassed the rectification of the two viewpoints. This process involved understanding the camera configuration, computing the right-to-left transformation, and determining the rectification rotation matrix. Although the rectification process drew from provided lecture slides, it demanded meticulous attention due to the clockwise rotation of the images in the dataset.

### Compute Disparity Map

Next, an algorithm was implemented to compute the disparity map. This task involved comparing patches using three distinct metrics: SSD (Sum of Squared Differences), SAD (Sum of Absolute Differences), and ZNCC (Zero-Mean Normalized Cross-Correlation). Kernel functions for each metric were crafted and applied to image patches.

### Compute Depth Map and Point Cloud

Following the acquisition of the disparity map, a function was developed to compute the depth map and point cloud. This enabled each pixel to store XYZ coordinates of the point cloud, enhancing the accuracy of the 3D reconstruction.

### Postprocessing

Several post-processing steps were introduced, including noise removal, depth map cropping, outlier removal from the point cloud, and transformation of the point cloud from the camera frame to the world frame.

### Visualization

Leveraging the K3D library, the reconstructed point cloud was visualized directly within the Jupyter notebook. The outcome was a detailed, interactive 3D reconstruction of the scene, originating from the initial 2D viewpoints.

### Multi-pair Aggregation

Finally, the project incorporated multiple view pairs for two-view stereo, culminating in the aggregation of the reconstructed point cloud in the world frame.
![K3D-sad](https://github.com/norahty/Machine-Perception-Project-Two-View-Stereo-Algorithm-Implementation/assets/94091909/58518e8e-92ec-4c89-974e-7009758fa55f)
![K3D-ssd](https://github.com/norahty/Machine-Perception-Project-Two-View-Stereo-Algorithm-Implementation/assets/94091909/575ab449-c3b1-4ceb-9dc3-90002b1de738)
![K3D-zncc](https://github.com/norahty/Machine-Perception-Project-Two-View-Stereo-Algorithm-Implementation/assets/94091909/c5355476-14ca-41d6-8618-aa81441a3d88)


## Project Conclusion

The pinnacle of this project was the successful creation of a fully reconstructed 3D point cloud of a temple. Screenshots of the reconstruction were captured, providing an interactive viewing experience. Overall, this project served as a valuable opportunity to delve deeply into machine perception and showcase proficiency in handling and interpreting complex datasets.
![K3D-aggregation](https://github.com/norahty/Machine-Perception-Project-Two-View-Stereo-Algorithm-Implementation/assets/94091909/76f691e3-71df-4e80-ad6f-9afbeda69548)

