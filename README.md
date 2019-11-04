# Harris-Corner-Detector
Harris Corner Detector is a corner detection operator that is commonly used in computer vision algorithms to extract corners and infer features of an image.
<br/>
<br/>
A corner is a point whose local neighborhood stands in two dominant and different
edge directions. In other words, a corner can be interpreted as the junction of two edges,
where an edge is a sudden change in image brightness. Corners are the important features
in the image, and they are generally termed as interest points which are invariant to
translation, rotation, and illumination.
<br/>
<br/>
### The Harris Corner Detector algorithm in simple words is as follows :
### STEP 1. It determines which windows (small image patches) produce very large variations in intensity when moved in both X and Y directions (i.e. gradients).
### STEP 2. With each such window found, a score R is computed.
### STEP 3. After applying a threshold to this score, important corners are selected and marked.
<br/>
<br/>
Take the gray-scale of the original image. Apply a Gaussian filter to smooth out
any noise. Apply Sobel operator to find the x and y gradient values for every pixel in
the grayscale image. For each pixel p in the grayscale image, consider a m*m window
around it and compute the corner strength function. Call this its Harris value. Find all
pixels that exceed a certain threshold and are the local maxima within a certain window
(to prevent redundant dupes of features). Compute a feature descriptor of all such points.
<br/>
<br/>
For more all the algorithms used refer the Report file
<br/>
For more details refer : https://iitmcvg.github.io/summer_school/Session3/
