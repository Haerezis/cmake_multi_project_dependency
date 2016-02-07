
project("test")
set(INCROOT ${CMAKE_CURRENT_SOURCE_DIR})
set(SRCROOT ${CMAKE_CURRENT_SOURCE_DIR})

include_directories(include)
add_subdirectory(src)
