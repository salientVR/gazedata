# Eye tracking dataset in SalientVR
This project hosts the gaze-annotated 360° video dataset introduced in SalientVR (MobiCom 2022).

You can download the 360-degree videos and the corresponding gaze data at https://drive.google.com/drive/folders/1E2qYrpdv1ZjAAZj4PNbA4YeP0wW8zTti?usp=sharing.

The raw videos are downloaded from the Virtual Reality channel on YouTube with the equirectangular projection.
The raw gaze data are collected using the HTC Vive Pro Eye VR headset with the built-in Tobii eye tracking device and the eye tracking software Tobii Pro Lab.
Besides the raw gaze data, we also release a set of processed gaze dataset to facilitate practical uses, processed as follows:
* handling the missing value (caused by eye closure for example) by moving average interpolation.
* converting the millisecond-level data to the frame-level data.
* converting the quaternion coordinates of head directions to the 2-dimension plane coordinates where both gaze points and head directions are fractional from 0.0 to 1.0 with respect to the panorama image and are computed from the top left corner.

Note that we found there are about 2.5% data in which the gaze points are out of the alleged viewport range computed by the corresponding head directions maybe due to the larger eyeball oculogyration range than VR screens.

If you use the dataset, please refer to our paper as follows: "S. Wang, S. Yang, H. Li, X. Zhang, C. Zhou, C. Xu, F. Qian, N. Wang, and Z. Xu, SalientVR: Saliency-Driven Mobile 360-Degree Video Streaming with Gaze Information, *ACM MobiCom, 2022*."
If you have any questions about the dataset, please contact me by email *wshb20081996@stu.xjtu.edu.cn*.
