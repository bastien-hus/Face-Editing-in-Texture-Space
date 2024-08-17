# Face Editing in Texture Space

This repository contains the PDF of my Bachelor thesis titled **"Face Editing in Texture Space"**, which I completed in August 2023 in collaboration with [Arbrea Labs](https://arbrea-labs.com/).

## About the Thesis

This thesis presents the development of a novel texture editing pipeline for human faces. The main goal of this work is to detect and remove facial wrinkles and other potential skin anomalies in a fully automated manner. The resulting skin texture can then be used to simulate aesthetic medicine and plastic surgery procedures. The research outlines three major steps: detection, inpainting, and upscaling, offering a comprehensive solution that can be used in both academic and commercial applications.

## Abstract

This thesis aims at developing a novel texture editing pipeline for human faces. The goal is to detect and remove facial wrinkles and other potential skin anomalies in a fully automated way. The new skin texture obtained by the pipeline will serve as a source texture for simulating aesthetic medicine and plastic surgery procedures. Therefore, supersampling is used at the end to enhance quality and address the high expectations imposed by medical uses.
The hereby proposed solution is structured into three major steps:  
1. Detection: Wrinkles and skin imperfections are being labelled at this stage. The perfect detection outputs a binary mask covering accurately all unwanted facial areas while covering as little as possible wanted areas. The mask shall provide a reliable input for the next step.  
2. Inpainting: Provided the input image and the generated detection mask, this step has to recreate skin texture to fill the labelled areas. The challenge is to create detailed skin texture and avoid filling the areas with new computer-generated wrinkles. Skin tone and lighting should also match the overall scene of the input picture, in order to provide a seamless inpainting.  
3. Upscaling: Finally,the processed image is upscaled to gain details and provide a workable texture for future applications. The upscaler should not smooth nor modify the colours of the image.
This work provides a comparison of multiple implementations of these steps. Each containing naive and straight-forward solutions as well as more involved and state-of-the-art algorithms.

Finally, a complete and automated pipeline is proposed to evaluate the performance of the solutions on different hardwares.
