# CHOICES

November 20th 2025  
Ehsan Hussain & Luca Ragosta

#### Basic Idea:
For the project concept, we decide to build a portable Linux based handheld console using raspberry pi alongside a game HAT interface.
We chose this idea because we (Luca and Ehsan) both found it quite interesting and fun to build a handheld console like the steamdeck or 
the Nintendo switch.

#### Expected Hardware:
For the hardware, we decided to use the raspberry pi as it is lightweight, supports Linux natively and can run emulation software
such as box86/64 and Wine, software needed to run the games we would like (Fallout 1 and 2). As well as the raspberry pi, we also
chose the Game Hat interface due to it having built in buttons, joysticks, speakers as well as a screen. This makes it an all in one 
portable console, and, due to the joysticks, makes it perfect for isometric games relative to other types of hardware we could've used. It 
also has pretty good physical integration with the raspberry pi.

#### Extra Features:
We 3D printed a shell as the device was very fragile and exposed without it. The shell would protect the electrical 
components within the console from external elements. 

#### Expected Softwares:
At first, we rejected using RetroPie as it focuses on console games while we plan to run cumputer games, but we ended up comming around to it as
the driver for the Game Hat was made with RetroPie in mind. We used the Game Hat's driver to easily convert our joystick and button inputs into
gameplay inputs. We also downloaded ROMs so there are games that can be played as a console needs to be able to play at least one game.

#### Games of Choice:
For the game we plan to be inside the device, we are choosing Fallout 1, Fallout 2 and Doom as:
- Doom is easy to run on many devices, so it is a good way to know if the device is runnig as intented;
- Fallout 1 & Fallout 2 are both isometric games, making them better for the console relative to a fps game;
- Fallout 1 & Fallout 2 are also classic retro-styled games which would minimize the risk of compatibility issues with a console made for more older games.

#### Various Considerations:
For the future, we plan to use Raspberry Pi OS due to the fact it is optimized for the raspberry pi hardware. It also supports Box86/64 and Wine, which are
softwares needed to run games that aren't as simple as arcaide ones. AntiMicroX might be required to convert the joystick and button inputs of the handheld
console into keyboard inputs for the computer games, as the Game Hat driver might not work with games that aren't suported by RetroPie.
