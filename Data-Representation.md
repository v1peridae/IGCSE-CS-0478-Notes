# Number Systems
-   There are 3 number systems
  a. Denary
  b. Binary
  c. Hexadecimal
<h2><u>Binary</u></h2>
- The components that process data in a computer are made up of very small **logic gates**
- This data is stored in registers
- Digital data is discrete. It is made up of 1s and 0s. 
- An example of a binary number is 10010110
<h2><u>Denary</u></h2>
- We use denary in our daily lives. 
- Its a base 10 number system and uses the digits 0-9
- The units of the denary system are ones, tens, hundreds and thousands.
- Any denary values can be converted into binary 
- An example of a denary number is 420
<h3><u>Converting between denary and binary</u></h3>
- The size of a binary number is referred to by the number of bits it has
- A 4-bit binary number will have 4 values, an 8-bit will have 8 values and so on
- To convert denary to 4-bit, you need the units 1,2,4,8

	Example 1.1:
150 in 8-bit

| 128 | 64  | 32  | 16  | 8   | 4   | 2   | 1   |    
| --- | --- | --- | --- | --- | --- | --- | --- |
|  1  |  0  |  0  |  1  | 0   | 1   |1    | 0   |  

- If the denary you're converting ends in a 1, its an odd number, if it ends in a 0 its even.
- To convert from binary to denary, you just reverse it
<h2><u>Hexadecimal</u></h2>
- Hexadecimal is a base 16 system and uses 16 symbols, these are the the numbers 0-9 and letters A-F
- This allows the denary values of 0-15 to be represented.

| Denary            | 0   | 1   | 2   | 3   | 4   | 5   | 6   | 7   | 8   | 9   | 10  | 11  | 12  | 13  | 14  | 15 |
| ------ | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | 
| Hexadecimal       |  0  |  1  |  2  |  3  |  4  |  5  |  6  |  7  |  8  |  9  |  A  |  B  |  C  |  D  |  E  |  F  |

*Table 1*
<h3><u>Converting denary to hexadecimal</u></h3>
- To Convert denary to hexadecimal, you need to convert it into binary first
	Example 1.2:
 12 in 4-bit
 
|  8  |  4  |  2  |  1  | 
| --- | --- | --- | --- |
|  1  |  1  |  0  |  0  |

- Binary for this is 1100
- On Table 1, you can convert this making it C

	Example 1.3:
201 in 8-bit
  
| 128 | 64  | 32  | 16  |  8  |  4  |  2  |  1  |  
| --- | --- | --- | --- | --- | --- | --- | --- |
| 1   |  1  |  0  |  0  |  1  |  0  |  0  |  1  |     

- Each hexadecimal symbol only uses 4-bits meaning you need to split the table into 2
- Convert each 4-bit into binary 
	8 + 4 = 12
	8 + 1 = 9
- The hexadecimal for 12 is C and the hexadecimal for 9 is 9 therefore 201 in hexadecimal is C9


# Binary Manipulation 
<h2><u> Binary Addition </u></h2>
**Rules:**
1. 0+0 = 0
2. 1+0 = 1
3. 1+1 = 10
4. 1+1+1 = 11

	Example 1.1
Add 10010100 and 00011110

  10010100
+00011110
**=10110010**
<h2><u>Overflow Error</u></h2>
- This is a type of error that occurs when a number larger than a register can store is generated
- Computers have a pre-defined limit for instance 16-bit
- When an overflow error happens, the number is bigger than 16-bits

<h2><u>Logical Binary Shifts</u></h2>
- This is a type of process that shifts the binary values to the left or to the right.
- Binary shifts to the right means a zero is added at the furthest left point
	Example 1.2:
1. Perform a logical binary shift one place to the left to the number 0 0 1 0 0 1 1 1
  - To the left means we add a zero to the furthest right point.
  - Hence it will be 0 1 0 0 1 1 1 0
<h2><u>Negative Binary Numbers</u></h2>
To convert negative numbers to binary you need to use the two complement system. The example below shows how to use it. 
	Example 1.3:
Convert -35 to a negative number
1. Convert 35 to a binary number
 0 0 1 0 0 0 1 1
2. Invert each of the values in the binary number
 1 1 0 1 1 1 0 0
3. Add 1
 1 1 0 1 1 1 0 1
 
# How Computers Represent Text, Images and Sound
 <h2>Converting text to binary</h2>
- When a computer converts text to binary to be processed it uses a tool called a character set. 
- There are two main types of character sets:
1. ASCII 
2. Unicode
- ASCII uses 8-bit. This means that it can represent up to 256 characters (0-255)
- Unicode uses 16-bit. This means it can represent aprox. 65,000 characters
- Each character has a set binary value.

<h2><u>Converting images to binary</u></h2>
- An image is made up of tiny dots called pixels
- If each image is converted into its binary value, a data set is created
- The type of data that is used to provide information such as the dimensions and resolution is called metadata
- Colours are created by computer screens using the RGB colour system
- Most images are made using thousands of pixels
- Each image has a resolution and colour depth
- **The resolution is the number of pixels wide and high used to create the image**
- The greater number of bits, the greater range of colour in an image
- If the resolution is changed, this will affect the size of image

<h2><u>Converting sound to binary</u></h2>
- Sound is made up of sound waves
- When sound is recorded it is done at a set **time** **intervals**. This process is called **sound sampling** 
- For sound to be accurate, more samples need to be taken each second. The number of samples taken per second is called the **sample rate**
- Sample rates are measured in hertz
- 1 hertz = 1 sample per second
- A common sample rate is 44.1khz. This mean 44,100 samples are taken each second!
- If a sample is increased, the amount of data needed is increased too!
- **Sample resolution** is the number of bits needed to represent each sample. A common sample resolution is 16-bit.

# Measuring Data Storage
| Unit             | Description    |
| ---------------- | -------------- |
| Bit              | Smallest       |
| Nibble           | 4-bits         |
| Byte             | 8 bits         |
| Kibibyte (KiB)   | 1024 bytes     |
| Mebibyte (MiB)   | 1024 kibibytes |
| Gibibyte   (GiB) | 1024 Mebibytes |
| Tebibyte (TiB)   | 1024 Gibibytes |
| Pebibytes (PiB)  | 1024 Tebibytes |
| Exibytes (EiB)   | 1024 Pebibytes |

<h2>Calculating the size of a file</h2>
Image size - width of image x height of image x colour depth x number of images
Sound size - sample rate x sample resolution x length of soundtrack

# Data Compression
- Benefits of compression:
1. Reduced storage space consumed
2. Less time needed to transmit from one device to another
3. It os quicker to upload and download
4. Not as much bandwith needed to transmit it over the internet

- There are two types of compression: lossy and lossless.
- Lossy - A compression that reduces the size the method that reduces the size of a file by permanently removing data
- Lossless - A compressiom that reduces the size of a file by temporarily altering data


