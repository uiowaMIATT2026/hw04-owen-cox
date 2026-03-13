# Gradient Anisotropic Diffusion

This gradient anisotropic diffusion algorithm smooths images like a Gaussian lowpass filter while preserving edges.
According to the Slicer wiki, the conductance parameter affects how edges are preserved in the image.
A lower conductance leads to better preserved edges while a higher conductance leads to more edge smoothing.

More iterations causes more smoothing. The time step is related to the time derivative in the heat diffusion equation 
according to the ITK wiki. I will have to do some more reading to understand what is going on here.

I tested this on the CT liver sample data in Slicer, which has some noise from CT artifacts.
These parameters generated a nice smoothing response while preserving edges:
- conductance = 1
- time step = 0.0625
- iterations = 5

These parameters preserved edges between soft tissue and bone while removing some of the CT noise artifacts.
I noted that this took several minutes to run on the CT torso image.
