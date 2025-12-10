# INSTALLATION GUIDE:

## REQUIREMENTS:
- Raspberry Pi 4B
- Game HAT interface (Has Joysticks buttons and screen)
- Power supply (18650 battery)
- Optional: 3D-printed case from Thingiverse
- (Model: Thingiverse Model ID: 3752237)
- MicroSD
- HDMI connector compatible with your Raspberry Pi model

## SOFTWARE:
- Raspberry Pi OS (32-bit recommended)
- RetroPie OS
- DosBox Emulator
- Game Hat Driver (from Waveshare Wiki)
- X11 session (required to allow RetroPie to work properly on Raspberry Pi OS)
- Fallout 1 and Fallout 2 Linux-compatible installers

## STEPS TO INSTALLATION:


### Raspberry Pi OS (SETUP):

1. On a laptop/PC, download "Raspberry Pi Imager".
2. Insert your microSD card.
3. In the imager:
   - Choose OS → Raspberry Pi OS (32-bit recommended)
   - Choose Storage → your SD card
   - Flash the card.

4. Insert SD card into the Raspberry Pi and boot it.
5. Complete the setup (language, WiFi, etc.).
6. Update everything:
       sudo apt update && sudo apt upgrade -y

NEXT

## Installing GameHat Driver:
- Download the correct RetroPie image for your Raspberry Pi model:
- RetroPie Image for Pi 4
- RetroPie Image for Pi 2/3
- RetroPie Image for Pi 1/Zero

- Unzip the downloaded .zip file to obtain the .img file.

- Insert your microSD card into your computer.

- Use a flashing tool (such as Raspberry Pi Imager or Win32DiskImager) to write the RetroPie .img file to the microSD card.

- Insert the prepared microSD card into the Raspberry Pi.

- Connect the Raspberry Pi to the Game HAT:

- Attach the Raspberry Pi to the Game HAT’s GPIO header

- Connect the correct HDMI adapter between the Pi and the Game HAT screen
- (Note: Game Hat includes different adapters; ensure you are using the correct one for your Pi model.)
- Toggle the Game HAT Battery switch to ON.

## IMPORTANT TO NOTE:If the battery is low, RetroPie may not boot

- You can connect a 5V/2A charger to power and charge the device. The charge indicator will blink while charging.

- RetroPie will boot into its main interface.

- Use the joystick to navigate emulator categories

- Press A to select options

- Find the button configuration tab and configure the buttons to your liking

- Press Exit to close the OSD menu

## To set up the wifi 
- In retroPie open the wifi setup tool
- When asked for "ESSID", enter your Wi-Fi network name manually, then enter your password
- The system will then assign you an IP address.
