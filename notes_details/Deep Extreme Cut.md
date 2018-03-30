# Abstract: 

This paper explores the use of extreme points in an object
(left-most, right-most, top, bottom pixels) as input to obtain
precise object segmentation for images and videos. We do
so by adding an extra channel to the image in the input of
a convolutional neural network (CNN), which contains a
Gaussian centered in each of the extreme points. The CNN
learns to transform this information into a segmentation of
an object that matches those extreme points.

By creating a heatmap with activations in the regions of extreme points. We center
a 2D Gaussian around each of the points, in order to create
a single heatmap. The heatmap is concatenated with the
RGB channels of the input image, to form a 4-channel input for the CNN.

![Deep Extreme Cut](https://github.com/fandulu/paper-notes/blob/master/images/Deep%20Extreme%20Cut.png)
