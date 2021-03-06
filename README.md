# Amiga4Kickstart

En este proyecto se trata de añadir al Amiga 1000 un reubicador de la cpu junto a una EPROM 27c160(2MB) para incluir hasta
4 kickstart diferentes añadiendo para ello una placa externa con un conmutador giratorio a traves del cual se puede seleccionar
la kickstart a cargar.
Se incluyen los esquematicos de las 3 placas necesarias junto a los gerbers.
El programador está diseñado para usarse con un programador TL866II plus.
La lista de componentes es la siguiente:


# Programador

| Cantidad      | Descripcion             | Formato                        |
| ------------- | ----------------------- | ------------------------------ |   
|      2        |  Zocalo de 42 pines     |                                |
|      2        |  Tira de 3 pines        |  2.54mm de paso                |
|      2        |  jumpers                |                                |
|      2        |  resistencias de 10K    |  0402 SMD                      |


# Reubicador

| Cantidad      | Descripcion             | Formato                        |
| ------------- | ----------------------- | ------------------------------ |   
|      2        |  Zocalo de 64 pin       |  DIP 64                        |
|      1        |  Zocalo de 42 pin       |  DIP 42                        |
|      1        |  Pin angulo recto 90º   |                                |
|      2        |  Tira de 64 pin         |  2.54mm macho                  |
|      1        |  Conector 4 pin         |  2.54mm                        |
|      1        |  EPROM 27c160           |  DIP 42                        |


# Conmutador

| Cantidad      | Descripcion               | Formato                        |
| ------------- | ------------------------- | ------------------------------ |   
|      1        |  Conmutador giratorio 3P4T| DIP                            |
|      2        |  Resistencia 10K          | 1206 SMD                       |
|      1        |  Conector 4 pin           | 2.54mm JST o similar           |


La configuración de puentes para programar la EPROM es la siguiente (a modo de ejemplo):


|               |                 |                 |
| ------------- | --------------- | --------------- |   
|    A18 = 0    |     A19 = 0     | KICKSTART (1.3) |
|    A18 = 1    |     A19 = 0     | KICKSTART (2.05)|
|    A18 = 0    |     A19 = 1     | KICKSTART (3.1) |
|    A18 = 1    |     A19 = 1     | ROMDIAG U OTRA  |





This project is intended to add an Amiga 1000 a CPU relocator with an EPROM 27c160(2M) to include up to 4 different kickstart
adding an external board with a rotary switch that selects the appropiate kickstart to load.
Schematics and gerbers for all boards are included.
The programmer board is designed to use with the TL866II plus programmer.
The BOM is the following:

# Programmer

| Quantity      | Description             | Package                        |
| ------------- | ----------------------- | ------------------------------ |   
|     2         |  42 pin IC Socket       |  DIP 42                        |
|     2         |  Jumpers                |                                |
|     2         |  10K Resistor           |  0402 SMD                      |


# Relocator

| Quantity      | Description             | Package                        |
| ------------- | ----------------------- | ------------------------------ |   
|      2        |  64 pin socket          |  DIP 64                        |
|      1        |  42 pin socket          |  DIP 42                        |
|      1        |  90º pin single         |                                |
|      2        |  64 pin strip           |  2.54mm macho                  |
|      1        |  4 pin connector        |  2.54mm                        |
|      1        |  EPROM 27c160           |  DIP 42                        | 


# Conmutador

| Cantidad      | Descripcion               | Formato                        |
| ------------- | ------------------------- | ------------------------------ |   
|      1        |  Rotary switch 3P4T       | DIP                            |
|      2        |  10K Resistor             | 1206 SMD                       |
|      1        |  4 pin connector          | 2.54mm JST or similar          |



The jumper configuration for the programmer board is the following (as an example):

|               |                 |                 |
| ------------- | --------------- | --------------- |   
|    A18 = 0    |     A19 = 0     | KICKSTART (1.3) |
|    A18 = 1    |     A19 = 0     | KICKSTART (2.05)|
|    A18 = 0    |     A19 = 1     | KICKSTART (3.1) |
|    A18 = 1    |     A19 = 1     | ROMDIAG / OTHER |


