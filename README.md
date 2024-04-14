# Assignment07---Multi-Threading
## Multi-Threading

## METHODOLOGY
This Python script benchmarks the performance of matrix multiplication with varying numbers of threads using the NumPy library. Here's the methodology:
Matrix Generation: Random matrices of size 1000x1000 are generated for the constant matrix and 100 random matrices.
Thread Configuration: The number of threads for NumPy operations is configured using environment variables (NUMEXPR_NUM_THREADS and OMP_NUM_THREADS). The script iterates over a list of thread counts from 1 to 8.
Matrix Multiplication: The constant matrix is multiplied with each of the 100 random matrices using NumPy's matmul function.
Time Measurement: The time taken for each multiplication operation is recorded.
CPU Usage Measurement: The CPU usage is measured before and after the matrix multiplication using the psutil library.

## RESULT GRAPH
The graph illustrates the relationship between the number of threads used in the matrix multiplication and the operation time. As the number of threads increases, the time taken generally decreases, indicating improved performance with parallelization. However, the overhead of managing additional threads may lead to diminishing returns beyond a certain point.

