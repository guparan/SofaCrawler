cmake_minimum_required(VERSION 3.1)
project(SofaCrawler)

find_package(SofaFramework REQUIRED)
find_package(SofaBase REQUIRED)
find_package(SofaCommon REQUIRED)
find_package(SofaGeneral REQUIRED)
find_package(SofaAdvanced REQUIRED)
find_package(SofaMisc REQUIRED)

add_executable(${PROJECT_NAME} main.cpp)
target_link_libraries(${PROJECT_NAME} SofaComponentBase SofaComponentCommon SofaComponentGeneral SofaComponentAdvanced SofaComponentMisc)
