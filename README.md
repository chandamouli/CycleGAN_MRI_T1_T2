# CycleGAN based model to transfer MRI T1 style to T2 and vice-versa
> To build a CycleGAN model to generate MRI T1 images from T2 and vice-versa.

## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
- # **Problem Statement**

Misdiagnosis in the medical field is a very serious issue but it's also uncomfortably common to occur. Imaging procedures in the medical field requires an expert radiologist's opinion since interpreting them is not a simple binary process ( Normal or Abnormal). Even so, one radiologist may see something that another does not. This can lead to conflicting reports and make it difficult to effectively recommend treatment options to the patient.

One of the complicated tasks in medical imaging is to diagnose MRI(Magnetic Resonance Imaging). Sometimes to interpret the scan, the radiologist needs different variations of the imaging which can drastically enhance the accuracy of diagnosis by providing practitioners with a more comprehensive understanding.

But to have access to different imaging is difficult and expensive. With the help of deep learning, we can use style transfer to generate artificial MRI images of different contrast levels from existing MRI scans. This will help to provide a better diagnosis with the help of an additional image.

In this capstone, we will use CycleGAN to translate the style of one MRI image to another, which will help in a better understanding of the scanned image. Using GANs we will create T2 weighted images from T1 weighted MRI image and vice-versa.

***Problem statement:*** To build a Generative adversarial model(modified U-Net) which can generate artificial MRI images of different contrast levels from existing MRI scans.

- The dataset consists of 46 T1 images and 43 T2 images. These are un-paired images

The following models are created in this project
   1. Create a U-net model that consists of downsampling (encoder), bottleneck and upsampling (decoder) 
   2. We ran with multiple epochs and plotted the loss function
   3. This requires a manual intervention to review the image quality and decide the number of epochs and other 
      parameters cross referencing the loss function plot
<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
- Model 128, 161, 207 or 250 doesn't show too much of variance in the predicted output. Hence we can conclude that model 128 can be used for further predictions.
Note: Due to time constraint for this project timelines, we are stopping here. The model can further be fine tuned to generate better images and also with other architectures like half-net etc...

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- numpy
- pandas
- tensorflow - Keras, pre-processing,callbacks
- google colab


<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements
- This project was inspired by CycelGAN model to transfer numbers using MNST dataset 
- Stackoverflow for certain code snippets and to understand the usage of augmentation
- tensorflow official documentation to understand various api's used in this project


## Contact
Created by [@chandamouli] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->