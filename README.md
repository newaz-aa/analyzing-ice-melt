# analyzing-ice-melt
Image Processing Task

In this project, satellite images are used to study climate change.  Two images of the same region in Antarctica taken two years apart were analyzed. The first image was captured in January of 2018 and the second image was taken in January of 2020. The objective is to understand how much more water from melting is visible in the image taken two years after the first. 

The project is done using Matlab 2020a. Color thresholder app is utilized for experimentation.
Using Color Thresholder app, the ice2020 image was segmented in such a way that areas that are water are labeled true in the resulting binary image. Using the segmentation function created(icemelt.m), ice2018 image was also segmented in the same way.

Experimentation was performed with different color spaces (RGB, YCbCr, HSV, L*a*b*) to obtain the one that provides the optimal segmentation for both images. The L-channel of the L*a*b* color space was found to be most suitable for segmentation.

It was observed that there is an increase of around 3.5 times more water from melting after two years.

icemelt.m file contains the segmentation function. analzye_ice_melt.mlx file contains necessary codes. icemelt18.png and icemelt20.png files display the segmentation.
