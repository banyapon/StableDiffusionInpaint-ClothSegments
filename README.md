# StableDiffusionInpaint-ClothSegments
This project explores the application of cloth segmentation to inpainting, allowing for modification or removal of objects from clothing images using Stable Diffusion Inpainting and a RunwayML model.
## Cloth Segmentation and Inpainting Labs

## Run this work ##
Jupyter notebook with the example pipeline: 

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/18gpTsNLfiXw5hADVPVUyyxVGf93SFlii?usp=sharing)

# Key Points
![](https://github.com/banyapon/StableDiffusionInpaint-ClothSegments/blob/main/images/screen1.png?raw=true)
## Pre-trained Model:
This code leverages a pre-trained model, which means you don't need to train the model from scratch. You can immediately use it for inference (making predictions).
## Image Segmentation: 
The primary goal is to identify and segment different clothing items within an image.
## Custom Library: 
The functions from iglovikov_helper_functions seem to be part of a custom or external library designed to simplify common tasks in deep learning projects.

```bash
pipe = StableDiffusionInpaintPipeline.from_pretrained("runwayml/stable-diffusion-inpainting")
```
This line of code is the heart of setting up the Stable Diffusion model for image inpainting tasks within your Python environment. 

![](https://github.com/banyapon/StableDiffusionInpaint-ClothSegments/blob/main/images/complete.jpg?raw=true)

## Retrieves:
It fetches the Stable Diffusion Inpainting model (weights, architecture, configuration) that has been trained by RunwayML specifically for the task of filling in missing or masked areas of images.
## Sets up: 
It creates an instance of the StableDiffusionInpaintPipeline class and initializes it with the downloaded model.
## Makes it usable: 
It assigns this pipeline to the pipe variable, allowing you to easily call functions on pipe to perform inpainting on your images.

## Result:
![](https://github.com/banyapon/StableDiffusionInpaint-ClothSegments/blob/main/images/download.png?raw=true)

## References
- https://github.com/mberkay0
- https://github.com/ternaus/cloths_segmentation
