
add_library(function function.c)
target_link_libraries(function m)
target_include_directories(function PUBLIC .)

add_executable(taskManager taskManager.c)
target_link_libraries(taskManager function)