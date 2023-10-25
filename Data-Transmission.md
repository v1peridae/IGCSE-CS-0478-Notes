# Methods of Data Transmission
- There are 5 main methods of data transmission:
1. Serial - This is where data is transferred using a single wire one bit at a time. 

| Advantages                     | Disadvantages                                             |
| ------------------------------ | --------------------------------------------------------- |
| Arrive in order                | Slower                                                    |
| Less chance of interference    | Additional data (start bit and stop bit) needs to be sent |
| Cheaper to buy and manufacture |                                                           |

- Serial transmission is suitable for long distance transmissions

2. Parallel - This is when multiple bits of data are transmitted using multiple wires at the same time.

| Advantages                                      | Disadvantages                                             |
| ----------------------------------------------- | --------------------------------------------------------- |
| Quicker                                         | Needs to be reordered increasing the risk of being skewed |
| No need to convert to transfer across a network | Chance of interference                                    |
|                                                 | More expensive to manufacture and buy                                                          |
- It is limited to 5 metres due to the increased chance of data being skewed

3. Simplex - This is when data is transferred from one device to another in one direction only. It is mostly used when there is no need to send data in both ways eg. connecting a keyboard to a computer
4. Half-duplex - This is when data can be transmitted in both directions but one direction at a time. An example is Wi-Fi
5. Full-duplex - This is when data can be transmitted in both directions at the same time. An example is a telephone conversation

# USB
- USB is used to describe different aspects not just the cable. 
- A USB interface includes:  a USB port, a USB cable, a USB connection and a USB device.
- A USB connection uses serial data transmission ot transmit data between the devices.
- We are currently in the 4th version of USB

| Advantages                      | Disadvantages                                                 |
| ------------------------------- | ------------------------------------------------------------- |
| It is a simple interface        | The length of USBs is limited to 5 meters                     |
| The speed is relatively high    | It isnt as fast as other types of connection such as ethernet |
| It is a universal standard      |                                                               |
| It is automatically detected    |                                                               |
| It can be used to power devices |                                                               |

# Detecting Errors in Data Transmission
- When data is transferred interference can occur.
- This can cause data to be gained. lost or changed.
- Accuracy of data is often vital therefore there needs to be a procedure to detect any errors in data.
- There are several error detection methods that can be used, these include:
<h3>1. Parity check</h3>
- A parity check can use an odd or even check method. Each byte of data has 7 bits + 1 parity bit. It is usually either the first or last digit. 
                                                  **1**0010001
- When an odd parity check is used, 1 is added as a parity bit. This is because all the 1s now add up to 3, which is an odd number. If an even parity check is used, 0 is added as the parity bit as the 1s and 0s would all be even. An error is detected when an odd or even parity check is used but an even or odd (respectively) is found.

<h3>2. Checksum</h3>
- A value is calculated from the data that will be transmitted before transmission takes place. A method such as modulo 11 could be used. 
- Once the checksum value has been calculated it is added to the data to be transmitted with it. After transmission, the receiving device uses the same method to calculate a value from the received data. If the values match, then the device knows that no error has occurred during transmission

<h3>3. Echo check </h3>
- This is simply a comparison of the data sent to the data received. 
- The sending device transmits the data to the
5. Check Digit
6. ARQ

# Structure Of A Data Packet

- The amount of data that is stored in a file can be large.
- Sometimes its way too large to be transmitted from one device to another all at once. 
- For the data to be transmitted, it is broken down into very small units called **packets**
- Packets contain 3 parts:

|         |
| ------- |
| Packet Header |     
| Payload |
| Trailer |


- A **packet header** contains a lot of information about the data closed in a packet and its destination. The info includes:
1. Destination address - The IP address of the device where the data is being sent
2. Packet number - When transmitting data, it might not go in the right order. This helps put the data in order once it reaches the destination
3. Originators address - The IP address where the data has originally been sent from. This is used to trace where data is from
- The **payload** is the actual data being sent. It is broken into smaller units to be sent as the payload in each packet
- The trailer is also known as the footer. It contains a marker to indicate that is the end of a packet and data for any data error detection

# Packet Switching
- The process of transmitting these packets is called packet switching. 
- Each packet of data is sent individually from one device to another

- There would be several pathways across a network that the packets could be transmitted.
- Each data packet could be sent along a different pathway. 
- A router is a device that controls which pathway will be used to transmit each packet.

- When packets are transferred, it is likely that the packets will arrive out of order. Once all packets have arrived, they are reordered to recreate the file.
