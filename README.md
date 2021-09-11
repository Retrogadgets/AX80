AX80

One chip ZX81 based on the Atmega1284p

Under Windows at the command prompt flash the atmega using avrdude with

avrdude -c usbtiny -p m1284p -e -U flash:w:ax81.hex

and set the fuses with

avrdude -c usbasp -F -p m1284p -U lfuse:w:0xe6:m -U hfuse:w:0xd1:m -U efuse:w:0xfc:m

alternatively run the two enclosed .bat files, but ensure the ax81.hex is in the same folder.
