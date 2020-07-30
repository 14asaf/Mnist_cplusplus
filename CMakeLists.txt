cmake_minimum_required(VERSION 3.13)
project(MNIST)


set(CMAKE_CXX_STANDARD 14)
#set(OpenCV_DIR=/home/opencv-3.2.0/share/OpenCV)
#SET("OpenCV_DIR" "/usr/local/include/opencv4/opencv2")
SET("OpenCV_DIR" "/home/asafh/opencv_build/opencv/build")
find_package( OpenCV REQUIRED )

MESSAGE(STATUS "Include dirs ${OpenCV_INCLUDE_DIRS}")
MESSAGE(STATUS "LINK LIBRARIES ${OpenCV_LIBS}")


include_directories( ${OpenCV_INCLUDE_DIRS} )
add_executable(cmake_testapp main.cpp)
#add_executable(cmake_testapp_MNIST main.cpp MNIST.h)
#add_library(test_library STATIC MNIST.h)
target_link_libraries(cmake_testapp  ${OpenCV_LIBS} )
#target_link_libraries(MNIST-Loader  opencv_photo )
