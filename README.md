# Code-Compendium-for-SIA-2026
This repository is where, each week, I will add new methods and functions that have been created for image analysis tasks, such as filtering, thresholding, and Fourier Transforms, to name a few. 

The functions included so far are:

1) first_step(file_path)
        - Given a path to an image, this function will output the image, the image size and type, and pixel value type, as well as the minimum and maximum.
2) watershedFunction(image, x, y)
        - This inputs a binary image, as well as two parameters x: min_distance, and y: threshold_abs, which are both used in the peak_local_max to find local maxima in the image. The output of this function is the distance map, the watershed, and a segmented image, as well as a labelled image and the total number of regions identified.
3) plotsHistogram(pixValMin, pixValMax, imgOrig)
        - Takes an image as well as the highest and smallest pixel value, and plots the count against pixel value to more easily observe where thresholds would work.
4) fourierFunction(imgOrig)
        - takes an image, applies the fourier transform, shifts the result, takes the absolute square of the result, as well as the log to display the 2d power spectrum.
5) powerSpectrum1D(image)
        - Takes the radial average of the 2d power spectrum, and displays it as a squashed 1 dimension to more obviously see the different length scale frequencies.
   
6) highPassFilter(size, center, radius)
        - Defines an array which is 1 everywhere, but zero in a central region. The parameters used are the size of the image, the centre, and the radius of the central region.
7) butterworth(size, center, radius)
        - This has a similar function to the high-pass filter, but does not have harsh edges, which causes the diffraction-looking effect. Instead, there is a gradient between the high and low regions.
9) RollingBall(image, radius)
        - Applies a rolling ball correction to an image to remove uneven illumination. The size of the ball is passed in as the radius, and the corrected image is formed by subtracting the background away from the image.
10) HistEqualise(image)
        - Reequalises the histogram of the image after the rolling ball, to give better contrast. 
   
   
