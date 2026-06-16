# Nordic split

![3D render](./Media/3Drender.png)

A split low-profile wireless keyboard with a nordic ISO layout. I used the [Caldera Keyboard by Christian Selig](https://github.com/christianselig/caldera-keyboard) as inspiration and it clearly shows in the design. Still the keyboard uses a nice!nano like microcontroller based on the same NRF52840, ZMK as the firmware and a custom pcb with Choc V1 hotswap sockets. The keyboard also has an ortholinear layout which can be more ergonomic for some users.

The project was made and designed as a part of Hack Club's [Fallout](https://fallout.hackclub.com/) event where people make hardware projects and get a chance to go to Shenzhen, China. This was also one of my first electronics projects.

## Highlights

* **Hotswapping**
* Open-source
* ZMK firmware (ZMK studio support)
* Wireless
* Nordic layout
* total of 74 keys

## Why it exists?

The project was made because I wanted a split keyboard but needed a nordic layout for my day to day stuff (I need the letters Ä, Ö, Å). So the nordic split was born. I took inspiration from the Caldera keyboard by Christian Selig. It's low profile so it can be transported easily around and it's also wireless so no need for annoying dual or split cables for connecting to a computer or laptop.

This is the first keyboard I have designed so the keymap and layout were made with some educated guess work. They might be updated later down the line. I will update this repo with the most recent keymap I use. Even though it was designed as nordic layout first. The keyboard could also be used by people with non-nordic layouts and you could use the extra row of keys on the right side as shortcut or macro keys. Of course also the pcb could be edited and these keys removed if you don't want them. This keyboard has ZMK studio support so you can change the keymap in the [ZMK.studio web app](https://zmk.studio).

## Build Guide Summary

1. Order PCB and other parts.
2. Order or print the case.
3. Solder parts to the PCBs (Diodes, hotswap-sockets, microcontroller)
4. Install the heated threaded inserts to the spots in the case (4 per side)
5. Install the PCB to the case.
6. Install top plate.
7. Install the choc switches to the sockets and keycaps.
8. Flash software (Check software section)
9. Enjoy!

More detailed build guide is available in the [build guide.md file](buildGuide.md). 

## Software

See [Software.md](./Software/software.md) for more info about software and software installation instructions.

## PCB

![PCB](./Media/PcbScreenshot.png)

Here is a picture of the left side PCB. You can see the switches, traces and a spot for the microcontrollers. The PCBs are seperated by mouse bites in the middle. Unlike some other split keyboards the Nordic Splits halves aren't mirrored but instead the right side has an extra row of keys primarly needed to support the Nordic layout.

The pcb was designed in KiCad by me. You can view the files in the [Kicad folder](./KICAD/splitkb). 

Here is also the schematic which is split into three different pages. One for each side and one main page that has the mousebites and links the pages together. 

![Main Schematic](./Media/MainSchematic.png)

![Right side Schematic](./Media/RightSchematic.png)

![Left side Schematic](./Media/LeftSchematic.png)

## Zine Page

![Zine Page](./Media/ZinePage.png)

Zine page is also available as a [PDF](./ZinePage/ZinePage.pdf).
Background picture was taken by my dad when we went up north.

## Demo

A video of the keyboard in use.

SOON (When I get the parts).

## Acknowledgements

* Thanks to [Hack Club](https://hackclub.com/) [Fallout](https://fallout.hackclub.com/). If you want to view the project I made for Fallout including journals you can view it on [the event page](https://fallout.hackclub.com/projects/156).

* [Caldera Keyboard by Christian Selig](https://github.com/christianselig/caldera-keyboard) was used as inspiration and [his video](https://www.youtube.com/watch?v=7UXsD7nSfDY) was a great watch. My design is clearly inspired by him.

## Tools used

### Design

* KiCad (PCB design)
* Fusion (Case design)
* Excalidraw (Notetaking)
* ZMK CLI

### Assembly

* Soldering iron
* Screwdriver for the M2 screws
* Computer to flash the software.
* USB-C cable
