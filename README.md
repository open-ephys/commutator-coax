# Torque-free Coax Commutator

The wide-spread availability of 6 degree of freedom pose tracking using internal-measurement units
(IMUs) allows continuous monitoring of an animal's rotational state in an environment. This obviates
the need for tether torque measurements to drive an active commutator since the rotational state of
the animal is known in real-time, and the commutator can simply follow along. This permits the use
of extremely thin [coaxial tethers](https://open-ephys.org/tethers) that cannot function with a
standard active commutator because they are too flexible to translate rotational torque.

![Zero-torque coaxial commutator.](./resources/demo.gif)

This commutator functions with serialized headstages and miniscopes such as 
[ONIX headstages](https://open-ephys.github.io/onix-docs/index.html), and UCLA Miniscope 4.0, that
provide orientation data. It can also be used with a coaxial headstage/miniscope without an IMU,
e.g. using video-based rotation tracking since its remote control interface is agnostic to how
rotational measurements are taken. 

For more information, visit the [commutator docs](https://open-ephys.github.io/commutator-docs/).

## Features

- Supports one high bandwidth RF links up to 18 GHz
- Optical table & 80/20 rail mountable
- Remote control using JSON-encoded commands
- Manual control using capacitive sense buttons
- Indication LED
    - Can be completely turned off
- Advanced stepper driver (TMC2130)
    - Voltage-controlled for silent operation
    - Precise motion using step interpolation (256 uSteps/step)
- USB powered and controlled
    - Internal super-capacitor circuitry prevents loading the USB bus during
      motion

## Hardware License

This work is licensed to Jonathan P. Newman and Jakob Voigts under CC BY-NC-SA
4.0. To view a copy of this license, visit
https://creativecommons.org/licenses/by-nc-sa/4.0

The creation of commercial products using the hardware documentation in this
repository is not permitted without an explicit, supplementary agreement
between the Licensor and the Licensee. Please get in touch if you are
interested in commercially distributing this tool.

## Software/Firmware License

Copyright Jonathan P. Newman

Permission is hereby granted, free of charge, to any person obtaining a copy of
this software and associated documentation files (the "Software"), to deal in
the Software without restriction, including without limitation the rights to
use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
of the Software, and to permit persons to whom the Software is furnished to do
so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.