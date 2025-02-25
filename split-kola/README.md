# Split-Kola

A 5x7 (30-keys) split keyboard that uses a TRRS cable for the interconnect.

* Keyboard Maintainer: [PonderSlime](https://github.com/ponderslime)

## Features
* Hotswap Keys
* RGB Backlit Keys 

## Flashing
Try running this command to flash for each half. If it doesn't work, then I probably need to change it to be different...
```
 qmk compile -kb split_kola -km default -bl uf2-split-left
```
after that, plug in the other half.
```
qmk compile -kb split_kola -km default -bl uf2-split-left
```

That being said, I don't know if this does anything. If that is the case, uncomment this line in config.h:
```
#define MASTER_LEFT
```

and comment
```
#define EE_HANDS
```

But yeah! It should work hopefully!



## Bill of Materials:
- 61 Cherry MX Switches
- 61 Kailh MX Hotswap Sockets
- 61 1N4148W Diodes (SOD-123 footprint)
- 2 PJ-320A TRRS Jacks
- 2 Raspberry Pi Pico footprint boards
- 63 SK6812Mini-E RGB LEDs
- 10 M3 Heatset Inserts
- 10 M3 Screws, 5-7mm length
- 1 PCB for each side (Two unique total)
- All 3D printed case parts

## Challenges
I decided i wanted to make a split keyboard for this, because I have a Bambulab A1 mini at home, and wanted the capability to be able to reprint the case if needed. Also, I decided that I needed both hotswap and RGB keys on it!

When designing the case, I was able to learn how to use onshape a little bit better!

The most frustrating part of the entire project was when I experimented with freerouting in KiCAD. I was forced to reroute everything from scratch!

### Images
![render](https://github.com/user-attachments/assets/342d228d-ea72-49b9-baa3-6384c8f3f0f0)

![https://raw.githubusercontent.com/PonderSlime/Keyboards/refs/heads/main/split-kola/assets/schematic_01.png](https://raw.githubusercontent.com/PonderSlime/Keyboards/refs/heads/main/split-kola/assets/schematic_01.png)


![https://raw.githubusercontent.com/PonderSlime/Keyboards/refs/heads/main/split-kola/assets/pcb_01.png](https://raw.githubusercontent.com/PonderSlime/Keyboards/refs/heads/main/split-kola/assets/pcb_01.png)

![https://raw.githubusercontent.com/PonderSlime/Keyboards/refs/heads/main/split-kola/assets/case_01.png](https://raw.githubusercontent.com/PonderSlime/Keyboards/refs/heads/main/split-kola/assets/case_01.png)
