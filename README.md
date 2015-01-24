# cmakeduino
Skeleton project for those who want to use some Arduino snippets in their projects

very basic configuration require editing target in `CMakeLists.txt` and the following lines in `avr.cmake`:
```CMake
SET(CMCU "-mmcu=atmega32u4")
SET(ARDUINO_VARIANT "leonardo")
SET(CDEFS "-DF_CPU=16000000")
```
where `ARDUINO_VARIANT` should match appropriate subdirectory in `arduino/variants/`, so it should be one of
the following: 
```
eightanaloginputs
ethernet
leonardo
mega
micro
robot_control
robot_motor
standard
```
