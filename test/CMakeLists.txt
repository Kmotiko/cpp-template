add_executable(template_test test_template.cpp)

target_link_libraries(template_test ${Boost_LIBRARIES} cpp_template)

add_test(template_test ${EXECUTABLE_OUTPUT_PATH}/template_test)


