cmake_minimum_required (VERSION 3.1)
project(cuda-tutorials)

find_package(CUDA REQUIRED)
find_package(OpenCV REQUIRED core highgui imgproc imgcodecs videoio)

include_directories(
    ./samples
    ${Boost_INCLUDE_DIR}
    ${OpenCV_INCLUDE_DIRS} 
    ${CUDA_INCLUDE_DIRS}
)

link_libraries(
    ${Boost_LIBRARIES}
    ${CUDA_LIBRARIES}
    ${OpenCV_LIBS} 
)

add_subdirectory(samples)