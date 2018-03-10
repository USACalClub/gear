# DMMs

Information about digital multimeters, especially used models of interest to volt-nuts.

## Models with 6.5-digit resolution

### General info:

| Make | Model | Introduced | Comms | Image |
|---|---|---|---|---|
| HP | 3456A | 1980? | GPIB | ![](media/hp-3456a.jpg) |
| HP | 3457A | 1985? | GPIB | ![](media/hp-3457a.jpg) |
| HP / Agilent / Keysight | 34401A | 1991? | GPIB, RS-232 | ![](media/hp-34401a.jpg) |
| Keithley | 192 | 1982? | ? | ![](media/keithley-192.jpg) |
| Keithley | 193 | 1985? | GPIB | ![](media/keithley-193.jpg) |
| Keithley | 196 | 1986? | GPIB | ![](media/keithley-196.jpg) |
| Keithley | 199 | 1986? | GPIB | ![](media/keithley-199.jpg) |
| Keithley | 2000 | | GPIB, RS-232 | ![](media/keithley-2000.jpg) |
| Keithley | 2015 | | GPIB, RS-232 | ![](media/keithley-2015.jpg) |
| ~~Keithley~~ | ~~2100~~ | | | ![](media/keithley-2100.jpg) |
| Fluke | 8502A | | GPIB (opt.) | ![](media/fluke-8502a.jpg) |
| Fluke | 8505A | | GPIB (opt.) | ![](media/fluke-8505a.jpg) |
| Fluke | 8520A | | GPIB | ![](media/fluke-8520a.jpg) |
| Datron | 1062 | | GPIB | ![](media/datron-1062.jpg) |
| Prema | 6001 | | | ![](media/prema-6001.jpg) |

Notes:
- "The rebadged Keithley 2100 was quite terrible" [[1](https://www.eevblog.com/forum/chat/bench-multimeter-(another)/msg244830/#msg244830)]

### Range info:

| Make | Model | Range scheme | Max value |
|---|---|---|---|
| HP | 3456A | 1x, 10x... | 1.1999x |
| HP | 3457A | 3x, 30x... | 3.0300x |
| HP/Agilent | 34401A | 1x, 10x... | |
| Keithley | 192 | 2x, 20x... | |
| Keithley | 193 | 2x, 20x... | |
| Keithley | 193 | 2x, 20x... | |
| Keithley | 196 | 3x, 30x... | |
| Keithley | 199 | 3x, 30x... | |
| Keithley | 2000 | | |
| Keithley | 2015 | | |
| Fluke | 8502A | | |
| Fluke | 8505A | | |
| Fluke | 8520A | | |
| Datron | 1062 | | |
| Prema | 6001 | | |

### DC Volts info:

| Make | Model | Best res. (range) | Hi-Z (value) |
|---|---|---|---|
| HP | 3456A | 100nV (100mV) | 100mV, 1V, 10V |
| HP | 3457A | 10nV (30mV) | 30mV, 300mV, 3V |
| HP/Agilent | 34401A | | |
| Keithley | 192 | 1uV (2V<sup>*</sup>) | 200mV, 2V, 20V (>1G) |
| Keithley | 193 | 100nV (200mV) | 200mV, 2V |
| Keithley | 196 | 100nV (300mV) | 300mV, 3V |
| Keithley | 199 |  |  |
| Keithley | 2000 | | |
| Keithley | 2015 | | |
| Fluke | 8502A | | |
| Fluke | 8505A | | |
| Fluke | 8520A | | |
| Datron | 1062 | | |
| Prema | 6001 | | |

Note:
- Keithley 192 has no 0.2V range in 6.5-digit mode (best 6.5-digit resolution is 1uV in 2V range).

### Calibration info:

| Make | Model | Cal methods |
|---|---|---|
| HP | 3456A | Trimpots |
| HP | 3457A | Front-panel, GPIB |
| HP/Agilent | 34401A | Front-panel, GPIB |
| Keithley | 192 | Trimpots |
| Keithley | 193 | |
| Keithley | 196 | |
| Keithley | 199 | |
| Keithley | 2000 | |
| Keithley | 2015 | |
| Fluke | 8502A | |
| Fluke | 8505A | |
| Fluke | 8520A | |
| Datron | 1062 | |
| Prema | 6001 | |

Notes:
- The 34401A's calibration counts each range as a "calibration", so a full calibration will increase the count by 35.

Ohms calibration info:

| Make | Model | Valid cal. input range |
|---|---|---|
| HP | 3456A | (arbitrary) |
| HP | 3457A | (See note<sup>*</sup>) |
| HP/Agilent | 34401A | 0.9x to 1.1x |
| Keithley | 192 | (must less than full-scale) |
| Keithley | 193 | |
| Keithley | 196 | |
| Keithley | 199 | |
| Keithley | 2000 | |
| Keithley | 2015 | |
| Fluke | 8502A | |
| Fluke | 8505A | |
| Fluke | 8520A | |
| Datron | 1062 | |
| Prema | 6001 | |

Notes:
- The 3457A allows entering the exact value of the calibration source, but I'm not sure of the allowed range of values.  The service manual lists the following "required equipment" for calibration:
  - 30R (+/-0.2%), 300R (+/-0.02%), 3K (+/-0.003%), 30K (+/-0.001%), 300K (+/-0.001%), 3Meg (+/-0.002%), 30Meg (+/-0.009%)
- The Keithley 192 calls for 1.9x calibration values.  The manual also specifies "To prevent AD saturation, peak AC+DC value must be less than full scale on any range".

### Additional resources:

- HP 3456A
  - [xDevs](https://xdevs.com/fix/hp3456a/)
- Keithley 199
  - [Re-engineered digital board](https://www.eevblog.com/forum/repair/keithley-199-digital-board-replacement/)
  - [Replacing 1N4579 ref. zener with LM399](https://www.eevblog.com/forum/chat/bench-multimeter-(another)/msg265846/#msg265846)

### Template:

| Make | Model | A | B |
|---|---|---|---|
| HP | 3456A | | |
| HP | 3457A | | |
| HP/Agilent | 34401A | | |
| Keithley | 192 | | |
| Keithley | 193 | | |
| Keithley | 196 | | |
| Keithley | 199 | | |
| Keithley | 2000 | | |
| Keithley | 2015 | | |
| Fluke | 8502A | | |
| Fluke | 8505A | | |
| Fluke | 8520A | | |
| Datron | 1062 | | |
| Prema | 6001 | | |


## Models with 5.5-digit resolution

### General info:

| Make | Model | Introduced | Comms | Image |
|---|---|---|---|---|
| Keithley | 195A | 1984? | GPIB | ![](media/keithley-195a.jpg) |
| Keithley | 199<sup>*</sup> | 1988? | GPIB | ![](media/keithley-199.jpg) |

Notes:
- The Keithley 199 is a scanner.
