project(main)

add_subdirectory(hello)
add_subdirectory(world)

add_executable(${PROJECT_NAME} main.cpp)

target_include_directories(${PROJECT_NAME} 
    PUBLIC
    ${Hello_Dir}
    ${World_Dir})

target_link_libraries(${PROJECT_NAME}
    PUBLIC
    hello
    world)