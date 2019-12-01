# **Finding Lane Lines on the Road** 

White Output               | Yellow Output
:-------------------------:|:-------------------------:
![](./image_output/white.gif) |  ![](./image_output/yellow.gif)


---
### Pipeline

The pipeline consists in 8 steps, including the ouput testing.

### 1) Read/Upload the image to be processed

First step is to upload the image that has to be processed.

->![Starting image](./image_output/starting.png)<-

### 2) Conversion into Gray Scale (cv library)

Once the image is uploaded, it is converted to a gray scaled one to start highlighting the pixel gradients.

->![Gray scaled image](./image_output/grayscale.png)<-

### 3) Canny Edge detection in order to higlight edges.

Canny Edge Detection is based on gradient, meaning how fast are x and y changning. It is expected to find edges where pixel values change rapidly (road lines).

->![Edge Detected](./image_output/edge.png)<-

### 4) Define a polynomial region of interest (where to find lane lines).

In an image, only a region of interest has to be taken into account, where our lines will be. For this reason, a mask is created in order to higlight edges where required.

->![Edge Masked](./image_output/edgemasked.png)<-

### 5) Hough Transformation in order to identify points building a line.

A transofrmation into the Hough Space is then performed in order to find the line that pass through all the points that a re making a line.

->![Hough Transofrmation](./image_output/houghtransform.png)<-

### 6) Line drawing

Once the line are highlightes, an average and extrapolation of their points is performed in order to draw the road lines.

->![Road Lines Drawn](./image_output/linedrawn.png)<-

### 7) Overlay of the two images (lines detected + original image).

Last part of the pipeline is to overlay the starting image with the one with the lines drawn.

->![Images overlayed](./image_output/finalimage.png)<-

### 8) Output testing.

Finally, the whole chain is run with sample images and videos.
