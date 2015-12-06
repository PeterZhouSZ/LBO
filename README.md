# LBO
Discrete Laplace Beltrami Operator (LBO) and related applications.

## Applications:

### Mean Curvature
A direct application of discrete LBO is calculate the mean curvature vector of a surface by simply multipling the Laplacian matrix on the point itself. Following is an example:
<div align="center">
<img src="figures/curvature_value_crop.png" width="200" align="center"/>
<img src="figures/curvature_vector_crop.png" width="200" align="center"/>
<br>
<caption align="bottom">Figure 1. An example of meancurvature field and vectors computed from LBO</caption>
</div>

### Harmonic Map
#### Disk Harmonic Map
Disk Harmonic Map maps a surface homeomorphic to the planar unit disk. It is a popular parameterization method. An example of disk harmonic map on a nefertiti model is shown below:
<div align="center">
<img src="figures/harmonic_map00_crop.png" width="150" align="center"/>
<img src="figures/harmonic_map01_crop.png" width="150" align="center"/>
<img src="figures/harmonic_map02_crop.png" width="200" align="center"/>
<br>
<caption align="bottom">Figure 2. An example of disk harmonic maps. Left to right: Original mesh, mapped mesh, stretched mesh on unit disk</caption>
</div>
#### Spherical Harmonic Map
Spherical harmonic map "blows" a genus-0 model into a sphere. Here an iterative implementation is used.
<div align="center">
<img src="figures/spherical_harmonic_map00_crop.png" width="200" align="center"/>
<img src="figures/spherical_harmonic_map01_crop.png" width="250" align="center"/>
<br>
<caption align="bottom">Figure 3. An example of spherical harmonic maps. A brain model is mapped onto a unit sphere.</caption>
</div>

### Heat method
The heat method ([1]) is a discrete geodesic solution on various domains (grids, triangle/polygonal meshes, point clouds etc.). It's specially suitable for calculating distance fields with different sets of sources on the same mesh for several times. The implementation here is based on triangle mesh only. Here is an example output of heat method on a bunny model:
<div align="center">
<img src="figures/heat_method00_crop.png" width="200" align="center"/>
<img src="figures/heat_method01_crop.png" width="200" align="center"/>
<img src="figures/heat_method02_crop.png" width="200" align="center"/>
<br>
<caption align="bottom">Figure 4. An example of geodesic distance fields generated by heat method.</caption>
</div>

[1] Crane K, Weischedel C, Wardetzky M. Geodesics in heat: A new approach to computing distance based on heat flow[J]. ACM Transactions on Graphics (TOG), 2013, 32(5): 152.
