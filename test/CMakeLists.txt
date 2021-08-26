add_executable(smftest test.cpp)
target_link_libraries(smftest PortSMF)
add_test(NAME smftest COMMAND smftest)
