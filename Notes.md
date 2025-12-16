\[Datasheet](https://documentation.espressif.com/esp32-s3-wroom-1\_wroom-1u\_datasheet\_en.pdf)



Strapping pins are read after EN pin goes high.

GPIO0 and GPIO46 are needed to control which mode the ESP32 boots into.

GPIO0 has a weak pullup and GPIO46 has a weak pull-down. (13)



To boot normally and execute the program stored in SPI flash: GPIO0 is high and GPIO46 is any value. (14)



To boot into Joint Download Boot mode, GPIO0 must be 0 and GPIO46 must be 0. (14)

The program can then be flashed over USB interface.

