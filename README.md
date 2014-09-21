CUDA_Exercises
==============

Group of introductory exercises to CUDA

===================================================
USAGE
===================================================
LINUX
---------
Use Makefile to compile project.
Requires gcc/g++ 4.4 (or nvcc compatible version)
CUDA 5.5 or later (latest version recommended)

WINDOWS
---------
Use included Visual Studio 2012 project. Should run out of the box.

===================================================
EXERCISES
===================================================
CUDA BENCHMARK
---------------
This executable runs a benchmark for pageable and pinned Host->Device and Device->Host memory transfer using cudaMemcpy.It also runs a benchmark for global memory Device->Device memory copies.

It is a good way to assess the maximum practical bandwidth limits of GPUS.

TRANSPOSE
----------
Executes matrix transpose operations.
Each stage advances the performance of the kernel.

REDUCTION
----------
Executes sum of all elements in an array.
Each stage advances the performance of the kernel.

===================================================
NOTES
===================================================
* Exercises run CUDA BENCHMARK internally and display output
* The VS projects and Makefiles are built for 64-bit machines. You can modify it for 32-bit fairly easily.

===================================================
CONTACT
===================================================
Email: mzshehzanayub@gmail.com

===================================================
