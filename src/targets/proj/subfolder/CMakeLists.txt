cmake_minimum_required (VERSION 3.15)

cmake_path(SET out_dir NORMALIZE "${CMAKE_SOURCE_DIR}/out/${CMAKE_BUILD_TYPE}")
cmake_path(SET CMAKE_LIBRARY_OUTPUT_DIRECTORY "${out_dir}")
cmake_path(SET CMAKE_RUNTIME_OUTPUT_DIRECTORY "${out_dir}")

set(PATH_TO_REPOROOT "${CMAKE_CURRENT_SOURCE_DIR}/../../../..")

include("${PATH_TO_REPOROOT}/src/targets/lib/CMakeLists.txt")
include("${PATH_TO_REPOROOT}/src/targets/prog/CMakeLists.txt")
