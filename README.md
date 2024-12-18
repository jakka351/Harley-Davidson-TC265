# Harley-Davidson-TC265
Notes on Flashing a Harley Davidson TC265 ECU

![image](https://github.com/jakka351/OpenJ2534/assets/57064943/d7fd8b9d-07d6-46fb-a249-773ad1ed46f7)

# Security Access
Seed & Key Exchange appears to be static, with only one seed and key combination per ECU.

# Read Flash Memory
The Flash Memory read is done via service 0x23 readMemoryByAddress, after unlocking the controller and uploading a secondary bootloader, then activating it.
## Upload Secondary Bootloader

# Write Flash Memory
The Flash Write process uses service 0x34 requestDownload and service 0x36 transferData to write to the flash memory.
