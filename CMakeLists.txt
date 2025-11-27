cmake_minimum_required (VERSION 3.28)
project (OtaryxDemo)

set(CMAKE_CXX_STANDARD_REQUIRED ON)

find_package(Qt6 REQUIRED COMPONENTS Quick)

qt_standard_project_setup(REQUIRES 6.8)

qt_add_executable(otaryx_demo
    main.cpp
)

qt_add_qml_module(otaryx_demo
    URI testje
    VERSION 1.0
    QML_FILES
        Main.qml
)


target_link_libraries(otaryx_demo
    PRIVATE Qt6::Quick
)

install (TARGETS otaryx_demo DESTINATION /usr/bin)
