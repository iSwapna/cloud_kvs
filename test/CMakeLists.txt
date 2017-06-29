project(nodeTest)

add_executable(MainTest  main.cpp)

include_directories(${utilLib_SOURCE_DIR})
include_directories(${netLib_SOURCE_DIR})
include_directories(${nodeLib_SOURCE_DIR})

target_link_libraries(MainTest "node" "net" "util" "gtest_main")

install(TARGETS MainTest DESTINATION bin)
