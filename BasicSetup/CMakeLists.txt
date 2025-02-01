cmake_minimum_required(VERSION 3.22)

project(
    cppTemplate
    VERSION 1.0.0
    LANGUAGES C CXX
)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

set(LIBRARY mylib)
set(EXECUTABLE exec)
# include
# FetchContent_Declare(
#     googletest
#     GIT_REPOSITORY https://github.com/google/googletest.git
#     GIT_TAG         v1.15.2  # Use the latest stable version or a specific one
# )

# # Prevent GoogleTest from installing itself
# set(INSTALL_GTEST OFF CACHE BOOL "Disable installation of GoogleTest" FORCE)

# # Fetch and make available
# FetchContent_MakeAvailable(googletest)

include_directories(include)
add_subdirectory(src)
add_subdirectory(application)