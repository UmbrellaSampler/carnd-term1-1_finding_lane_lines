# **Finding Lane Lines on the Road** 

## Writeup

### Overview

---

**Finding Lane Lines on the Road**

The goals / steps of this project are the following:
* Make a pipeline that finds lane lines on the road
* Reflect on your work in a written report


[//]: # (Image References)

[image1]: ./examples/grayscale.jpg "Grayscale"

---

### Reflection

### 1. Describe your pipeline. As part of the description, explain how you modified the draw_lines() function.

My pipeline consists of 6 steps and an optional 7th steps. 

* Gray Scaling
* Gaussian Blur
* Canny Edge Detection
* Masking by Polygon
* Drawing Lines 
  - Line Detection 
    - Applying a Hough transform on the clipped and edged image.
    - Separating lines by negative and positive slope
    - Linear fit through all both start end end line points.
    - Use linear model to find start and end point for the resulting line  
  - Line Drawing
    - Draw detected road lines on empty image
* Draw detected edges on original image
First, I converted the images to grayscale, then I .... 

In order to draw a single line on the left and right lanes, I modified the draw_lines() function by ...

If you'd like to include images to show how the pipeline works, here is how to include an image: 

[image1]: ./test_images_output/solidWhiteCurve.jpg


### 2. Identify potential shortcomings with your current pipeline


One potential shortcoming would be what would happen when ... 

Another shortcoming could be ...


### 3. Suggest possible improvements to your pipeline

A possible improvement would be to ...

Another potential improvement could be to ...
