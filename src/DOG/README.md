# Difference of Gaussians

Difference of Gaussians is a bandpass filter where the highpass and lowpass frequencies are specified by the two sigma values.
The DOG algorithm therefore preserves edges within some range of strengths or gradients.

I tested this on the Slicer brain tumor 2 sample image with various parameters.

## sigma1 = 1, sigma2 = 5
These parameters made the image black and white and blocky. This preserves midrange frequencies and medium edges.

## sigma1 = 5, sigma2 = 6
This preserves a narrow range of low frequency features. The image is wavy and warped looking with some blob structure.

## sigma1 = 0.5, sigma2 = 1
These parameters preserve a narrow band of high frequency features. The resulting image looks like black and white noise with some structure from the original image.

The difference of Gaussian filter can be used for edge detection or to emphasize a particular spatial frequency range.
