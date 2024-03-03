# Color Halftone Image Super-Resolution with Halftone-EDSR and Halftone-Net

This project introduces novel methods for enhancing the resolution of color halftone images using convolutional neural networks (CNNs). Notably, our work represents the first attempt to achieve this using CNNs.

## Halftone-EDSR Approach
We propose a variation of the Enhanced Deep Super-Resolution (EDSR) network trained specifically on halftone images, referred to as Halftone-EDSR. 

Two strategies are explored for upscaling color halftone images using Halftone-EDSR:

1. **Independent-Channel**: Employ four monochrome Halftone-EDSR models to upscale each channel independently and subsequently merge the results to obtain the final upscaled color image.
   
2. **Joint-Channel**: Train a single model capable of simultaneously increasing the resolution of all four channels.

## Data Augmentation and Training Efficiency
Data augmentation is crucial for preventing overfitting and enhancing model performance in various CNN applications. However, conventional augmentation techniques are impractical for halftone images due to their unique dot patterns. We demonstrate that random cropping serves as an effective data augmentation method for halftone image upscaling, leading to significant performance improvements. Moreover, employing cropping reduces training time considerably.

## Moiré Pattern Reduction with Halftone-Net
Upscaled halftone images may exhibit strong Moiré patterns. To address this issue, we introduce Halftone-Net, a modified CNN architecture derived from Halftone-EDSR.

# Read more

[Super-Resolution of Color Halftone Images Using Convolutional Neural Networks](https://ieeexplore.ieee.org/document/10387444)

# Cite this
```
@ARTICLE{10387444,
  author={Novaes, Guilherme Apolinario Silva and Kim, Hae Yong},
  journal={IEEE Access}, 
  title={Super-Resolution of Color Halftone Images Using Convolutional Neural Networks}, 
  year={2024},
  volume={12},
  number={},
  pages={9082-9096},
  keywords={Image color analysis;Image resolution;Color;Printing;Convolutional neural networks;Printers;Data augmentation;Deep learning;Superresolution;Halftone;convolutional neural networks;deep learning;up-sampling;super-resolution},
  doi={10.1109/ACCESS.2024.3352431}}
```
