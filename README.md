# Lidar maps for KITTI Odometry Benchmark Suite

The KITTI dataset does not contain prebuilt map. We, as well as the authors of the other approaches, reconstruct the environment map from LiDAR sweeps. These maps are slightly different and comparison is not truly objective. To resolve this problem for the future research we make our 3D LiDAR map publicly available.

# Paper: "Localization of Mobile Robot in Prior 3D LiDAR Maps using Stereo Image Sequence" 

<!-- ## Pipeline:
<img src="./assets/Pipeline.png" alt="Pipeline" width="800"/> -->

## Demo video:
[<img src="https://img.youtube.com/vi/M3FqPPb9njQ/hqdefault.jpg" width="600" height="300"
/>](https://www.youtube.com/embed/M3FqPPb9njQ)

## Abstract
The paper studies the real-time stereo image-based localization of a vehicle in a prior 3D LiDAR map. 
A novel localization approach for mobile ground robot, which successfully combines conventional computer vision techniques, neural network based image analysis and numerical optimization, is proposed.
It includes matching a noisy depth image and visible point cloud based on the modified Nelder-Mead optimization method. 
Deep neural network for image semantic segmentation is used to eliminate dynamic obstacles.
The visible point cloud is extracted using a 3D mesh map representation.
The proposed approach is evaluated on the KITTI dataset and a custom dataset collected from a ClearPath Husky mobile robot.
It shows a stable absolute translation error of about 0.11-0.13 m. and a rotation error of 0.42-0.62 deg.
The standard deviation of the obtained absolute metrics for our method is the smallest among other state-of-the-art approaches. 
Thus, our approach provides more stability in the estimated pose.
It is achieved primarily through the use of multiple data frames during the optimization step  and dynamic obstacles elimination on depth image.
The method's performance is demonstrated on different hardware platforms, including energy-efficient Nvidia Jetson Xavier AGX. 
With parallel code implementation, we achieve an input stereo image processing speed of 14 frames per second on Xavier AGX.

## Citation
If you find this project useful in your research, please consider citing our work:

```
@article{belkin2024localization,
  title={Localization of mobile robot in prior 3D LiDAR maps using stereo image sequence},
  author={Belkin, Ilya V and Abramenko, Alexander A and Bezuglyi, Vitaly D and Yudin, Dmitry A},
  journal={Computer Optics},
  volume={48},
  number={3},
  pages={406--417},
  year={2024}
}
```
