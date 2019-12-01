# **Finding Lane Lines on the Road** 

White                      |  Yellow
:-------------------------:|:-------------------------:
![](./image_output/white.gif) |  ![](./image_output/yellow.gif)


---

1) Read/Upload the image to be processed.
2) Conversion into Gray Scale (cv library).
3) Canny Edge detection in order to higlight edges.
4) Define a polynomial region of interest (where to find lane lines).
5) Hough Transformation in order to identify points building a line.
6) Line drawing
7) Overlay of the two images (lines detected + original image).
8) Output testing.


---

### Reflection

### 1. Describe your pipeline. As part of the description, explain how you modified the draw_lines() function.

My pipeline consisted of 5 steps. First, I converted the images to grayscale, then I .... 

In order to draw a single line on the left and right lanes, I modified the draw_lines() function by ...

If you'd like to include images to show how the pipeline works, here is how to include an image: 

![alt text][image1]


### 2. Identify potential shortcomings with your current pipeline


One potential shortcoming would be what would happen when ... 

Another shortcoming could be ...


### 3. Suggest possible improvements to your pipeline

A possible improvement would be to ...

Another potential improvement could be to ...
