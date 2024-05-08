#embedded #pwr 

**U**niversal **A**synchronous **R**eceiver and **T**ransmitter is not a communication protocol, but a physical circuit in a micro controller. A [[UART]]’s main purpose is to take bits in parallel, transmit them in series, then other [[UART]] micro controller will receive it and make it parallel again. It main advantage is that it only uses 2 wires, without need for a clock.

![[UART_in_work.png]]

## Why it doesn't need clock?
Before transmitting/receiving data, you need to choose or set some baud rate (usually 9600 bits per second). Then one device send start bit, which is low voltage unlike default state (this is because it is more obvious when there is other device on the other end, and when is not). Then it sends bits one by one, and ends it with end bit or bits.

![[UART_sending_data.png]]

## Data Packets
Data is transited in packets.
![[UART_data_packet.png]]

Data frame could be 8 bit long if parity bit is used, or as long as 9 bits if there is no parity bit.

### Why there is a stop bit?
It is good question, if every packet is the same size, and we already have a start bit to synchronise devices, why there is a stop bit necessary? It wouldn't be necessary if we lived in perfect world, but we are not living in one. Connection could be started while there is already packet in wire, or start bit was missing.

Take a look at this: **0 xxxx xxxx 1 ...**
We can be almost sure that it is correct packet, however if we got something like this: **0 xxxx xxxx 0 ...**
We know that it is not whole packet, so we left shift, and try to match our pattern of **start(0) data(xxxx xxxx) end(1)**. So it is used to synchronise devices and another way of checking if data was corrupted.
