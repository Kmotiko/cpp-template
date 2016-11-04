set(EXECUTABLE_OUTPUT_PATH ${PROJECT_SOURCE_DIR})
add_executable(template main.cpp)
target_link_libraries(template
              cpp_template
              )
install(TARGETS template DESTINATION bin)

add_subdirectory(cpp_template)
