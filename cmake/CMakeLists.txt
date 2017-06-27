cmake_minimum_required(VERSION 3.6)
project(archmage_googletest)

include(ExternalProject)
ExternalProject_Add(googletest
  GIT_REPOSITORY https://github.com/google/googletest
  CMAKE_ARGS
  -DCMAKE_INSTALL_PREFIX=${CMAKE_INSTALL_PREFIX}
  -DBUILD_GTEST=ON -DBUILD_GMOCK=OFF
#  -Dgtest_disable_pthreads=ON
#  -Dgtest_force_shared_crt=ON
  -DBUILD_SHARED_LIBS=ON
  )