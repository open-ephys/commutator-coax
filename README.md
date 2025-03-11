# Torque-free Coax Commutator

The wide-spread availability of 6 degree of freedom pose tracking using internal-measurement units
(IMUs) allows continuous monitoring of an animal's rotational state in an environment. This obviates
the need for tether torque measurements to drive an active commutator since the rotational state of
the animal is known in real-time, and the commutator can simply follow along. This permits the use
of extremely thin [coaxial tethers](https://open-ephys.org/tethers) that cannot function with a
standard active commutator because they are too flexible to translate rotational torque.

![Zero-torque coaxial commutator.](./resources/demo.gif)

This commutator functions with serialized headstages and miniscopes (such as [ONIX
headstages](https://open-ephys.github.io/onix-docs/index.html) and UCLA Miniscope 4.0) that provide
orientation data. It can also be used with a coaxial headstage/miniscope without an IMU, using
video-based rotation tracking since its JSON-based command protocol over serial is agnostic to how
rotational measurements are taken. 

For more information, visit the [commutator docs](https://open-ephys.github.io/commutator-docs/).

## BOM

The BOM is 
[here](https://docs.google.com/spreadsheets/d/1M2R0Q2-OuRHzctt05BxtA3hxNcCHtRZHORzCKElmG1Q/edit?usp=sharing).