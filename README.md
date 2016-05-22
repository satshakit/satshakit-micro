<h1 style="font-family: courier;" align="center"> satshakit</h1>
<p align="center">
<img src="media/readme/satshakites.jpg" width="70%">
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

satshakit boards
--

There are different kinds of **satshakit boards** depending on the **fabrication technique** you will use to make them, or on the **size** of the board. 

<img src="media/readme/satshakit_versions.jpg" width="70%">

Here is a comparison table about different satshakit boards:

|name|mcu|pins|size(mm)|
| :---: | :---:|:---:|:---:|
|`satshakit laser`|ATmega328P|Arduino + ADC6/7|48 x 42|
|`satshakit cnc`|ATmega328P| Arduino + ADC6/7  |54 x 45|
|`satshakit multicore`|2 x ATmega328P| 2 x Arduino + ADC6/7|50 x 42|
|`satshakit micro`| ATmega328P|Arduino|40 x 24|


satshakit micro
--

**satshakit micro** is a downsized version of the satshakit laser and cnc, developed to be used in **constrained space applications** like embedding the board in textiles or in small objects, or useful for who wants just a **bare metal board** to start with, also easy to be modified and/or customized. While satshakit micro is less than half the size of the other satshakits, it's a **full featured board** with the full Adruino pinout, missing only the possibility to be programmed using an FTDI cable.

Here is the **satshakit micro board**:

<img src="media/satshakit_micro_board.jpg" width="70%">

<img src="/media/satshakit_micro.png" width="70%">

**downloads (right click, download as)**

- [satshakit micro svg](https://raw.githubusercontent.com/satshas/satshakit/master/media/satshakit_micro/satshakit_micro.svg)
- [satshakit micro internal png](https://raw.githubusercontent.com/satshas/satshakit/master/media/satshakit_micro/satshakit_micro_internal.png)
- [satshakit micro holes png](https://raw.githubusercontent.com/satshas/satshakit/master/media/satshakit_micro/satshakit_micro_holes.png)
- [satshakit micro cut png](https://raw.githubusercontent.com/satshas/satshakit/master/media/satshakit_micro/satshakit_micro_cut.png)
- [satshakit micro cut tips png](https://raw.githubusercontent.com/satshas/satshakit/master/media/satshakit_micro/satshakit_micro_cut_tips.png)
- [satshakit micro schematic](https://raw.githubusercontent.com/satshas/satshakit/master/eagle_projects/satshakit_micro/satshakit_micro.sch)
- [satshakit micro board](https://raw.githubusercontent.com/satshas/satshakit/master/eagle_projects/satshakit_micro/satshakit_micro.brd)
- [satshakit micro BOM Open Document](https://github.com/satshas/satshakit/raw/master/docs/satshakit_micro/satshakit_micro_BOM.ods)
- [satshakit micro BOM Excel](https://github.com/satshas/satshakit/raw/master/docs/satshakit_micro/satshakit_micro_BOM.xlsx)

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

<img src="media/satshakit_micro/satshakit_micro_arduino_programming.png" width="60%">

<img src="media/satshakit_micro/satshakit_micro_fabisp_programming.png" width="60%">

Once everything is connected, follow these steps to upload Arduino bootloader:

1. open Arduino IDE 
2. select proper programmer (for example Arduino as ISP or USBtinyISP) 
3. select Arduino UNO as board
4. click on tools->Burn Bootloader

To program a satshakit micro, you have always to use a programmer, and use the **Sketch >Upload using a programmer** function of the Arduino IDE.

And here is the Arduino pinout of the satshakit micro:

<img src="media/satshakit_micro/satshakit_micro_arduino_pin_mapping.png" width="60%">

What's in the repo
--
- **[docs](https://github.com/satshas/satshakit/tree/master/docs)**: BOM files for Farnell
- **[egle projects](https://github.com/satshas/satshakit/tree/master/eagle_projects)**: eagle projects of satshakit
- **[media](https://github.com/satshas/satshakit/tree/master/media)**: svg of satshakits, connections schemas, images for cnc milling machine and fiber laser cutter, other images

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
This work is licensed under the terms of Attribution-NonCommercial-ShareAlike 4.0 International ([CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/)).

Disclaimer  
--

<div class="align-justify">
This hardware/software is provided "as is", and you use the hardware/software at your own risk. Under no circumstances shall any author be liable for direct, indirect, special, incidental, or consequential damages resulting from the use, misuse, or inability to use this hardware/software, even if the authors have been advised of the possibility of such damages.</div>
