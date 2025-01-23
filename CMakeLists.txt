cmake_minimum_required(VERSION 3.10)
project(my_library)

set(CMAKE_CXX_STANDARD 14) # Adjust as needed

add_library(my_library SHARED ${SRC_FILES})

target_link_libraries(my_library PUBLIC ${LIBS}) 

# Optional: Specify include directories
target_include_directories(my_library PUBLIC ${INCLUDE_DIRS}) 
