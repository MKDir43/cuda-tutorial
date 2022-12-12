# options
set(CMAKE_CXX_STANDARD 14)
set(CMAKE_CXX_FLAGS "-std=c++14 -O3 -Wno-format")
set(CMAKE_BUILD_TYPE Release)
#set(CUDA_NVCC_FLAGS "${CUDA_NVCC_FLAGS}")

cuda_add_executable(convolution main.cpp)