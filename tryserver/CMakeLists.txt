cmake_minimum_required(VERSION 2.6)
project(tryserver)

add_executable(tryserver tryserver.c)

target_link_libraries(tryserver PUBLIC pthread sqlite3)

install(TARGETS tryserver RUNTIME DESTINATION bin)
