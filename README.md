# Color Transfer Between Images: Implementation
This is implementation of paper <i>"<a href="https://pdfs.semanticscholar.org/c68a/5e31f75249b335a4d29cc348ba3e3160e337.pdf">Color Transfer between Images</a>"</i>.

## Specification
This code is written by C++.  
We use <a href="https://opencv.org/">OpenCV (Open Source Computer Vision Library)</a> for basic image operations.

## Description
They map the reference image's look and feel onto the source image (see figure below).  
For this goal, they select lab color space as an orthogonal color space without correlations between color axes, and adjust the mean and variance of colors in the lab space of the source image to the reference image.  

In <i>"main.cpp"</i>, the source image path and the reference image path is <i>"src_filename"</i> and <i>"ref_filename"</i> respectively.

<u>source image</u>
<img src="examples/src.jpg">
<u>reference image</u>
<img src="examples/ref.jpg">
<u>result image</u>
<img src="examples/dst.jpg">
