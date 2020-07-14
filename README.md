# I2C-Bus-Routines
Routines for using bit banged I2C on a Z80 SBC.

A collection of I2C routines for communication with various devices.

#TODO
Add routines for reading and writing DS1307 RTC registers in a single block.

Add seperate I2C_RX routine as the previous RX routine sends NACK after a single databyte is recieved. This was fine for the original BLOCK_WR EEPROM routines 
because every byte written to the EEPROM is read back and compared with the original. Having a seperate RX routine means I can choose to either ACK or NACK the I2C device
as needed.

Add seperate ACK routine.

Add seperate NACK routine.

Add seperate RESTART routine.
