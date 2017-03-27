# Description
Original tools

# list
## simple_usbkeyboard_decoder.py
Decode formatted usb keyboard data to string.

### Usage
If you have usb keyboard packet capture data,  
$ tshark -r ./keyboard.pcap -T fields -e usb.capdata usb.capdata and usb.device_address==3 > data.txt  
$ python simple_usbkeyboard_decoder.py data.txt  

## asmshell.py
Command line assembler emulator. TO USE, NEED UNICORN(https://github.com/unicorn-engine/unicorn)  
Emulate all architecture implemented in unicorn engine.(Now x86 only)

### Usage
$ python ./asmshell.py
> xor eax,eax
