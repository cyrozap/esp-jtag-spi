# esp-jtag-spi

This is a simple Wi-Fi JTAG and SPI adapter based on the ESP-12E module. This
project was inspired by the [WIFI-JTAG][1] project with the goal of
implementing simultaneous JTAG and SPI interfaces in the ESP-12E using
[esp-open-rtos][2].

## Development

Assuming you already have the [esp-open-sdk][3] installed with the
xtensa-lx106-elf toolchain in your `PATH`, clone this repository using the
following command:

    git clone --recursive https://github.com/cyrozap/esp-jtag-spi.git
    cd esp-jtag-spi

If you already cloned the repository but did not do it recursively, change to
the project directory and run:

    git submodule update --init --recursive

## Pinout

  PIN | ESP-12E | NodeMCU
------|---------|--------
 TMS  | GPIO2   | D4
 TCK  | GPIO0   | D3
 TDO  | GPIO4   | D2
 TDI  | GPIO5   | D1
 CS   | GPIO15  | D8
 MOSI | GPIO13  | D7
 MISO | GPIO12  | D6
 SCLK | GPIO14  | D5


[1]: https://github.com/emard/wifi_jtag
[2]: https://github.com/SuperHouse/esp-open-rtos
