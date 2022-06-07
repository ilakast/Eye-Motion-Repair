# Eye Motion Repair.
Code that removes residual distortions due to eye motion from images and videos processed by DeMotion. More specifically, it works by calculating the median (*x*,*y*) shift
observed at each row of the registered image from the registration shift in each frame contributing to that image; it then “de-warps” the registered image using
these median shifts, assuming random eyemovement.

References
https://doi.org/10.1167/tvst.11.5.19
