# grblPANEL

A hardware control panel implementation for [grblHAL](https://github.com/grblHAL).

This is the top level repository for the grblPANEL project, containing links to the various project components.

![panel](https://github.com/dresco/grblPANEL/blob/master/images/panel.jpg)

## Background

This project started with the desire to add physical controls to a grblHAL CNC machine, without extending logic level signals from the controller board outside of the electronics enclosure.

Using **Modbus RTU** for connectivity seemed a logical first choice, as was already supported by grblHAL, and actively in use for VFD control. Subsequently, support for **CAN bus** was added as an option. This is a work in progress, as a new [CAN bus plugin](https://github.com/dresco/Plugin_canbus) and platform drivers are required on the grblHAL side.

This control panel implementation supports physical buttons, encoders, and a display. It allows for issuing commands, jogging, spindle/feed overrides, and for displaying current machine position & status.

## Project components

As well as the plugin, this project also provides the open source firmware, and  hardware designs for a reference implementation of a control panel.

The hardware designs cover the printed circuit boards (front panel, main board, keypad, and encoder breakouts), along with the 3D printed components necessary for assembly (a mounting bezel for the display & control board, and the back box of the enclosure).

Until now, the prototype boards & panels have been hand assembled. However, the various hardware components could be made available in kit form if there is sufficient interest. Open to feedback on this, see discussion [here](https://github.com/grblHAL/core/discussions/82).

## Repositories

Software.
 - [grblPANEL firmware](https://github.com/dresco/grblpanel_firmware) 
 - [Control panel plugin for grblHAL](https://github.com/dresco/Plugin_panel)

Printed circuit boards (KiCad & gerber files).
 - [Front panel](https://github.com/dresco/grblpanel_front_panel)
 - [Main controller board](https://github.com/dresco/grblpanel_main_board)
 - [Keypad](https://github.com/dresco/grblpanel_keypad_6x11)
 - [Encoder breakout](https://github.com/dresco/grblpanel_encoder_breakout)

3D printing designs (CAD models & STL files).
 - [Front panel layout](https://github.com/dresco/grblpanel_front_panel_openscad)
 - [Bezel mount for display & control board](https://github.com/dresco/grblpanel_display_bezel)
 - [Back box](https://github.com/dresco/grblpanel_back_box)
