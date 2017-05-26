### Abstract
Vision-based mobile robot navigation is a vibrant area of research with numerous algorithms developed, with a vast majority of which either belong to the scene-oriented simultaneous localization and mapping (SLAM) or fall into the category of robot-oriented lane-detection/trajectory tracking. These methods suffer from high computational cost and require stringent labelling and calibration efforts. To address these challenges, this paper proposes a lightweight robot navigation framework based purely on uncalibrated spherical images. To simplify the orientation estimation, path prediction and improve computational efficiency, the navigation problem is decomposed into a series of classification tasks. To mitigate the adverse effects of insufficient negative samples in the ``navigation via classification'' task, we introduce the spherical camera for scene capturing, which enables $360^\circ$ fisheye panorama as training samples and generation of sufficient positive and negative heading directions. The classification is implemented as an end-to-end Convolutional Neural Network (CNN), trained on our proposed Spherical-Navi image dataset, whose category labels can be efficiently collected. This CNN is capable of predicting potential path directions with high confidence levels based on single, uncalibrated spherical image. Experimental results demonstrate that the proposed framework outperforms competing ones in realistic applications.

### Model
![Image](network.png)

### Data
Dataset can be downloaded [here](http://pan.baidu.com/s/1jILuDng), or [here](http://dwz.cn/61ckOmhttp://dwz.cn/61ckOm). Total in size = 7.43G. 
Data was caputred 29frames/s, and sampled 30 frames/s. Thus, 1 image ~= 1s. 
Demo video 15fps, ~= 15x faster than the original video.

### Performance
[Here](https://www.youtube.com/watch?v=Z6GgbcZRwsM) is a demo video for navigation within campus.

### Reference
1. Ran, L.; Zhang, Y.; Yang, T.; Zhang, P. Autonomous Wheeled Robot Navigation with Uncalibrated Spherical Images. Chinese Conference on Intelligent Visual Surveillance. Springer, Singapore, 2016, pp. 47–55.
2. Giusti, A.; Guzzi, J.; Ciresan, D.; He, F.L.; Rodriguez, J.P.; Fontana, F.; Faessler, M.; Forster, C.; Schmidhuber, J.; Di Caro, G.; Scaramuzza, D.; Gambardella, L. A Machine Learning Approach to Visual Perception of Forest Trails for Mobile Robots. IEEE Robotics and Automation Letters 2016. 