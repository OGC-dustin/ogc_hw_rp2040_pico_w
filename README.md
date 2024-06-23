# OGC.Engineering
### ogc_hw_rp2040_pico_w - hardware description for the Raspberry Pi RP2040 Pico-W controller
developer contact - dustin ( at ) ogc.engineering

---

# Description:
* Hardware description definitions for OGC.Engineering C based layered development
* Development controller Raspberry Pi RP2040 Pico-W
* Documentation can be found at https://www.raspberrypi.com/documentation/microcontrollers/raspberry-pi-pico.html
* Features:
```
RP2040 ( 2MB Flash, 3 pin Arm Serial Wire Debug ( SWD ) )
      
      UART0_TX, I2C0_SDA, SPI0_RX, GP0 - [ 01 ][ 40 ] - VBUS
     UART0_RX, I2C0_SCL, SPI0_CSn, GP1 - [ 02 ][ 39 ] - VSYS
                                   GND - [ 03 ][ 38 ] - GND
               I2C1_SDA, SPI0_SCK, GP2 - [ 04 ][ 37 ] - 3V3_EN
                I2C1_SCL, SPI0_TX, GP3 - [ 05 ][ 36 ] - 3V3( OUT )
      UART1_TX, I2C0_SDA, SPI0_RX, GP4 - [ 06 ][ 35 ] - ADC_VREF
     UART1_RX, I2C0_SCL, API0_CSn, GP5 - [ 07 ][ 34 ] - GP28, ADC2
                                   GND - [ 08 ][ 33 ] - GND, AGND
               I2C0_SDA, SPI0_SCK, GP6 - [ 09 ][ 32 ] - GP27, ADC1, I2C1_SCL
                I2C1_SCL, SPI0_TX, GP7 - [ 10 ][ 31 ] - GP26, ADC0, I2C_1_SDA
      UART1_TX, I2C0_SDA, SPI1_RX, GP8 - [ 11 ][ 30 ] - RUN
     UART1_RX, I2C0_SCL, SPI1_CSn, GP9 - [ 12 ][ 29 ] - GP22
                                   GND - [ 13 ][ 28 ] - GND
              I2C1_SDA, SPI1_SCK, GP10 - [ 14 ][ 27 ] - GP21, I2C0_SCL
               I2C1_SCL, SPI1_TX, GP11 - [ 15 ][ 26 ] - GP20, I2C0_SDA
     UART0_TX, I2C0_SDA, SPI1_RX, GP12 - [ 16 ][ 25 ] - GP19, SPI0_TX, I2C1_SCL
    UART0_RX, I2C0_SCL, API1_CSn, GP13 - [ 17 ][ 24 ] - GP18, SPI0_SCK, I2C1_SDA
                                   GND - [ 18 ][ 23 ] - GND
              I2C1_SDA, SPI1_SCK, GP14 - [ 19 ][ 22 ] - GP17, SPI0_CSn, I2C0_SCL, UART0_RX
               I2C1_SCL, SPI1_TX, GP15 - [ 20 ][ 21 ] - GP16, SPI0_RX, I2C0_SDA, UART0_TX

Infineon 43439 ( 2.4GHz 802.11n, part number: CYW43439 )
    LED on WL_GPIO0
```
