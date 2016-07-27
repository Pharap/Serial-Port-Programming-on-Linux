## Programming the Serial port on a Linux System using C and termios API
<img src="http://xanthium.in/sites/default/files/site-images/serial-prog-linux/serial-programming-in-linux-tutorials.jpg">
--------------------------------------------------------------------------------------------------------------------------------------
Code for programming the serial port on a Linux System using **ANSI C** and **Terminos API**.
The codes can be used for transmitting and receiving data from an x86 Linux PC and a Microcontroller deevelopment board through 3 wire Serial Link or RS232 Port. 

<a href = http://xanthium.in/Serial-Port-Programming-on-Linux>You can find the **original Tutorial** here </a>

<img src="http://xanthium.in/sites/default/files/site-images/serial-prog-linux/SerialPort-Write.jpeg" alt ="Screenshot of the serial port programming code running on Linux">


The Microcontroller and PC are connected in null modem configuration using  3 signals (TX,RX and Ground).

The code uses termios API's to intialize the PC serial port and transmit a character to the microcontroller board.
- The PC side code is written in **C** using **termios API** 
- and can be compiled using **GCC** .

The Code will Work With Standard **RS232 Serial ports** or any **USB to Serial Converter**.

More info about the  <a href = "http://xanthium.in/USB-to-Serial-RS232-RS485-Converter">USB to Serial/RS232/RS485 Converter used in the above tutorial can be found here</a>

<img src = "http://s25.postimg.org/ucb73bztr/usb_to_rs485_converter_250px.jpg"  href="http://xanthium.in/USB-to-Serial-RS232-RS485-Converter"/>

The Microcontroller side code is written in **Embedded C** and can be Compiled using **Code Composer Studio for MSP430**.

The Hardware used is MSP430G2553 on Launch pad development board.
