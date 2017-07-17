cmake_minimum_required(VERSION 2.8)
project( hesaff )

set(CUDA_TOOLKIT_ROOT_DIR /usr/local/MATLAB/R2016a/bin/glnxa64/)
find_package( OpenCV REQUIRED )

add_executable( hesaff hesaff.cpp pyramid.cpp affine.cpp siftdesc.cpp helpers.cpp )
target_link_libraries( hesaff ${OpenCV_LIBS} )

