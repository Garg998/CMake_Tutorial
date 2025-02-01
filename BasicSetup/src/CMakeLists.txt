set(LIB_SRC
    HelloWorld.cpp
)

# set(LIB_HEADER
#     HelloWorld.hpp
# )

add_library( ${LIBRARY} STATIC
    ${LIB_SRC}
    # ${LIB_HEADER}
)

# target_include_directories(${LIBRARY} PUBLIC 
#     "/"
# )

target_include_directories(${LIBRARY} PRIVATE
    ${CMAKE_SOURCE_DIR}/include
)