project(asset-nxa)
message(STATUS "Project " ${PROJECT_NAME})

set(SRC ${PT_ROOT_MAIN}/asset/nxa/lib)

set(SOURCE_FILES
        ${SRC}/usb-rank.c
        ${SRC}/usb-save.c
        ${SRC}/util.c)

add_library(${PROJECT_NAME} STATIC ${SOURCE_FILES})

target_link_libraries(${PROJECT_NAME} util)
