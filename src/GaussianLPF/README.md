# Gaussian Lowpass Filter

The Gaussian lowpass filter uses recursive Gaussian filtering to smooth images.
The sigma value specifies how much smoothing is to be done.
A small sigma corresponds to a narrow Gaussian kernel and a large sigma corresponds to a wide Gaussian kernel.
Because a small sigma better approximates an impulse function, this means less blurring.

I experimented with different sigma values on the Slicer brain tumor 1 sample image.
In this image resolution, a sigma value of ~1.5 seems to provide an amount of blurring that may be useful for algorithmic applications or noise removal.
A sigma value above 5 seems to probably reduce resolution beyond the point of usability, at least for images of this size.
