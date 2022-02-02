cmake_minimum_required(VERSION 3.21)
project(Qt_WireShark)

set(CMAKE_CXX_STANDARD 14)
set(CMAKE_AUTOMOC ON)
set(CMAKE_AUTORCC ON)
set(CMAKE_AUTOUIC ON)

find_package(Qt5 COMPONENTS
        Core
        Gui
        Widgets
        REQUIRED)

add_executable(Qt_WireShark main.cpp mainwindow.cpp mainwindow.ui)
target_link_libraries(Qt_WireShark
        Qt5::Core
        Qt5::Gui
        Qt5::Widgets
        )

