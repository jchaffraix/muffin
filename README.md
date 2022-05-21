# muffin

A small mechanical keyboard for learning (and fun).

The goal is to build a small factor to learn how to build the PCB, soldering small components
and writing the firmware.

## Features

* USB-C connector.
* 5 keys, using Cherry MX or Kailh choc switches, including a 2U with a stabilizer.
* 1 rotary encoder.
* ATmega16 based.
* Mostly 805 SMT components.
* Include a programmer connector for ease of prototyping.
* A Muffin logo (because why not!?).

## PCB

The project relies on the [Keebio parts](https://github.com/keebio/Keebio-Parts.pretty) repository for the encoder and switch footprints.

To fetch the dependencies, run:

```
git submodule fetch
```

## Bill Of Materials

| Item | Package | Qty | Reference |
|------|---------|-----|-----------|
| 10uF Capacitor | SMT 805 | 1 | |
| 1uF Capacitor | SMT 805 | 1 | |
| .1uF Capacitor | SMT 805 | 4 | |
| 22pF Capacitor | SMT 805 | 2 | |
| Diode | SMT 805 | 5 | Rated 5V |
| 5.5V Zener Diode | SMT 805 | 1 |  |
| LED Red | SMT 805 | 1 | |
| LED Blue | SMT 805 | 1 | |
| LED Green | SMT 805 | 1 | |
| 10k resistor | SMT 805 | 1 | |
| 5.1k resistor | SMT 805 | 2 | |
| 330 resistor | SMT 805 | 4 | |
| 22 resistor | SMT 805 | 2 | |
| USB ESD protection | SOT-143 | 1 |  Used D1213A-02SR-7|
| USB C receptable (female) | | 1 | Used HRO-TYPE-C-31-M-12 |
| AVR-ISP-6 connector | | 1 | |
| RotaryEncoder Switch | | 1 | Used Alps EC11 |
| Cherry or Kailh choc Switches | | 5 | |
| Switch stabilizer for 2U | | 1 | |
| ATmega16U4-M | QFN-44 | 1 | ATmega32U4 should work too|
| 16MHz crystal | | 1 | Used 3155-16M20P2/49US-ND |
| Reset switch | | 1 | Used MJTP1117 |
| Optional programming Switch | SMT 254 | 1 | Used 2223-DS04-254-2-01BK-SMT-ND |

Note: The crystal and the 2pF capacitors can be omitted if you use the internal clock (which requires programming some bits on the ATmega16).

## Compiling and flashing

Coming soon.
