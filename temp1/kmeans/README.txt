kmeansSequential.c: naive 2-dimensional implementation of Lloyd's K-means algorithm
kmeansCUDA.cu: parallelized CUDA C implementation of the same.

Required files:

  x_coordinates.txt: x coordinates of the data points arranged in a column.
  y_coordinates.txt: y coordinates of the data points arranged in a column.

  initialCluster_x_coordinates.txt: initial cluster centers in the x direction arranged in a column.
  initialCluster_y_coordinates.txt: initial cluster centers in the y direction arranged in a column.


Compilation of kmeans.c:

  > gcc kmeansSequential.c -o kmeansSequential

Compilation of gpu_kmeans.cu:

  > nvcc kmeansCUDA.cu -o kmeansCUDA


Run:

  > ./kmeansSequential

  or

  > ./kmeansCUDA


Output saved in "output" folder :

  .txt: final cluster centers in the x direction
  .txt: final cluster centers in the y direction
  .txt: final cluster index of each point  


