add_library(app_lib
    myclass.cpp
    myclass.h
)
add_executable(app
    launcher.cpp
)
target_link_libraries(app app_lib)
