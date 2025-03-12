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

| Qty. | Part | Part No. | Description | Link |
| --- | --- | --- | --- | --- |
| 1	| RF Rotary Joint	|	BN 835047C0010 | SMA-f (50 Ω), DC-18 GHz | [link](https://products.spinner-group.com/1-channel-coaxial-rotary-joint-sma-female-dc-18-ghz-bn835047C0011) |
| 1 | NEMA 11 motor | 11HS18-0674S | 45mm length, 1.8 deg step angle, ~600mA max | [link](https://www.omc-stepperonline.com/nema-11-bipolar-1-8deg-9-5ncm-13-5oz-in-0-67a-4-6v-28x28x45mm-4-wires-11hs18-0674s) |
| 1 | 3D printed case | Custom part | 3D printed | [link](https://github.com/open-ephys/commutator-coax/tree/main/mechanical/production) |
| 1 | 3D printed motor gear | Custom part | 3D printed | [link](https://github.com/open-ephys/commutator-coax/tree/main/mechanical/production) | 
| 1 | 3D printed commutator gear | Custom part | 3D printed | [link](https://github.com/open-ephys/commutator-coax/tree/main/mechanical/production) | 
| 7 | M2.5 x 8mm socket head cap screws | 91290A102 | for attaching rotary joint to case | [link](https://www.mcmaster.com/91290a102) |
| 4 | M2.5 x 8mm button head screws | 91239A756 | for attaching the PCB to the case | [link](https://www.mcmaster.com/91239A756) |