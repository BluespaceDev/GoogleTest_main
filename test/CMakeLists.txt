cmake_minimum_required(VERSION 3.8)
set(PROJECT GoogleTestMain)

set(SOURCES
    main.cpp
)

add_executable(${PROJECT} ${SOURCES})

target_link_libraries(${PROJECT}
    PUBLIC
        gtest
)

add_test(
    NAME ${PROJECT}
    COMMAND ${PROJECT}
)






