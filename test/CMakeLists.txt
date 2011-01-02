include_directories(${CMAKEPRIMER_SOURCE_DIR}/include)
include_directories(${CMAKE_CURRENT_SOURCE_DIR}/../../../../googletest/include)

link_directories(${CMAKEPRIMER_BINARY_DIR}/src)
link_directories(${CMAKE_CURRENT_SOURCE_DIR}/../../../code/gtestBuild)

add_executable(test CarTest.cpp)

target_link_libraries(test Car gtest gtest_main)