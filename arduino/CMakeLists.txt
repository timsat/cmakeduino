include_directories(variants/${ARDUINO_VARIANT} ./)

add_library (arduinocore STATIC
    WInterrupts.c
    wiring_analog.c
    wiring.c
    wiring_digital.c
    wiring_pulse.c
    wiring_shift.c
    CDC.cpp
    HardwareSerial.cpp
    HID.cpp
    IPAddress.cpp
    #    main.cpp
    new.cpp
    Print.cpp
    Stream.cpp
    Tone.cpp
    #    USBCore.cpp
    WMath.cpp
    WString.cpp
)

