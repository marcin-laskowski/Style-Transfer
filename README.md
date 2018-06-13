# Style Transfer in PyTorch
Style Transfer in PyTorch 0.4.0

### Overview

The idea is that we have two input images: a content image and a style image. The goal is to produce a mixed image which contains style (such as texture, colour) from style image and content from content image. In convolutional neural network, the feature maps in lower layers captures the low level features (i.e. content) and vice versa, the feature maps in higher layers captures the high level features (i.e. style). During style reconstructions, the higher feature levels capture the style of the painting. On the other hand, during content reconstructions, the lower feature levels capture the content.

Measuring low level features would not be able to capture perceptual defferences between output and ground truth images. Gatys et al proposal using high level features to obtain the style of the image and therefore reduce the perceptual differences. Moreover, Johnson et al improves Gatys et al’s work by training a feed forward transformation networks ahead. Following code is based on the Neural-Style algorithm developed by Leon A. Gatys, Alexander S. Ecker and Matthias Bethge.


Input pictures:
<p align="center">
  <img width="700" src="https://github.com/mlaskowski17/Style-Transfer/blob/master/images/style_and_content.jpg">
</p>

Output pictures:
<p align="center">
  <img width="1000" src="https://github.com/mlaskowski17/Style-Transfer/blob/master/images/epochs.jpg">
</p>
