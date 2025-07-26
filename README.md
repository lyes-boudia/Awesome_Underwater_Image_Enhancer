# Awesome Heuristic Method for Underwater Image Enhancement

This repository contain my implementation of a custom heuristic method that I developed to further enhance previously enhanced underwater images, with targeted improvements in contrast, luminance, and color vibrancy. 
The resulting higher quality images can serve as references to enable an underwater image enhancement neural networks to be trained on data with improved visual fidelity.

For certain types of images, this heuristic method may introduce minor color artifacts due to its rule based nature. However, these artifacts can be corrected by fine tuning the parameters provided in the implementation.

## behind this code:

In order to train a neural network to enhance unerwater images (UNET based architecture for instance), a labeled dataset containing input images along with their corresponding reference images is required. 
Such a supervised design can output good results if the spatial resolution of the images are preseved and the architecture is well designed.

The main objectives of any underwater enhancement model should not simply replicate the reference images provided, but to go beyond them in terms of luminance,
contrast, and color fidelity. If we were to use the reference images directly as targets during training, the model would at its best be limited to reproducing those exact images. 

This approach would constrain the model to the quality and limitations of the reference enhancements, preventing it from producing images of superior quality. 

However, this limitation is somewhat relative, because the network parameters are optimized over a relatively large number of images in the training dataset, which includes
a variety of underwater scenes, which acts as a form of implicit regularization. This broad exposure enables the model to learn more generalized enhancement patterns, 
resulting in more consistent and balanced outputs in terms of color fidelity and contrast restoration.

In general, having better quality reference images provides a stronger supervision signal, this can significantly improve the perceptual and visual quality of the network enhanced outputs.


## Important Note

If you use this repository in your research, project, or publication, if you find this project useful whether in part or in whole. consider citing it as a sign of academic integrity:

Lyes, Boudia. 2025. Awesome_Underwater_Image_Enhancer. Version 1.0. GitHub: https://github.com/lyes-boudia/Awesome_Underwater_Image_Enhancer

This project is shared freely under an open license that requires attribution. 

## License

This repository is licensed under the [Creative Commons Attribution-NonCommercial 4.0 International (CC BY-NC 4.0)](https://creativecommons.org/licenses/by-nc/4.0/).

You are free to use, modify, and share this code for **non-commercial purposes** with proper attribution.  
Commercial use and redistribution are **not permitted**.
