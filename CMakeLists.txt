cmake_minimum_required(VERSION 3.22)

project(pokemon_box_organizer VERSION 1.0.0 LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

find_package(Qt6 REQUIRED COMPONENTS Widgets)

qt_standard_project_setup()

qt_add_executable(pokemon_box_organizer
    main.cpp
)

target_link_libraries(pokemon_box_organizer PRIVATE Qt6::Widgets)