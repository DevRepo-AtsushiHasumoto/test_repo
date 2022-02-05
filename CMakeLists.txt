cmake_minimum_required(VERSION 3.10)

project(test_repo)

set(CMAKE_CXX_FLAGS "")
set(CMAKE_EXPORT_COMPILE_COMMANDS "1")

include_directories(
  Includes
  /usr/local/include
  )

link_directories(
  /usr/local/lib
  )


file(GLOB SOURCES Sources/*.cpp)


add_executable(
  test01
  ${SOURCES}
  )

target_link_libraries(
  test01
  )
