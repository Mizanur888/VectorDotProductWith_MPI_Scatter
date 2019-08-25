# VectorDotProductWith_MPI_Scatter
In this assignment we parallelize the matrix-vector product to calculate dot product more efficiently. To reducing the calculation time, we send chunks to array to different processes, so that each process can calculate the dot product of chunks of array. Also, we calculate the start, end and total time to determine how long it taken by each process. 

## Design and Implementation: 
Idea is to make the program work more efficiently by using different processes, and let each process do each part of the work. we calculate the dot product of matrix and vector; large matrix can take longer amount of time to calculate dot product. We use different MPI Program to minimize the time complexity, so that larger matrix can be calculate faster by sending chunks of data to different processes. So, we needed function to cut the matrix small parts and send it to different process, and MPI scatter does that things, it’s very efficient to work with MPI scatter to send data to different process. MPI Scatter takes in array of elements and distributed the elements in the order of process rank. 
