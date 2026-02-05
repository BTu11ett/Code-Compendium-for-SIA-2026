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
        -
7) butterworth(size, center, radius)
        -
8) RollingBall(image)
        -
9) HistEqualise(image)
        - 
   
   
