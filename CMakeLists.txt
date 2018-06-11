    cmake_minimum_required (VERSION 2.6)
    project(stb)
    
    add_library(${PROJECT_NAME} STATIC stb_vobis.c)

    install ( TARGETS ${PROJECT_NAME} DESTINATION lib )
    file(GLOB HEADER_FILESS "*.h" "*.hpp")
    install ( FILES ${HEADER_FILESS} DESTINATION include/${PROJECT_NAME} )
