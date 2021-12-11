# joykey

joykey is a simple program that converts button and axis inputs of joystick devices to keyboard inputs on Linux.

## Installation

```bash
(sudo) pip3 install -r requirements.txt
```

## Usage

```
joykey [options]

Options:
    -h, --help
        Show this help message
    -v, --print-state
        Print the state of the joystick when conntected
```

The `joykey.yaml` configuration file can be placed in the current directory, beside the executable, in `~/.config` and in `/etc`.

The root entries of the configuration file are the names of the joystick devices you want to configure.

Each device has action definitions for buttons and axes. 

# References

Based on gist by rdb realeased under the Unlicense (unlicense.org):
https://gist.github.com/rdb/8864666

Based on information from:
https://www.kernel.org/doc/Documentation/input/joystick-api.txt

Keyboard input is generated using pynput which is released under the LGPL license
https://github.com/moses-palmer/pynput


# Licensing

```
This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.
```
