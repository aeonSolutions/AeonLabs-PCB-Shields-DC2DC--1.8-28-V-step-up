# AeonLabs PCB Shields DC DC 1.8-28V Step up
This is a pcb design for a DC DC [1.8;28]V step-up converter intended for small, low power, applications/ devices.. Suitable as a add-on design for any other KiCad project. The MT3608 is a constant frequency, 6-pin SOT23 with hight efficiency up to 97%. To change the output voltage one needs to change the resistance in the voltage divider connected to pin 3 of the MT3608 IC.

*Don't forget to LIKE , SHARE and subscribe the free whatsApp group* and if you liked this PCB consider buying me a cup of coffee. Links below.

![](https://views.whatilearened.today/views/github/aeonSolutions/AeonLabs-PCB-Shields-DC2DC--1.8-28-V-step-up.svg)
![](https://img.shields.io/github/downloads/aeonSolutions/AeonLabs-PCB-Shields-DC2DC--1.8-28-V-step-up/total)

### Status
![](https://github.com/aeonSolutions/AeonLabs-PCB-Shields-DC2DC--1.8-28-V-step-up-down/blob/main/designs/working_green.png)  fully tested & working.

If you already tested this PCB send me a message. Thank you


## Revisions
- revision 1.0
 
## Download options
Download this repository if you need the KiCad Files or, download the Gerber files in the release section of this repository

## Liked it ? Get a Free PCB for yourself
Send me your Device or hardware and i will design a custom PCB for it. Free of charge. Contact-me on WhatsApp or email for more info. 

## Q&A WhatsApp Group
If you have any Questions or simply  like this kind of projects and want to stay updated with the latest research ideas and prototypes during the day and week, join the WhatsApp Group
[A.I. Things](https://chat.whatsapp.com/FkNC7u83kuy2QRA5sqjBVg)

## Fully assembled PCB
Alternatively, and if you do not want to build a PCB by yourself and like to buy one, you can do it here:

[![](https://github.com/aeonSolutions/PCB-Prototyping-Catalogue/blob/main/tindie_sell.png)](https://www.tindie.com/stores/aeonlabs/)

The price will be around 30eur plus postage fees.
(I will also deliver the assembled PCB with all the components in place at a fair aditonal cost).

#### Be supportive of my dedication and work towards technology education and buy me a coffee. Link below.

![](https://github.com/aeonSolutions/AeonLabs-PCB-Shields-DC2DC--1.8-28-V-step-up/blob/main/designs/pcb_front.png)

________________________________________________________________________________________________________________

## PCB Parts list
- [Capacitor 2.2uF SMD](https://s.click.aliexpress.com/e/_AVdmzr)
- [Resistor SMD 1206 ](https://s.click.aliexpress.com/e/_A7OXrR)
- [SS34 rectifier Diode](https://s.click.aliexpress.com/e/_DkhOib9)
- [MT3608 DC DC 5W 2A](https://s.click.aliexpress.com/e/_Dmd5xxh)
- [SMD inductor]( https://s.click.aliexpress.com/e/_Dlx2YWx)


## Firmware Download 
one can use the PCB in the repository [AeonLabs-MCU-Burner-USB-to-UART-TTL](https://github.com/aeonSolutions/AeonLabs-MCU-Burner-USB-to-UART-TTL) to program the ESP32 WROOM32 MCU on this PCB.


## REWORKING MT3608 BOOST CONVERTERS FOR LOWER IDLE CURRENT DRAW
by [Lewin Day](https://hackaday.com/author/lewinday/) and by [Aka Kasyan](https://www.youtube.com/c/KasyanTV)

One drawback of the MT3608 IC, particularly when working with batteries, is the idle current draw, on the order of 1 to 1.5mA. Fear not, however — there is a workaround, courtesy of [Aka Kasyan]. (Video, embedded below.)

The trick is to modify the behavior of the converter when no load is connected. The enable pin of the boost converter is held low through a pull-down resistor, keeping the boost converter switched off. In this state, the output voltage is equal to the input voltage. A current sense resistor is then installed in the output path. When a load is connected, this causes a voltage drop across the current sense resistor. This is then used to switch a transistor, which then connects the enable pin to the positive rail, switching the converter on, leading to the full boosted output voltage being reached.

Aka Kasyan reports that this drastically cuts the idle current draw, which is particularly useful for battery powered projects. It’s important to note that the current sense resistor must be appropriately sized for the given load, however. 

[![](https://github.com/aeonSolutions/AeonLabs-PCB-Shields-DC2DC--1.8-28-V-step-up/blob/main/designs/youtube_mt3608.png)](https://www.youtube.com/watch?v=zJJcdptSH80)
______________________________________________________________________________________________________________________________

### License
2022 Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International

https://creativecommons.org/licenses/by-nc-sa/4.0/

### Own a copy of this work
if you like to own a copy of this work, you can buy it as a NFT or Ethereum. contact me for more details at mtpsilva@gmail.com
________________________________________________________________________________________________________________
## [Go back to main catalogue page](https://github.com/aeonSolutions/PCB-Prototyping-Catalogue)
________________________________________________________________________________________________________________

### Share this PCB board files
[![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?original_referer=https%3A%2F%2Fjitpack.io%2F&ref_src=twsrc%5Etfw&text=Version%201.0%20of%20![](https://github.com/aeonSolutions/AeonLabs-PCB-Shields-DC2DC--1.8-28-V-step-up/blob/main/designs/pcb_back.png)%20is%20now%20available%20on%20&tw_p=tweetbutton&url=http%3A%2F%2Fgithub.com%2FaeonSolutions%2F![](https://github.com/aeonSolutions/AeonLabs-PCB-Shields-DC2DC--1.8-28-V-step-up/blob/main/designs/pcb_back.png))

<a href="https://stackexchange.com/users/18907312/miguel-silva"><img src="https://stackexchange.com/users/flair/18907312.png" width="208" height="58" alt="profile for Miguel Silva on Stack Exchange, a network of free, community-driven Q&amp;A sites" title="profile for Miguel Silva on Stack Exchange, a network of free, community-driven Q&amp;A sites" /></a>

### Be supportive of my dedication and work towards technology education and buy me a coffee

[<img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" data-canonical-src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" height="70" />](https://www.buymeacoffee.com/migueltomas)


