cmake_minimum_required(VERSION 3.5)

project(terminal_town LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)


add_executable(chest 
    ${CMAKE_SOURCE_DIR}/chest/main.cpp
    ${CMAKE_SOURCE_DIR}/shared_tools/tools.cpp
)
target_include_directories(chest PRIVATE
    chest
    shared_tools
)

add_executable(hermit
    ${CMAKE_SOURCE_DIR}/hermit/main.cpp
    ${CMAKE_SOURCE_DIR}/shared_tools/tools.cpp
)
target_include_directories(hermit PRIVATE
  hermit
  shared_tools
)

add_executable(magnate 
    ${CMAKE_SOURCE_DIR}/magnate/main.cpp
    ${CMAKE_SOURCE_DIR}/shared_tools/tools.cpp
)
target_include_directories(magnate PRIVATE
  magnate
  shared_tools
)

add_executable(mirror 
    ${CMAKE_SOURCE_DIR}/mirror/main.cpp
    ${CMAKE_SOURCE_DIR}/shared_tools/tools.cpp
)
target_include_directories(mirror PRIVATE
  mirror
  shared_tools
)

add_executable(prisoner 
    ${CMAKE_SOURCE_DIR}/prisoner/main.cpp
    ${CMAKE_SOURCE_DIR}/shared_tools/tools.cpp
)
target_include_directories(prisoner PRIVATE
  prisoner
  shared_tools
)
