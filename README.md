# Anycubic-Mega-TFT-Resource-Converter

This tool converts BMPDATA.BIN and TABLE.BIN to BMP images and vise versa. It allows you to edit images on Anycubic i3 Mega / Mega-S TFT display:
- add translation
- modify backgorunds
- create "themes"

[![IMAGE ALT TEXT](http://img.youtube.com/vi/awsmliBWBBg/0.jpg)](https://youtu.be/awsmliBWBBg "Proof of concept")

# Limitations
- works with version of display older than 03. For version 03, use https://github.com/b-desconocido/Anycubic-Mega-TFT-Resource-Converter
- the maximum size of embedded flash accessible through USB is 16MB
- you can't resize images above the limit 480(W)x320(H)
- you can't remove or add new bitmaps
- if you want to rename a file, you must keep the first number and first underscore at the beggining of the file
- only BMP files are supported
- touch screen areas are hardcoded in MCU's APROM
- dynamic text properties, foreground and background colors, are hardcoded either

# Usage
convert.exe "PathToDirectory" \[-o -i]
- -o - optimize output file size by re-using bitmap data
- -i - ignore all restrictions, might be very unsafe

# How-To
Use it at your own risk! It might damage your display, making it unusable, catch fire or blow apart in thermonuclear explosion!
- connect TFT display to your PC via USB cable
- download all files from display
- make a backup of these files
- drag and drop directory containing BMPDATA.BIN and TABLE.BIN to "covert.exe"
- "Bitmaps" folder will apear, containing all the extracted images
- edit bitmaps you like to change
- drag and drop directory containing images you've edited before to "covert.exe"
- "Resources" folder will apear, containing new BMPDATA.BIN and TABLE.BIN files
- remove old BMPDATA.BIN and TABLE.BIN, do not turn off the display. **Do not remove ASC24DOT.BIN**
- copy new BMPDATA.BIN and TABLE.BIN files from resource directory onto your display. **IT MIGHT TAKE A WHILE, PLEASE, BE PATIENT AND WAIT UNTIL FILES ARE COPIED. DO NOT TURN OFF THE DISPLAY UNTIL FILES ARE COPIED!**
- re-plug the display and enjoy chages you've made

# Binaries
You can get executable [here](https://github.com/belotv/Anycubic-Mega-TFT-Resource-Converter/releases)
