# **Finding Lane Lines on the Road** 

White                      |  Yellow
:-------------------------:|:-------------------------:
![](./image_output/white.gif) |  ![](./image_output/yellow.gif)


---
### Pipeline

The pipeline consists in 8 steps, including the ouput testing.

### 1) Read/Upload the image to be processed

First step is to upload the image that has to be processed.

![Starting image](./image_output/starting_image.png)

2) Conversion into Gray Scale (cv library).
3) Canny Edge detection in order to higlight edges.
4) Define a polynomial region of interest (where to find lane lines).
5) Hough Transformation in order to identify points building a line.
6) Line drawing
7) Overlay of the two images (lines detected + original image).
8) Output testing.


---

### Reflection

### 1. ### Reflection

### 2. Identify potential shortcomings with your current pipeline


One potential shortcoming would be what would happen when ... 

Another shortcoming could be ...


### 3. Suggest possible improvements to your pipeline

A possible improvement would be to ...

Another potential improvement could be to ...
