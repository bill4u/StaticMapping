if (CUDA_FOUND)
  file(GLOB cuda_srcs "*.cu")
  cuda_add_library(registrators_cuda STATIC ${cuda_srcs})
  target_link_libraries(registrators_cuda ${CUDA_UTILS_LIBRARIES})
endif (CUDA_FOUND)