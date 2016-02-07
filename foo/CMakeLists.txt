project("foo")

add_subdirectory(foo1)
add_subdirectory(foo2)

set(${PROJECT_NAME}_INCLUDE_DIRS ${foo1_INCLUDE_DIRS} ${foo2_INCLUDE_DIRS}
   CACHE INTERNAL "${PROJECT_NAME}: Include Directories" FORCE)

add_library(foo INTERFACE)
target_link_libraries(foo INTERFACE foo1 foo2)
