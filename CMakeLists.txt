cmake_minimum_required(VERSION 3.3)

project(boost_utility)

add_library(boost_utility INTERFACE)

target_include_directories(boost_utility BEFORE INTERFACE ${CMAKE_CURRENT_SOURCE_DIR}/include)

install(TARGETS boost_utility DESTINATION lib)
install(DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}/include/boost DESTINATION include)
