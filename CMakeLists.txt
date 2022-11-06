cmake_minimum_required(VERSION 3.21)
project(cheapglk)

add_library(cheapglk STATIC
    cgblorb.c
    cgdate.c
    cgfref.c
    cggestal.c
    cgmisc.c
    cgschan.c
    cgstream.c
    cgstyle.c
    cgunicod.c
    cgwindow.c
    gi_blorb.c
    gi_debug.c
    gi_dispa.c
    main.c
    )

set_target_properties(cheapglk PROPERTIES C_STANDARD 99)

target_include_directories(cheapglk
    PUBLIC
    ${CMAKE_CURRENT_SOURCE_DIR}
    )
