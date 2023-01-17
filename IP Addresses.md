# IPv4 
  
  ### Required information for a device to connect to a network
  - IPv4 address
  - Subnet mask
  - gateway address
  ---
  ### Meanings of the terms
  
  - IPv4 address
	  - A 32-bit value
	  - usually written in base-10 (decimal system) for human readability
	  - split into 4 8-bit parts called octets and periods seperating them
	  - Octet in base-ten is a value between 0-255 
	  -  Split to 2 portions
	- Network portion
		- Defines the network the device is part of.
	- Device portion 
		- Unique identifier for device recognition

- Subnet mask
	- Defines what part of the ip address is network portion and what is for device portion
	- A 32-bit value
	  - usually written in base-10 (decimal system) for human readability
	  - split into 4 8-bit parts called octets and periods seperating them
	  - Octet in base-ten is a value between 0-255 
  - In binary it masks the IPv4 address
	  - where ones indicate its part of the network portion and zeros indicate the device portion

- Gateway address
	- Usually your closest router
	- Usually the first usable IPv4 address in the network
	- Defines where to send network packets to connect to anything

---

### Example device IPv4 information


|  IPv4 address |  Subnet mask  |   Gateway   |
|:-------------:|:-------------:|:-----------:|
| 10.17.242.152 | 255.255.255.0 | 10.17.242.1 |


---
### Binary numeral system
2<sup>n</sup> System

| 2<sup>7</sup> | 2<sup>6</sup> | 2<sup>5</sup> | 2<sup>4</sup> | 2<sup>3</sup> | 2<sup>2</sup> | 2<sup>1</sup> | 2<sup>0</sup> |
|:----:|:----:|:----:|:----:|:----:|:----:|:----:|:----:|
| 128  | 64   | 32   | 16   | 8    | 4    | 2    | 1    |

#### Example converison base-10 -> binary 8-bit (base-2)

Binary = 0000 1010<sub>b</sub></br>
128\*0+64\*0+32\*0+16\*0+8\*1+4\*0+2\*1+1\*0 = 8+2 = 10
Decimal (base-10) = 10 

(Always provide the the answer in as many bits as told in this case 8-bits if not specified just provide the answer as normal binary number so only everything that you need)

---
### IPv4 Classes
| Class |          IPv4 range         |   Subnet mask   | Subnet Bits |
|:-----:|:---------------------------:|:---------------:|-------------|
|   A   |  1.0.0.0 - 127.255.255.255  | 255.0.0.0       | 8-bit       |
|   B   | 128.0.0.0 - 191.255.255.255 | 255.255.0.0     | 16-bit      |
|   C   | 192.0.0.0 - 223.255.255.255 | 255.255.255.0   | 24-bit      |

- Most used IPv4 class is C-class
- Reserverd IPs
	- First ip address in the range is for only Documentation purposes (Class-A - Class-C: .0)
	-  Last ip address in the range is for Broadcasting (Class-A - Class-C: .255)
	- In Class-A ip range of 127.0.0.0 - 127.255.255.255 is reserved for loopback
- Best practises
	- Use the second ip address in a range for gateway/router, it is the normal in most networks (.1 ending ip address)
- Class-C has sub-classes that are used for special purposes.
	- For additional information about the ranges and subnet masks refer [This](https://www.aelius.com/njh/subnet_sheet.html) 
---
### Example network 
- Network range: 192.168.1.0 - 192.168.1.255
- Subnet mask: 255.255.255.0
-  192.168.1.1 | Gateway
- 192.168.1.2 - 192.168.1.254 | Free to use for any device
- 192.168.1.255 | Broadcast address

## IMPORTANT
"8-bittinen peruna"
