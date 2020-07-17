# C++ version:

* the implementations of the ball k-means algorithm are "ball_k_means_Xf.cpp" and "ball_k_means_Xd.cpp", which are code for "float" and "double" versions respectively.

* the param "isRing" is used to switch the ring version and the no ring version of the algorithm.

### Description of 'Xd' and 'Xf' versions：

* "Xd" means that data is stored and operated in the program in "double" type.

* "Xf" means that data is stored and operated in the program in "float" type.

* According to our experience, the "Xd" version can get more accurate results but the running time is slightly slower, and the "Xf" version can reach the fastest running time, but low accuracy will result in inaccurate results.

# Requirements

### Minimal installation requirements (C++):

* C++ compiler supporting C++11
  
* Linux operating system or Windows operating system

* Eigen 3 template library

### Optional but recommended (C++):

* BLAS implementation, we recommend this one: http://www.openblas.net/
  
* Intel MKL implementation, we recommend this one: https://software.intel.com/en-us/mkl

# Using

### Step 1: call "ball_k_means" function

#### Parameters: 

* dataset: clustering data in Matrix format in the Eigen library.

* centroids: initial center point data in matrix format in the Eigen library.

* isRing: int type, switch the ring version and the no ring version of the algorithm. '1' means the current algorithm is a ring version, and others mean the current algorithm is no ring version.

* detail: bool type variable, "true" means output detailed information (including k value, distance calculation times, time, etc.), "false" means no detailed information is output. The default is false.

#### Output: 

* labels: labels of clustering data in matrix format in the Eigen library.