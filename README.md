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

OSX
--------
Use Makefile to compile the project.
You will need to re-target the compiler to clang to avoid clang unsupported
flags.

WINDOWS
---------
Use included Visual Studio 2012 project. Should run out of the box.
If you do not have Visual Studio 2012, follow the following instructions:
* 1. Create an empty project in this repository. 
* 2. Change the build customizations to target the correct version of CUDA on
     your machine.
* 3. Add cudaBenchmark.cu
* 4. Add paths to NvTools headers and libraries.  If you have installed NSight
     properly, VS should have a macro $(NVTOOLSEXT_PATH) that points to the
     folder. The headers are in include, and the libraries are in lib.
* 5. You should now be able to build the solution contained cudaBenchmark.cu.
     NOTE : To run, you may need to copy the nvtoolsext_32.dll to the System32
     folder or the same folder as the built executable.
* 6. Repeat steps 2 through 5 for reduction and transpose.

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
