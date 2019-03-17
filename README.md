# Amiga4Kickstart

En este proyecto se trata de añadir al Amiga 1000 un reubicador de la cpu junto a una EPROM 27c160(2MB) para incluir hasta
4 kickstart diferentes añadiendo para ello una placa externa con un conmutador giratorio a traves del cual se puede seleccionar
la kickstart a cargar.
Se incluyen los esquematicos de las 3 placas necesarias junto a los gerbers.
El programador está diseñado para usarse con un programador TL866II plus.
La lista de componentes es la siguiente:


Programador

2 Zocalos de 42 pines

2 tiras de 3 pines 2.54mm de paso

2 jumpers

2 resistencias de 10K 0402 SMD


Reubicador

2 Zocalos de 64 pines

1 Zocalo de 42 pines

1 pin angulo recto 90º

2 tiras de 64 pines 2.54mm macho

1 conector de 4 pines 2.54mm de paso

1 EPROM 27c160


Conmutador

1 Conmutador giratorio de 3 polos x 4 giros

2 resistencias de 10K 1206 SMD

1 conector de 4 pines 2.54mm de paso


La configuración de puentes para programar la EPROM es la siguiente (a modo de ejemplo):

A18 = 0 : A19 = 0 ------ KICKSTART (1.3)

A18 = 1 : A19 = 0 ------ KICKSTART (2.05)

A18 = 0 : A19 = 1 ------ KICKSTART (3.1)

A18 = 1 : A19 = 1 ------ ROMDIAG u otra





This project is intended to add an Amiga 1000 a CPU relocator with an EPROM 27c160(2M) to include up to 4 different kickstart
adding an external board with a rotary switch that selects the appropiate kickstart to load.
Schematics and gerbers for all boards are included.
The programmer board is designed to use with the TL866II plus programmer.
The BOM is the following:

Programmer

2 42 pines IC Socket

2 2.54mm pitch 3 pin strip male

2 jumpers

2 0402 10K SMD resistor


Relocator

2 64 pin IC Socket

1 42 pin IC Socket

1 2.54mm 1 pin 90º angle

2 64 pin 2.54mm pitch strip male

1 4 pin 2.54mm pitch connector

1 EPROM 27c160


Conmutador

1 Rotary switch 3P4T

2 10K SMD Resistor 1206

1 4 pin 2.54mm pitch connector


The jumper configuration for the programmer board is the following (as an example):

A18 = 0 : A19 = 0 ------ 1ST KICKSTART (1.3)

A18 = 1 : A19 = 0 ------ 2ND KICKSTART (2.05)

A18 = 0 : A19 = 1 ------ 3RD KICKSTART (3.1)

A18 = 1 : A19 = 1 ------ ROMDIAG or other


