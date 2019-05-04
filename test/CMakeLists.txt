include_directories(${app_SOURCE_DIR}/src)
include_directories(${gtest_SOURCE_DIR}/include ${gtest_SOURCE_DIR})
include(GoogleTest)

add_executable(app_test
    test1_test.cpp
)
target_link_libraries(app_test
    app_lib
    gtest
    gtest_main)
gtest_add_tests(TARGET app_test)

