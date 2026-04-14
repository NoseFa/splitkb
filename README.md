# Nordic split

![3D render](./Media/LeftSideRenderSnowEnv.png)

A split low-profile wireless keyboard with a nordic ISO layout. I used the [Caldera Keyboard by Christian Selig](https://github.com/christianselig/caldera-keyboard) as inspiration and it clearly shows in the design. Still  The keyboard uses a nice!nano like microcontroller based on the NRF52840, ZMK as the firmware and a custom pcb with Choc V1 hotswap sockets.

The project was made as a part of Hack Club's [Fallout](https://fallout.hackclub.com/) event.

## Highlights

* **Hotswapping**
* Open-source
* Wireless
* Nordic layout
* total of 74 keys

## Why it exists?

The project was made because I wanted a split keyboard but needed a nordic layout for my day to day stuff (I need the letters Ä, Ö, Å). So the nordic split was born. I took inspiration from the caldera keyboard. It's low profile so it can be transported easily around and it's also wireless so no need for annoying dual or split cables for connecting to a computer. 

Even though it was designed as nordic layout first. The keyboard could also be used by people with non-nordic layouts and you could use the extra row of keys on the right side as shortcut or macro keys. Of course also the pcb could be edited and these keys removed if you don't want them.

## Build guide

### Ordering parts

First you need to order the PCBs from a PCB manufacturer. (Technically nothing prevents you from hand wiring this keyboard but it would require some redesigning of the case and is outside the scope of my project.) I ordered the PCB with the diodes installed. They are pretty annoying to hand solder because of their small size and are not that much more expensive to get preassembled from manufacturers like [JLCPCB](https://jlcpcb.com/). When buying the microcontroller you should probably not buy a nice!nano and instead just a NRF52840 based dev board. This is the one I bought [ProMicro NRF52840](https://www.aliexpress.com/item/1005007205026373.html?spm=a2g0o.productlist.main.8.5285a54cPOmIpa&aem_p4p_detail=202603200108531573820844269200000457052&algo_pvid=ebbbcca8-17d4-4ca8-b59a-75b1f3198b0b&algo_exp_id=ebbbcca8-17d4-4ca8-b59a-75b1f3198b0b-7&pdp_ext_f=%7B%22order%22%3A%22771%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&pdp_npi=6%40dis%21EUR%214.49%213.16%21%21%2134.88%2124.54%21%40211b813f17739941330401522ee8fd%2112000039797470328%21sea%21FI%210%21ABX%211%210%21n_tag%3A-29910%3Bd%3Ab451bb2c%3Bm03_new_user%3A-29895%3BpisId%3A5000000197850273&curPageLogUid=OxA2oroU7gov&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005007205026373%7C_p_origin_prod%3A&search_p4p_id=202603200108531573820844269200000457052_2) from aliexpress and it's pretty much a drop in replacement for the nice!nano.

 For the other components you can look at [Bill of Materials](./BOM.csv). 

### The case

For the case you can either print it or use a 3D printing service. I have a 3D printer so I printed one myself but manufacturers like [JLC3DP](https://jlc3dp.com/) can print the case for you. Remeber that the size are not just mirrored and have different case files. All 3d files are in the [Fusion Files folder](./FusionFiles/). 

### Build Guide Summary

1. Order PCB and other parts.
2. Order or print the case.
3. Solder parts to the PCBs (Diodes, hotswap-sockets, microcontroller)
4. Install the heated threaded inserts to the spots in the case (4 per side)
5. Install the PCB to the case.
6. Install top plate.
7. Install the choc switches to the sockets and keycaps.
8. Flash software (Check software section)
9. Enjoy!

## PCB

![Left Side PCB](./Media/LeftSidePcbScreenshot.png)
Here is a picture of the left side PCB. You can see the switches, traces and a spot for the microcontroller.


![Right Side PCB](./Media/RightSidePcbScreenshot.png)
Here is a picture of the left side PCB. You can see that it is different from the left side instead of just being a mirrored version like some boards are. 

Unlike some other split keyboards the Nordic Splits halves aren't mirrored but instead the right side has an extra row of keys primarly needed to support the Nordic layout. 

## Zine Page

![Zine Page](./Media/ZinePage.png)

Zine page is also available as a [PDF](./ZinePage/ZinePage.pdf). T
Background picture was taken by my dad when we went up north.

## Demo

A video of the keyboard in use.

SOON

## Acknowledgements

* [HackClub Fallout](https://fallout.hackclub.com/)
* [Caldera Keyboard by Christian Selig](https://github.com/christianselig/caldera-keyboard)

## Tools used

### Design

* KiCad (PCB design)
* Fusion (Case design)
* Excalidraw (Notetaking)

### Assembly 

* Soldering iron