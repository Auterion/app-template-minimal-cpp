cmake_minimum_required(VERSION 3.10.2)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

project({{cookiecutter.app_name}})

add_executable({{cookiecutter.app_name}}
    {{cookiecutter.app_name}}.cpp
)

