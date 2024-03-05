**De-Smoking-De-Hazing-Algorithm**

This project implements a single image dehazing technique in Python. The code's objective is to improve the clarity of photos impacted by fog or air haze. 

*Estimating ambient light and determining the transmission map are the first steps in the dehazing process, which include applying the results to eliminate haze from the original image.

*The image_dehazer class includes functions to compute the transmission map, estimate atmospheric light, and eliminate haze from an input image. 

*Techniques including atmospheric light estimates, filtering, boundary constraints, and optimization using a regularization parameter are all part of the dehazing process.

*Numerous factors can be adjusted for the dehazing technique, such as window sizes for boundary constraints and atmospheric light estimates, constants C0 and C1, regularization parameters, and optimization process parameters.

*The project filters images using a set of Kirsch filters. The weighting function, which is utilized in the dehazing optimization procedure, is computed using these filters.

*The optimization process involves iteratively refining the transmission map using a set of Kirsch filters and a regularization parameter. The goal is to enhance the image by reducing the impact of haze.

*An image that has undergone haze correction—a method that successfully reduces or eliminates atmospheric haze—is the end product of the dehazing procedure. 

*A direct-use function called remove_haze is included in the project. It returns the dehazed image and the associated haze transmission map in exchange for an input image and optional parameters. 

*To display the haze transmission map while the optimization is being done, the code has an option called showHazeTransmissionMap.

*The project leverages the OpenCV library for image processing tasks, including filtering and convolution operations.

**Usage:**

*To use the remove_haze function, users must supply an input image and modify the parameters to fit their own requirements. 

*An example image is included in the code to illustrate the dehazing process and give a real-world example of the algorithm in operation.


