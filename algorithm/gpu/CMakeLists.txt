set(CUDA_ARCHITECTURES "86")
if(NOT DEFINED CUDA_ARCHITECTURES)
set(CUDA_ARCHITECTURES "35;50;60;61;70;75;80;86" CACHE STRING "List of target NVIDIA GPU architectures")
endif()


project(dawn LANGUAGES CXX CUDA)
add_subdirectory(apsp_gpu)
add_subdirectory(bfs_gpu)
add_subdirectory(cc_gpu)
add_subdirectory(mssp_gpu)
add_subdirectory(sssp_gpu)