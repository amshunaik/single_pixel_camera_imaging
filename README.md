## About single pixel camera imaging 
* Single-Pixel Imaging(SPI) involves projecting spatially resolved patterns onto a scene and measuring correlated intensities with the single-pixel detector.
* Here we use SPyRiT which is a PyTorch-based toolbox for deep image reconstruction, and single pixel imaging simulation

### The mathematical formulation in Single Pixel Camera (SPC) Imaging is centered around the measurement model, which can be represented as:
####  M⋅x=y
Here’s what the variables represent:
* ( M ) is the measurement matrix, where each row includes the sampling patterns.
* ( x ) is the image being measured, consisting of real-valued pixels.
* ( y ) is the result of the measurement that includes elements corresponding to the intensity of light reflected by the object for each pattern.
  
The measurement matrix ( M ) is typically a rectangular ( k times n ) matrix, where ( k ) is less than ( n ) for a compressive measurement. This means that the number of measurements ( k ) is less than the number of pixels ( n ), which is the basis of compressed sensing.
The reconstruction process in compressive sensing is an optimization problem that seeks to find the sparsest solution that is consistent with the measurements. This often involves solving an underdetermined system with regularization terms that promote sparsity (e.g., L1 norm minimization).
