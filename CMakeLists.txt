cmake_path(SET out_dir NORMALIZE "${CMAKE_SOURCE_DIR}/out/${CMAKE_BUILD_TYPE}")
cmake_path(SET CMAKE_LIBRARY_OUTPUT_DIRECTORY "${out_dir}")
cmake_path(SET CMAKE_RUNTIME_OUTPUT_DIRECTORY "${out_dir}")

cmake_path(SET src_dir NORMALIZE "${CMAKE_CURRENT_SOURCE_DIR}/src")

add_subdirectory(src/targets/lib)
add_subdirectory(src/targets/prog)

