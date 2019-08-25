# VectorDotProductWith_MPI_Scatter
In this assignment we parallelize the matrix-vector product to calculate dot product more efficiently. To reducing the calculation time, we send chunks to array to different processes, so that each process can calculate the dot product of chunks of array. Also, we calculate the start, end and total time to determine how long it taken by each process. 
