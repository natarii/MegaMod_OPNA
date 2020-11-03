# OPNA MegaMod
This add-on board lets you play OPNA, OPN, and AY-3-8910 VGM files using your MegaGRRL Desktop.

![](<images/unit.jpg>)

**This board is provided as an experimental add-on. Software support is working, but incomplete. Software support may improve in the future.**

**MegaGRRL Desktop Firmware v0.97dev or newer is required!** See [Firmware Releases](https://git.agiri.ninja/natalie/megagrrl/-/releases)

# Usage
1. Power off the MegaGRRL Desktop.
2. Remove the YM2612 and SN76489, and seat the addon board into their sockets.
3. Set all 4 DIP switches on the desktop board to OFF.
4. Power on. The presence of the OPNA board will be detected upon boot. Play an OPNA/OPN/AY-3-8910 VGM file.

# Bill of Materials
| Ref.Dsg. | Value | Note |
| -------- | ----- | ---- |
| C1 | 10uF electrolytic |
| C2 | 2.7nF ceramic |
| C3 | 2.7nF ceramic |
| C4 | 68pF ceramic |
| C5 | 0.1uF ceramic |
| C6 | 0.1uF ceramic |
| C7 | 0.1uF ceramic |
| C8 | 0.1uF ceramic |
| C9 | 0.1uF ceramic |
| R1 | 33 ohm |
| R2 | 470 ohm |
| R3 | 1k ohm |
| RN1 | 10k bussed | Must be 9-pin bussed type |
| IC1 | YM2608 |
| IC2 | HM514260DJ | Tested with HM514260DJ. Other DRAMs may be compatible. Must be SOJ-40 footprint, 5V, 4Mbit (256Kx16), "fast page" type |
| IC3 | 74HC04 |
| IC4 | TL072 or SA5532 | Many opamps will work |
| IC5 | YM3016 |
| D1 | 1N5819 |
| Misc | 40 pins 0.1" machine pin header | 0.1" machine pin male-to-male headers, 40 pins total required. Must be machine pin type!!! |

All parts other than the DRAM at IC2 are THT.

# Assembly
1. Solder on the DRAM. Be careful to not short any pins underneath the IC
2. Solder on the remaining THT components
3. Solder on the pin headers (use MegaGRRL Desktop IC sockets for alignment)

# Gerber files
Gerbers for JLCPCB are in the `gerbers/` directory.
