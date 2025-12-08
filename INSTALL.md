INSTALLATION GUIDE:





REQUIREMENTS:
- Raspberry Pi 
- Game HAT interface (Has Joysticks buttons and screen)
- Power supply (4A battery)
- Optional: 3D-printed case from Thingiverse
- (Model: Thingiverse Model ID: 3752237)
- MicroSD

SOFTWARE:
- Raspberry Pi OS (32-bit recommended)
- Box86
- Box64
- Wine
- AntiMicroX
- Fallout 1 and Fallout 2 Linux-compatible installers

STEPS TO INSTALLATION:


Raspberry Pi OS (SETUP):

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

Install Needed Dependencies:

- Needed Dependencies for Box86/64
    sudo dpkg --add-architecture i386
    sudo apt update
    sudo apt install git cmake build-essential python3 -y
    sudo apt install libgl1-mesa-dev libsdl2-dev -y
    git clone https://github.com/ptitSeb/box86
-
-Install Box86
    cd box86
    mkdir build && cd build
    cmake .. -DRPI4=1 -DCMAKE_BUILD_TYPE=RelWithDebInfo
    make -j4
    sudo make install
    sudo systemctl restart systemd-binfmt
-
-Install Box64
    cd ~
    git clone https://github.com/ptitSeb/box64
    cd box64
    mkdir build && cd build
    cmake .. -DRPI4=1 -DCMAKE_BUILD_TYPE=RelWithDebInfo
    make -j4
    sudo make install
    sudo systemctl restart systemd-binfmt
-
-Install Wine
    sudo dpkg --add-architecture i386
    sudo apt update
    sudo apt install wine wine32 wine64 -y
    winecfg
-
-Install Antimicrox
    sudo apt install antimicrox -y
-


PREPARE FOR FALLOUT GAME FILES

Create a folder:

    mkdir ~/fallout
    cd ~/fallout

Copy GOG installers into this folder
setup_fallout_1.exe
setup_fallout_2.exe

INSTALL FALLOUT:
In the cmd
wine setup_fallout_1.exe
wine setup_fallout_2.exe


Configure controls
Open antimicrox and perform the following changes

Map:
- D-Pad → Arrow keys / WASD  
- Buttons → Enter, Space, etc.
- Joystick → Mouse movement, Mouse click (when pressed downwards)

Launch the games