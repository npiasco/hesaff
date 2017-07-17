cmake_minimum_required(VERSION 2.8)
project( hesaff )

find_package( OpenCV REQUIRED )

add_executable( hesaff hesaff.cpp pyramid.cpp affine.cpp siftdesc.cpp helpers.cpp )
target_link_libraries( hesaff ${OpenCV_LIBS} )

