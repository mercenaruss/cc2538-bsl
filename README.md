TI CC13xx/CC2538/CC26xx Serial Boot Loader
==========================================

This folder contains a python script that communicates over LAN with the boot loader of the Texas Instruments CC2538, CC26xx and CC13xx SoCs (System on Chips).<br>
It can be used to erase, program, verify and read the flash of ZigStar LAN,USB Coordinators.

### Requirements

To run this script you need a Python interpreter, Linux and Mac users should be fine, Windows users have a look here: [Python Download][python].

### Dependencies

pip install pyserial intelhex python-magic

### Usage

This modified version of CC2538-BSL by Jelmer_T is intended to be used with ZigStar Gateways,Sticks based on CC2652 chips from TI<br>
python cc2538-bsl.py -p socket://ip_or_mdns.local:6638 - evwZ firmware.hex<br>
where:<br>
-Z or --zigstar is for LAN Coordinator

You can find more info on the different options by executing `python cc2538-bsl.py -h`.

##### Authors
Jelmer Tiete (c) 2014, <jelmer@tiete.be>   
Loosly based on [stm32loader] by Ivan A-R <ivan@tuxotronic.org>
  
