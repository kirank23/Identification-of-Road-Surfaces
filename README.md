# Identification-of-Road-Surfaces 

Detecting various irregularities in road surfaces using images which can be integrated with an ADAS based vehicular navigation system to provide assistance while driving. 

## Abstract

A Road Surface Segmentation and Identification based solution assisting in adaptability and smarter decision making for an Advanced Driver Assistance System (ADAS) in a vehicular environment. It provides reliable assistance for dealing with environments with variations in road surfaces largely relevant but not limited to developing countries. Beneficial for accident avoidance and automating the assessment of road quality which can help identify areas where maintenance is required.

Keywords - Road surface, vehicles, ADAS.

## Project Overview

The primary purpose of this project is to find irregularities in road surface patterns and also finding speed bumps or any other things which can be relevant for vehicular navigation in an Advanced Driver Assistance System (ADAS). 

For example, identifying if the road has cracks, is made up of asphalt or cobblestone or is an unpaved dirt road. The results of this can then be integrated into an Advanced Driver Assistance System (ADAS) which can aid autonomous vehicles. This will help in adapting to the way the vehicles are driven and can be used to create an entire navigation system which can detect such patterns on the road thereby allowing communication between vehicles connected in a network. 

## Introduction

Why is identification of road surfaces important?

In today's world, numerous technologies in the field of autonomous vehicles, such as sensors have made significant progress. They can be used for obstacle recognition and environmental awareness, which is important for ensuring safe personal mobility. These obstacles can include damaged roads, other vehicles and pedestrians as well. There is a need for technology that can help prevent vehicular crashes or collisions when driving. 

The identification of road surfaces provides important information for the way a vehicle should be driven, whether by a human or by an autonomous vehicle. In addition to passenger comfort and vehicle maintenance, it involves the safety of everyone as well. 

## Source of Data Collection - Dataset

RTK (Road Traversing Knowledge) dataset from LAPIX

## Description of Methodology

1. Training Data

The total number of images used = 701.

<img width="369" alt="Screenshot 2022-05-19 at 6 50 14 PM" src="https://user-images.githubusercontent.com/79298507/169303500-9f382b25-ffde-493a-a54e-566f2d3557d9.png">

2. Ground Truth

To train the neural network and to test and validate the results, a Ground Truth (GT) was created with 701 images from the RTK dataset.

<img width="370" alt="Screenshot 2022-05-19 at 6 50 48 PM" src="https://user-images.githubusercontent.com/79298507/169303626-9e41246c-9a6e-40f0-b785-87bb5a751ed6.png">

3. Data Augmentation

For the data augmentation step, standard options from the fastai library were used, with horizontal rotations and perspective distortions being applied.

4. Image Segmentation

<img width="413" alt="Screenshot 2022-05-19 at 6 52 08 PM" src="https://user-images.githubusercontent.com/79298507/169303899-f2821f5b-b491-48ee-9d3a-bb86c931cf60.png">

<img width="627" alt="Screenshot 2022-05-19 at 6 59 08 PM" src="https://user-images.githubusercontent.com/79298507/169305088-2fc6db98-26d5-4368-9142-a0a94fc2d7b2.png">
<img width="627" alt="Screenshot 2022-05-19 at 6 59 36 PM" src="https://user-images.githubusercontent.com/79298507/169305099-a3c5dc31-0675-42c5-9b29-2f4e47d5cb99.png">
<img width="627" alt="Screenshot 2022-05-19 at 7 00 02 PM" src="https://user-images.githubusercontent.com/79298507/169305104-f6f7877b-e0a6-44fa-94d3-0c2c870004cf.png">

## Conclusion

With the ever growing demand for personal mobility vehicles, the spread of autonomous driving technology is expected to accelerate to ensure safe driving for the passengers. However until now the developments in autonomous driving technology had concentrated only on ordinary vehicles, which assumed that the road surfaces are in perfect conditions for driving safely. 

## References

[1] T. Rateke, A. von Wangenheim. “Road surface detection and differentiation considering surface damages”, (2020), Autonomous Robots (Springer).

[2] T. Rateke, K. A. Justen and A. von Wangenheim. “Road Surface Classification with Images Captured From Low-cost Cameras”, Revista de Informática Teórica e Aplicada (RITA).

[3] O. Ronneberger, P. Fischer, T. Brox. “U-net: Convolutional networks for biomedical image segmentation”, (2015).

[4] Shim, Seungbo & Cho, Gye-Chun. (2020). “Lightweight Semantic Segmentation for Road-Surface Damage Recognition Based on Multiscale Learning”. IEEE Access. 

