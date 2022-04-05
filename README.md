ABNielsen.com 6502 Single Board Computer R1

This is a 6502-based complete single board computer intended to help during the global IC shortage. Why use new chips when you can reuse scrap?

Video about the wireless bootloader: https://youtu.be/NABU7gQDtcs

Check out the NEW project on HackADay if you want to read more and see some pretty pictures :)

https://hackaday.io/project/184725-abn6502-sbc-r1

For R1 I got rid of the Padauk MCU without increasing the chip count!

Build instructions:

1) Send gerber files from /hardware to your favorite board house
2) Build the project using assemble.sh - this will also try to burn the main ROM using Minipro. Dependencies: [CC65] (https://github.com/cc65/cc65) and a way to burn the ROM's.
3) Source the IC's - the spirit of this project is to contribute as little as possible to the global IC shortage and get used chips locally or from Ebay/AliExpress/etc.
4) Burn the ROMs. I use a TL866II Plus variant for the actual ROMs.
5) Solder away
6) For the PS/2-keyboard I use Ben Eater's (a.k.a. Dieter Müller's) interface: https://www.reddit.com/r/beneater/comments/mjeilv/keyboard_interface_diagram/
7) Enjoy!

Optional:
Setup SSH keys with a Raspberry Pi, connect an nRF24L01+ compatible module to it and compile the wireless bootloader code in /software_linux

License: Attribution-NonCommercial 4.0 International (CC BY-NC 4.0) https://creativecommons.org/licenses/by-nc/4.0/
