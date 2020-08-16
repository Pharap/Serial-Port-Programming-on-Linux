# Programming the Serial Port on a Linux System using C and `termios` API

<img src="http://xanthium.in/sites/default/files/site-images/serial-prog-linux/serial-programming-in-linux-tutorials.jpg">

--------------------------------------------------------------------------------------------------------------------------------------

- Code for programming the serial port on a Linux System using **ANSI C** and **`termios` API**.
- The code can be used for transmitting and receiving data from an x86 Linux PC and a microcontroller development board through a 3 wire Serial Link (TXD, RXD, GND) or RS232 Port. 


## Online Tutorial

- [Serial Port Programming on Linux using Termios API Tutorial](http://xanthium.in/Serial-Port-Programming-on-Linux)

---------------------------------------------------------------------------------------------------------------------------------------------

 <img src="http://xanthium.in/sites/default/files/site-images/serial-prog-linux/SerialPort-Write.jpeg" alt ="Screenshot of the serial port programming code running on Linux">

--------------------------------------------------------------------------------------------------------------------------------------

## Features

- PC side is written in **ANSI C** using **Terminos API** to communicate with the Serial Port.
- Transmission and reception are kept separate in different C files so that user can easily understand the mechanisms involved.
- PC communicates with MSP430 microcontroller using a 3 wire serial Link (RX,TX,GND).Refer <a href = http://xanthium.in/Serial-Port-Programming-on-Linux> Tutorial for Circuit </a>
- The Microcontroller and PC are connected in **null modem configuration** using  3 signals (TX,RX and Ground).
- Code will work with standard **RS232 Serial ports** or any **USB to Serial Converter**.
- Microcontroller side code is written in **Embedded C** and can be compiled using **Code Composer Studio for MSP430**.
- The hardware used is an MSP430G2553 on a LaunchPad development board.

--------------------------------------------------------------------------------------------------------------------------------------
## Code Explanation

- **serial.c** - A simple C file which opens a connection to Linux Serial Port and closes it. 

- **USB2SERIAL_Read** - **Serial Reception** Program which runs on the Linux PC and receives data from the MSP430 microcontroller. The Received Data is then displayed on Console Window.
  - <img src = "http://xanthium.in/sites/default/files/site-images/serial-prog-linux/SerialPort-Read-String-Received.jpeg"/>

- **USB2SERIAL_Write** - **Serial Transmission** which runs on the Linux PC and Transmits a charcter to the MSP430 microcontroller. The MSP430, upon receiving the character, lights up an LED on the LaunchPad Development board.
  - <img src = "http://xanthium.in/sites/default/files/site-images/serial-prog-linux/SerialPort-Write.jpeg"/>

 -------------------------------------------------------------------------------------------------------------------------------------
 
## Circuit 

- <a href ="http://xanthium.in/Serial-Port-Programming-on-Linux">Available  in the original Tutorial</a>

<img src ="http://xanthium.in/sites/default/files/site-images/serial-prog-linux/MSP430-Connected-to-USB2SERIAL_Marked.jpg"/>

-------------------------------------------------------------------------------------------------------------------------------------

## Hardware used 

- [USB to Serial/RS485 Converter](https://www.xanthium.in/ft232-based-usb-to-serial-rs485-converter-industrial-scientific-applications)
- ![](https://www.xanthium.in/sites/default/files/site-images/usb2rs485-v2-2-product-page/ft232-usb-rs485-converter-v2-2-610px.png)






