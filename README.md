# Lock-Door-System
It is used to make only the people who has a password pass the door and does not for those who do not have a password ,the password is written by the keypad and is displayed on the lcd the ARM MC take this password and transmit it to the AVR MC through the SPI protocol , the AVR authenticates that the password is already saved in the EEPROM which communicate with the AVR through the I2C protocol ,then the AVR returns the result to the ARM with the time and the date using RTC which communicates with the AVR by I2C protocol ,then the ARM opens/closes the door ,and view that to the admin through the UART protocol on the PUTTY terminal . The admin can add , delete or edit this passwords ,and also can open the door manually if he needs that
the Cortex-M4 chip communicating wiht the LCD , the Keypad through digital I/Os and with the Putty terminal through the UART interface 
the AVR chip communicating with the EEPROM and the RTC through the I2C interface 
the Two chip communicating with each other through SPI interface 