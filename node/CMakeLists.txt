project(nodeLib)

add_library(node SHARED "Application.cpp" "Application.h"
                 "MP1Node.cpp" "MP1Node.h" )

include_directories(${utilLib_SOURCE_DIR})
include_directories(${netLib_SOURCE_DIR})

target_link_libraries(node "util" "net")

install(TARGETS node DESTINATION lib)
install(FILES "Application.h" "MP1Node.h" DESTINATION include )
