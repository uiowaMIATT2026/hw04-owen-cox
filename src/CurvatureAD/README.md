# Curvature Anisotropic Diffusion

I tested the Curvature AD algorithm on the Slicer brain tumor 1 sample image and found that these parameters worked fairly well:
- conductance = 0.5
- time step = 0.0625
- iterations = 5

This flattened much of the noise and led to a more "matte" appearance, but the edges seem distorted in a way that 
is different from the gradient AD.
According to the ITK wiki, the curvature anisotropic diffusion algorithm does not preserve edges as well as gradient anisotropic diffusion.
This aligns with my observations in implementing it on the brain tumor image.
I found that a lower conductance value seemed to produce more reasonable smoothing for curvature vs gradient AD, which would make sense if gradient AD is intrinsically better at edge preservation.
