# add_subdirectory(# directory)

add_library(dingo STATIC ${ALL_OBJECT_FILES})

set(DINGO_LIBS
    # directory
        )

set(DINGO_THIRDPARTY_LIBS
        # library
        )

target_link_libraries(
        dingo 
        ${DINGO_LIBS}
        ${DINGO_THIRDPARTY_LIBS}
    )

target_include_directories(
        dingo PUBLIC $<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}/include>
        $<INSTALL_INTERFACE:${CMAKE_INSTALL_INCLUDEDIR}>)
