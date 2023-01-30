# USB Arcade two player controller with spinner
## Introduction
Firmware for the Arcade two player controller with spinner built by [Antonio Villena](https://www.antoniovillena.es/).

As it is based on MickGyver's work, the input lag for this adapter is also minimal.

## Building the projects
You will need the [Arduino IDE](https://www.arduino.cc/en/Main/Software) to build the project. Download the repository via the "Clone or download" button, open the project (.ino extension) in the IDE and select "Arduino Leonardo" in Tools / Board. Connect the Arduino to a USB port and build/upload from Scetch / Upload.

You have to install the great [YetAnotherArduinoPcIntLibrary](https://github.com/paulo-raca/YetAnotherArduinoPcIntLibrary) for the management of PCINT.

You can enable the use of the spinner as a PC mouse (diagonal) by uncommenting the #DEFINE MOUSE line.

## Usage
First time you use the adapter (and first time you change your setup, i.e. you add, or remove, the spinner in your machine, to be able to use buttons B5 and B6 on Player 2 -they collide with endoder inputs-) you must tell the adapter so.

To indicate that:

* You want to use the Spinner: press Player 1 UP while resetting (connecting USB or powering ON) your adapter.
* You want to use B5 and B6 on Player 2: press Player 1 DOWN while resetting (connecting USB or powering ON) your adapter. Keep in mind that if you leave the enconder connected, you may register B5 and/or B6 phantom pushes.

You only have to do this ONCE, as the value is persistent (stored in EEPROM). Of course, if you change your setup (with/out spinner), you have to do it again.

## License
This project is licensed under the GNU General Public License v3.0.

## Credits
The great work by MickGyver and his [DaemonBite-Arcade-Encoder](https://github.com/MickGyver/DaemonBite-Arcade-Encoder), from where I took the code for the base and two player arcade adapter.

Also, the great work by Niels3RT and his [SpinJoy - Spinner and Joystick combo](https://github.com/Niels3RT/SpinJoy), from where I took the code for the spinner.

And last but not least, thanks to [Antonio Villena](https://www.antoniovillena.es/) for the ideas and prompts.

