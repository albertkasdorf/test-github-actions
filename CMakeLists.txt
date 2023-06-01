cmake_minimum_required(
    VERSION 3.22
)
project(
    TestGitHubActions
    VERSION 1.0.0.0
    LANGUAGES CXX
)
set(
    TARGET_NAME "main"
)
add_executable(
    ${TARGET_NAME}
    ${CMAKE_CURRENT_SOURCE_DIR}/main.cpp
)
set_target_properties(
    ${TARGET_NAME}
    PROPERTIES
        CXX_STANDARD 11
        CXX_STANDARD_REQUIRED YES
        CXX_EXTENSIONS NO
)
target_compile_features(
    ${TARGET_NAME} PUBLIC cxx_std_11
)