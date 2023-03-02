
<h1 align="center">:books:Fourier-Transformation:book: :signal_strength: </h1>

When we work in image processing, Fourier transform is an important image processing tool which is used to decompose an image into the frequency domain. the input image of the Fourier transform is the spatial domain(x,y) equivalent. the output of the Fourier transform represents the image in the frequency domain.

In the frequency domain image, each point represents a particular frequency contained in the spatial domain image. if an image has more high-frequency components (edges, stripes, corners ), there will be a number of points in the frequency domain at high-frequency values.

example:

```bash
import numpy as np
import matplotlib.pyplot as plt
import cv2
%matplotlib inline
# Read in the images
image_stripes = cv2.imread(‘images/stripes.jpg’)
# Change color to RGB (from BGR)
image_stripes = cv2.cvtColor(image_stripes, cv2.COLOR_BGR2RGB)
# Read in the images
image_solid = cv2.imread(‘images/pink_solid.jpg’)
# Change color to RGB (from BGR)
image_solid = cv2.cvtColor(image_solid, cv2.COLOR_BGR2RGB)
# Display the images
f, (ax1,ax2) = plt.subplots(1, 2, figsize=(10,5))
ax1.imshow(image_stripes)
ax2.imshow(image_solid)
```

