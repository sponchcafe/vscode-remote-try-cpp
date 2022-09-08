cmake_minimum_required(VERSION 3.18)
project(Demo LANGUAGES CXX)

add_subdirectory(third_party)

if (${BUILD_TESTING})
    enable_testing()
    add_subdirectory("test")
endif()

add_subdirectory(frobnicator)

add_executable(main main.cpp)
#target_link_libraries(main frobnicator)