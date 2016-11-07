# hypre_openmp

Get same results with openmp enabled, in terms of floating point numbers (I have tested with Intel compilers). Please follow below configuration options

1. configure with following command
    
        ./configure --prefix=---- CC=mpiicc CFLAGS="-O3 -xHOST -fp-model strict -qopenmp -mkl" CXX=mpiicpc F77=mpiifort CXXFLAGS="-O3 -xHOST -fp-model strict -qopenmp -mkl" FFLAGS="-O3 -xHOST -fp-model strict -qopenmp -mkl" --with-openmp --with-blas --with-blas-lib="-lmkl_rt -lmkl_intel_lp64 -lmkl_core -lmkl_intel_thread" --with-lapack --with-lapack-lib="-lmkl_rt -lmkl_intel_lp64 -lmkl_core -lmkl_intel_thread"

2. compile with "make"

3. make install


    
