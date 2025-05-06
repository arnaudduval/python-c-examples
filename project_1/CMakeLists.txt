cmake_minimum_required(VERSION 3.18)
project(mymodule LANGUAGES CXX)

# Trouver pybind11 via le module Python (fourni par scikit-build-core)
find_package(pybind11 CONFIG REQUIRED)

pybind11_add_module(mymodule mymodule/mymodule.cpp)