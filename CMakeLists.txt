cmake_minimum_required(VERSION 3.1)

project(count_strings CXX)

# include(../../common/cmake/common.cmake)

# set_common_project_settings(tbb)

add_executable(count_strings count_strings.cpp)

target_link_libraries(count_strings TBB::tbb Threads::Threads)
# target_compile_options(count_strings PRIVATE ${TBB_CXX_STD_FLAG})
