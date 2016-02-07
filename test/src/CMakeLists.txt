set(INCROOT ${INCROOT}/include)
set(SRCROOT ${SRCROOT}/src)

add_executable(test
  ${SRCROOT}/test.cpp
  ${SRCROOT}/main.cpp
)

add_definitions(${bar_DEFINITIONS})

include_directories(${foo_INCLUDE_DIRS})
include_directories(${bar_INCLUDE_DIRS})

target_link_libraries(test foo bar)
