## MidDas_3.0


# Depth Estimation with DPT (Depth Prediction Transformer)
This repository contains code for performing depth estimation on images using the DPT (Depth Prediction Transformer) model. Depth estimation is the task of predicting the depth map of a scene from a single image, which can be useful for various applications such as autonomous driving, robotics, and augmented reality.

## Overview
In this repository, we utilize the DPT model provided by Intel through the Transformers library to perform depth estimation on images. The DPT model is a transformer-based architecture specifically designed for depth prediction tasks.

## Code Explaination
The script utilizes the Hugging Face Transformers library to access the pre-trained DPT model, specifically the DPTImageProcessor and DPTForDepthEstimation classes. Initially, an image is loaded from a URL using the PIL library. Subsequently, the DPTImageProcessor preprocesses the image, converting it into a format suitable for the DPT model. The preprocessed image is then fed into the DPTForDepthEstimation model, which predicts the depth map of the scene depicted in the image. After obtaining the depth prediction, the script performs interpolation to resize the predicted depth map to match the original image's dimensions. Finally, the interpolated depth map is converted back into an image format and displayed. This script serves as a practical example of using pre-trained deep learning models for computer vision tasks, specifically depth estimation, showcasing the capabilities of the DPT model for understanding the spatial layout of scenes captured in images. Additionally, it demonstrates how to integrate Hugging Face's Transformers library for seamless access to pre-trained models and processing pipelines.

## Output
The output of the provided code will be an image representing the estimated depth map of the scene depicted in the input image. This depth map provides information about the distance of objects from the camera in the original image. The output image will display varying shades of gray, where lighter shades correspond to objects closer to the camera, and darker shades represent objects farther away. The depth map is generated using the Depth Prediction Transformer (DPT) model, which leverages deep learning techniques to infer the spatial layout of the scene and estimate depth accurately. By visualizing the depth map, users can gain insights into the three-dimensional structure of the scene captured in the input image, enabling applications such as augmented reality, autonomous navigation, and scene understanding.

![out](https://github.com/AkshayRamakrishnann/MidDas_3.0/assets/111365771/1103ce34-c600-4201-9f44-a78bcd5803d2)

