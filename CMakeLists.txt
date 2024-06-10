cmake_minimum_required(VERSION 3.29)
cmake_policy(VERSION 3.29)

project(hello LANGUAGES Swift)

add_compile_options(
  $<$<COMPILE_LANGUAGE:Swift>:-v>
  $<$<COMPILE_LANGUAGE:Swift>:-explicit-module-build>)

add_executable(hello Hello.swift)
