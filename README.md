# Arduino Core for SAMD21 CPU

This repository contains the source code and configuration files of the Arduino Core
for Atmel's SAMD21J processor (based on the same for the Arduino Zero, modified for Brown Cubesat's board variant).

In addition, the bootloader is modified to support loading program (sketch) code from radiation-safe memory into main program memory over SPI.

## Installation on Arduino IDE

The Brown CubeSat fork requires a few more steps to install. Assuming you are installing as a developer for this project:

1. Clone this repository to a local directory
2. Install the Arduino Core for SAMD21 using the Arduino board manager:
  * This core is available as a package in the Arduino IDE cores manager. Just open the "Boards Manager" and install the package called: "Arduino SAMD Boards (32-bit ARM Cortex-M0+)"
3. Navigate to the install location of the Arduino SAMD 21 core definition. On Mac OS X it finds itself under `~/Library/Arduino15/packages/arduino/hardware/samd/<version>`
4. For purposes of this project, replace the contents of that directory with the contents of this repository. Alternatively, replace the `<version>` directory under `samd/` with a symlink to the contents of this repository elsewhere on the filesystem.

If you'd like to revert back to the upstream Arduino board definition, reinstall the definition from the Arduino IDE Boards Manager.

## Support

There is a dedicated section of the Arduino Forum for general discussion and project assistance for the Arduino Zero:

http://forum.arduino.cc/index.php?board=98.0

This fork does not have official support.

## Bugs or Issues

If you find a bug you can submit an issue here on github:

Before posting a new issue, please check if the same problem has been already reported by someone else
to avoid duplicates.

## Contributions

Contributions are always welcome. The preferred way to receive code cotribution is by submitting a 
Pull Request on github.

## License and credits

This repository is forked from the upstream Arduino core which is developed by Arduino LLC in collaboration with Atmel.

```
  Copyright (c) 2015 Arduino LLC.  All right reserved.

  This library is free software; you can redistribute it and/or
  modify it under the terms of the GNU Lesser General Public
  License as published by the Free Software Foundation; either
  version 2.1 of the License, or (at your option) any later version.

  This library is distributed in the hope that it will be useful,
  but WITHOUT ANY WARRANTY; without even the implied warranty of
  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
  See the GNU Lesser General Public License for more details.

  You should have received a copy of the GNU Lesser General Public
  License along with this library; if not, write to the Free Software
  Foundation, Inc., 51 Franklin St, Fifth Floor, Boston, MA  02110-1301  USA
```
