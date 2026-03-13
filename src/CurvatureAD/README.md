# Curvature Anisotropic Diffusion

I tested the Curvature AD algorithm on the Slicer brain tumor 1 sample image and found that these parameters worked fairly well:
- conductance = 0.5
- time step = 0.0625
- iterations = 5

This flattened much of the noise and led to a more "matte" appearance, but the edges seem distorted in a way that 
is different from the gradient AD.