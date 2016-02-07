
project("foo2")
set(INCROOT ${CMAKE_CURRENT_SOURCE_DIR})
set(SRCROOT ${CMAKE_CURRENT_SOURCE_DIR})

set(${PROJECT_NAME}_INCLUDE_DIRS ${PROJECT_SOURCE_DIR}/include
   CACHE INTERNAL "${PROJECT_NAME}: Include Directories" FORCE)


include_directories(include)
add_subdirectory(src)
