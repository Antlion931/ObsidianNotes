#embedded 
# SPI Protocol
- SCLK/SLK - clock band
- MOSI - master output, slave input
- MISO - master input, slave output
- SS - slave select

## Example
LCD connected to microcontrolel

![[SPI_image.png]]

## Sending data
Data is changed in certain point of time, signalazed by changing clock, and read at different.

![[SPI_data_reading.png]]

However what change in clock cases what, depends, there are different combinations.

![[SPI_types.jpeg]]

CPOL say wheres idle state of clock is high or low, CPHA says if change should happens when returning to idle state or from it.

## Modifications
- master can communicate with only 4 bands, to a lot of slave, when slaves are addressed and firstly we send address of slave we want to interact with.
- We can separate them
#todo add 2 more from presentation
# One-wire Protocol
It is two-way, half duplex, protocol. There are 2 lines, GND and DATA, so there is only one data that sends information. It is also master-slave

#todo Write about one-wire protocol