include_directories(${PROJECT_SOURCE_DIR}/src/include)

add_executable(server server.cpp)
add_executable(multiple_client multiple_client.cpp)
add_executable(single_client single_client.cpp)
add_executable(thread_test thread_test.cpp)

target_link_libraries(server Server)
target_link_libraries(multiple_client Server)
target_link_libraries(single_client Server)
target_link_libraries(thread_test Server)