cmake_minimum_required(VERSION 3.25)
project(untitled5)

set(CMAKE_CXX_STANDARD 23)

add_executable(untitled5 main.cpp)

install(TARGETS untitled5 RUNTIME DESTINATION bin)

set(CPACK_GENERATOR DEB)

set(CPACK_PACKAGE_VERSION_MAJOR "${1}")
set(CPACK_PACKAGE_VERSION_MINOR "${0}")
set(CPACK_PACKAGE_VERSION_PATCH "${2}")

set(CPACK_PACKAGE_CONTACT example@example.com)

include(CPack)