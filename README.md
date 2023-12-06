# 2D-Kuramoto-Sivashinsky

Exectutable files and modules for the numerical solution of the two-dimensional Kuramoto-Sivashinsky equation.

There are two main files: 
- 2d_ks_single.exe, and 
- 2d_ks_single_L.exe.
These correspond to solving the equation on [0, 2pi] x [0, 2pi] or [0, 2Lx] x [0, 2Ly] domains, respectively.

The values of the various parameters are defined as inputs and can be found in files data_2d and data_extra. Users can modify these to run the code for different parameter values.

The produced output includes the following files:
- x_k1.txt, has two columns: x and k1
- y_k2.txt, has two columns: y and k2
- u_norm.txt, has four columns: t, E(t), Ė(t), u(π,π)
- u_fft.txt, has size 4M x 2N. This contains the full solution at the final simulation time, u(x,y) at t=Tfinal (which is of size 2M x 2N), followed by its Fourier transform û(k1,k2) which is also of the same size.
