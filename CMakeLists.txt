cmake_minimum_required(VERSION 2.8)
project(opencv_face_alignment)
set(OpenCV_DIR C:/ICV/OpenCV_bin_release/install)
find_package(OpenCV REQUIRED)
add_executable(opencv_face_alignment sources/preprocessFace.cpp
									 sources/detectObject.cpp
									 sources/main.cpp)
target_link_libraries(opencv_face_alignment opencv_core opencv_imgproc opencv_highgui opencv_objdetect)