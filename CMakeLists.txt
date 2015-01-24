cmake_minimum_required(VERSION 2.6)

Project(#[[Project name]])

include(avr.cmake)
add_subdirectory(arduino)

add_executable(${PROJECT} 
    # Sources
)

add_custom_command(TARGET ${PROJECT} POST_BUILD
    COMMAND avr-objcopy -O ihex ${PROJECT} ${PROJECT}.hex)
target_link_libraries(${PROJECT} arduinocore) 



