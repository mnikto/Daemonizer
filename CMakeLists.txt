set(target daemonizer)

set(sources
    ${CMAKE_CURRENT_SOURCE_DIR}/service.cc
    ${CMAKE_CURRENT_SOURCE_DIR}/service.h
    ${CMAKE_CURRENT_SOURCE_DIR}/daemon.cc
    ${CMAKE_CURRENT_SOURCE_DIR}/daemon.h)

add_executable(${target} ${sources})

target_include_directories(${TARGET_NAME}
        PRIVATE
            ${CMAKE_CURRENT_SOURCE_DIR})

set_target_properties( ${TARGET_NAME}
        PROPERTIES
            CXX_STANDARD 17)
