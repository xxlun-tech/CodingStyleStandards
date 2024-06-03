cmake_minimum_required(VERSION 3.12)
project(Test VERSION 0.0.0 LANGUAGES CXX)

set(CMAKE_CXX_FLAGS  "${CMAKE_CXX_FLAGS} -Wall -Wextra")
set(CMAKE_CXX_CLANG_TIDY clang-tidy -checks=-*,performance-*)
set(CMAKE_CXX_CLANG_TIDY clang-tidy -checks=-*,readability-*,-readability-braces-around-statements,-readability-isolate-declaration,-readability-magic-numbers,-readability-else-after-return)
set(CMAKE_CXX_CLANG_TIDY clang-tidy -checks=-*,modernize-*,-modernize-use-trailing-return-type,-modernize-use-auto)
set(CMAKE_CXX_CLANG_TIDY clang-tidy -checks=-*,portability-*)
