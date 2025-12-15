# CHOICES

November 20th 2025  
Luca Ragosta & Ehsan Hussain

#### Basic Idea:
For the project concept, we decide to build a portable Linux based handheld console using raspberry pi alongside a game HAT interface.
We chose this idea because we (Luca and Ehsan) both found it quite interesting and fun to build a handheld console like the steamdeck or 
the Nintendo switch.

#### Expected Hardware:
For the hardware, we decided to use the raspberry pi as it is lightweight, supports Linux natively and can run emulation software
such as RetroPie, software needed to run the games we would like (Fallout 1 and 2). As well as the raspberry pi, we also
chose the Game Hat interface due to it having built in buttons, joysticks, speakers as well as a screen. This makes it an all in one 
portable console, and, due to the joysticks, makes it perfect for isometric games relative to other types of hardware we could've used. It 
also has pretty good physical integration with the raspberry pi.

#### Extra Features:
We 3D printed a shell as the device was very fragile and exposed without it. The shell would protect the electrical components within the console from external elements. We also got 4 18650 batteries from Canadian Tire, as they are required for the system to be portable and work as a handheld mobile console.

#### Expected Softwares:
At first, we rejected using RetroPie as it focuses on console games while we plan to run cumputer games, but we ended up coming around to it as
the driver for the Game Hat was made with RetroPie in mind. We used the Game Hat's driver to easily convert our joystick and button inputs into
gameplay inputs. We also downloaded ROMs so there are games that can be played as a console needs to be able to play at least one game. We also wanted
to run Fallout 1 and/or Fallout 2 on our system, but decided against it due to difficulty and lack of time.

#### Games of Choice:
For the game we plan to be inside the device, we chose Doom as:
- Doom is easy to run on many devices, so it is a good way to know if the device is runnig as intented;


#### Various Considerations:
For the future, we plan to use Raspberry Pi OS due to the fact it is optimized for the raspberry pi hardware. It also supports RetroPi ontop of it as an emulator. We initially wanted to use Box86/64 and Wine but decided against it and instead chose to use RetroPie and DosBox instead, as they are a lot simpler and straightforward and there is a tutorial on the gamehat website for how to use them. We wanted to use Fallout 1&2 as our games for the presentation however it became all too complicated. Doom, a game released in 1993, was very easy, lightweight and quick to install, making it the final choice for the game we chose.