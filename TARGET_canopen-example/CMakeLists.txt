# Copyright (c) 2020 ARM Limited. All rights reserved.
# SPDX-License-Identifier: Apache-2.0

add_library(mbed-canopen-example INTERFACE)

target_sources(mbed-canopen-example
    INTERFACE
        PeripheralPins.c
)

target_include_directories(mbed-canopen-example
    INTERFACE
        .
)

target_link_libraries(mbed-canopen-example INTERFACE mbed-stm32f091xc)
