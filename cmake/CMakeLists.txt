cmake_minimum_required(VERSION 3.6)
project(archmage_googletest)

include(ExternalProject)

ExternalProject_Add(googletest
  GIT_REPOSITORY https://github.com/google/googletest
  CMAKE_ARGS -DCMAKE_INSTALL_PREFIX=bin
  )