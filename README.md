<h1 style="font-family: courier;" align="center"> satshakit micro</h1>
<p align="center">
<img src="media/satshakit_micro_2.jpg" width="70%">
<div align="center"><i>An improved & fabbable 100% Arduino IDE/libraries compatible board.</i></div>
</p>  

What is satshakit?
--

satshakit is a **100% Arduino IDE  and libraries compatible**, fabbable and open source board, and also an improved version of [Fabkit](http://fabacademy.org/archives/2015/doc/projects/fabkit-0.4.html). 

Main **improvements and features** are:

- **16Mhz** instead of 8Mhz
- **crystal** instead of resonator
- **costs less** (7-9 euro vs 13 euro)
- 100% compatible with **default Arduino IDE** (satshakit is recognized as Arduino UNO)
- ADC6/7 connected instead of ADC6/7 not connected (satshakit laser and cnc)
- larger space to easy soldering (satshakit laser and cnc)

Here you can find all of the satshakit boards: **[satshakit organization](https://github.com/satshakit)**.

satshakit micro
--

**satshakit micro** is a downsized version of the satshakit laser and cnc, developed to be used in **constrained space applications** like embedding the board in textiles or in small objects, or useful for who wants just a **bare metal board** to start with, also easy to be modified and/or customized. While satshakit micro is less than half the size of the other satshakits, it's a **full featured board** with the full Adruino pinout, missing only the possibility to be programmed using an FTDI cable.

Here is the **satshakit micro board**:

<img src="media/satshakit_micro_board.jpg" width="70%">

<img src="/media/satshakit_micro.png" width="70%">

**downloads (right click, download as)**

- [satshakit micro svg](https://raw.githubusercontent.com/satshakit/satshakit-micro/master/media/satshakit_micro.svg)
- [satshakit micro internal png](https://raw.githubusercontent.com/satshakit/satshakit-micro/master/media/satshakit_micro_internal.png)
- [satshakit micro holes png](https://github.com/satshakit/satshakit-micro/blob/master/media/satshakit_micro_holes.png)
- [satshakit micro cut png](https://github.com/satshakit/satshakit-micro/blob/master/media/satshakit_micro_cut.png)
- [satshakit micro cut tips png](https://github.com/satshakit/satshakit-micro/blob/master/media/satshakit_micro_cut_tips.png)
- [satshakit micro schematic](https://raw.githubusercontent.com/satshakit/satshakit-micro/master/eagle_projects/satshakit_micro/satshakit_micro.sch)
- [satshakit micro board](https://raw.githubusercontent.com/satshakit/satshakit-micro/master/eagle_projects/satshakit_micro/satshakit_micro.brd)
- [satshakit micro BOM Open Document](https://github.com/satshakit/satshakit-micro/raw/master/docs/satshakit_micro_BOM.ods)
- [satshakit micro BOM Excel](https://github.com/satshakit/satshakit-micro/raw/master/docs/satshakit_micro_BOM.xlsx)

**media**

<img src="media/satshakit_micro_1.jpg" width="70%">

<img src="media/satshakit_micro_2.jpg" width="70%">

satshakit micro blink:

<a href="http://www.youtube.com/watch?feature=player_embedded&v=3qz0hKS8dOc
" target="_blank"><img src="http://img.youtube.com/vi/3qz0hKS8dOc/0.jpg" 
alt="http://img.youtube.com/vi/3qz0hKS8dOc/0.jpg" width="240" height="180" border="10" /></a>

Getting Started
--
A satshakit board is **totally like an Arduino board**, thus is possible to use the Arduino IDE without any modification. When you finish solder satshakit, you're ready to program it. If you want to use satshakit as an Arduino, you first need to **upload Arduino bootloader**. This will also set the ATmega328P fuses as the same of an Arduino UNO.
To do this you need to use a **programmer**, for example another Arduino or FabISP. If you plan to program a satshakit with an Arduino, be sure to upload the **Arduino as ISP skecth** before connecting the satshakit to it.

Here are the connection schemas for programming **satshakit micro**:

<img src="media/satshakit_micro_arduino_programming.png" width="60%">

<img src="media/satshakit_micro_fabisp_programming.png" width="60%">

Once everything is connected, follow these steps to upload Arduino bootloader:

1. open Arduino IDE 
2. select proper programmer (for example Arduino as ISP or USBtinyISP) 
3. select Arduino UNO as board
4. click on tools->Burn Bootloader

To program a satshakit micro, you have always to use a programmer, and use the **Sketch >Upload using a programmer** function of the Arduino IDE.

And here is the Arduino pinout of the satshakit micro:

<img src="media/satshakit_micro_arduino_pin_mapping.png" width="60%">

What's in the repo
--
- **[docs](https://github.com/satshakit/satshakit-micro/tree/master/docs)**: BOM files for Farnell
- **[egle projects](https://github.com/satshakit/satshakit-micro/tree/master/eagle_projects/satshakit_micro)**: eagle projects of satshakit
- **[media](https://github.com/satshakit/satshakit-micro/tree/master/media)**: svg of satshakits, connections schemas, images for cnc milling machine and fiber laser cutter, other images

Authors
--

- Daniele Ingrassia

Contact
--
- **ingrassiada@gmail.com**
- **[linkedin](http://it.linkedin.com/in/danieleingrassia)**


Thanks
--

[Fablab Kamp-Lintfort](http://fablab.hochschule-rhein-waal.de/index.php/de/)<br />
Hochschule Rhein-Waal<br />
Friedrich-Heinrich-Allee 25, 47475 Kamp-Lintfort, Germany<br />
fablab@hochschule-rhein-waal.de


License
--
This work is licensed under the terms of the open source license: Creative Commons Attribution-ShareAlike 4.0 International ([CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/)).

Disclaimer  
--

<div class="align-justify">
This hardware/software is provided "as is", and you use the hardware/software at your own risk. Under no circumstances shall any author be liable for direct, indirect, special, incidental, or consequential damages resulting from the use, misuse, or inability to use this hardware/software, even if the authors have been advised of the possibility of such damages.</div>
