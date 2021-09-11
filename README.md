# AX80
One chip ZX81 based on the Atmega1284p

Under Windows at the command prompt flash the atmega using avrdude with

avrdude -c usbtiny -p m1284p -e -U flash:w:ax81.hex

and set the fuses with

avrdude -c usbasp -F -p m1284p -U lfuse:w:0xe6:m -U hfuse:w:0xd1:m -U efuse:w:0xfc:m

alternatively run the two enclosed .bat files, but ensure the ax81.hex is in the same folder.

Partlist

Exported from ax80.brd at 11/09/2021 11:26:11

EAGLE Version 6.5.0 Copyright (c) 1988-2013 CadSoft

Assembly variant: 

Part      Value

C201      1µ                   

C202      100n                  

C203      22p                   

C204      22p                  

C205      100n                  C025-025X050   rcl            (2450 3080)           R180

C501      100n                  C025-025X050   rcl            (2985 1870)           R90

C502      100n                  C025-025X050   rcl            (3650 1150)           R90

C601      220µ                  E3,5-8         rcl            (875 330)             R270

C602      100µ                  E2,5-6         rcl            (1875 160)            R180

C603      100n                  C025-025X050   rcl            (1880 415)            R180

C604      100µ                  E2,5-6         rcl            (1875 685)            R180

C605      100n                  C025-025X050   rcl            (2635 1080)           R180

CN1                             DCJACK_2MM_PTH adafruit       (175 -5)              R0

D601      1N4004                DIODE-1N4148   SparkFun       (905 650)             R0

EXPANSION PAR                   ML26           con-harting-ml (3250 3700)           R180

IC201     ATMEGA644P/1284P-20PU DIL40          atmel          (2945 2390)           R180

IC501     74AHC125N             DIL14          74xx-eu        (3400 1550)           R0

IC601     L4940V5               78XXL          SparkFun       (1330 610)            R180

IC602     LM3940IT-3.3          78XXL          SparkFun       (1330 1090)           R0

JP1                             JP1            jumper         (1010 3620)           R180

JP2       WP                    JP1            jumper         (1255 3615)           R180

JP3       SD DET                JP1            jumper         (1510 3615)           R180

JP4                             JP1            jumper         (1720 3615)           R180

JP101     S/W                   1X04           SparkFun       (2020 3010)           R180

JP601                           JP1            jumper         (1060 3000)           R270

KEYBOARD  PS2                   M_DIN6         mini_din       (3700 300)            R180

LED1                            LED3MM         adafruit       (560 130)             R180

Q201      20MHz                 HC49US         SparkFun       (2750 3350)           R180

R101      1k                    0204/7         rcl            (905 2485)            R90

R102      1k8                   0204/7         rcl            (1055 2485)           R90

R103      3k3                   0204/7         rcl            (1640 2490)           R90

R104      1k                    0204/7         rcl            (1790 2490)           R90

R105      470                   0204/7         rcl            (1495 2490)           R90

R106      470                   0204/7         rcl            (1350 2490)           R90

R107      470                   0204/7         rcl            (1205 2485)           R90

R201      10k                   0204/7         rcl            (3205 855)            R90

R202      10k                   0204/7         rcl            (3355 855)            R90

R203      10k                   0204/7         rcl            (2890 850)            R90

R204      10k                   0204/7         rcl            (3045 850)            R90

R401      180                   0204/7         rcl            (3765 3245)           R270

R402      180                   0204/7         rcl            (3655 2970)           R270

R403      180                   0204/7         rcl            (3555 3245)           R270

R404      180                   0204/7         rcl            (3455 2970)           R270

R405      180                   0204/7         rcl            (3360 3255)           R270

R406      180                   0204/7         rcl            (3250 2975)           R270

R407      180                   0204/7         rcl            (3155 3255)           R270

R408      180                   0204/7         rcl            (3055 2970)           R270

R501      10k                   0204/7         rcl            (2015 955)            R0

R502      10k                   0204/7         rcl            (2015 1095)           R0

R503      10k                   0204/7         rcl            (2010 1235)           R0

R504      10k                   0204/7         rcl            (2010 1385)           R0

R505      10k                   0204/7         rcl            (2010 1535)           R0

R601      240                   0204/7         rcl            (555 460)             R90

R701      10k                   0204/7         rcl            (3800 850)            R90

R702      10k                   0204/7         rcl            (3500 850)            R90

R703      100                   0204/7         rcl            (3950 845)            R90

R704      100                   0204/7         rcl            (3645 850)            R90

S1        Output select         DP-04-PHW      GKR            (2150 3600)           R180

S2                              TACTILE-PTH    SparkFun2      (3200 250)            R270

U$5       SD-SDAMB              SD-SDAMB       GKR            (50 1350)             MR0

VGA101    VGA                   HDF15H         con-subd       (500 2670)            R270

VIDEO101  Cinch                 736880-49      GKR            (500 3600)            R0

WS801     AVR_SPI_PRG_6         ML6            Propeller      (2355 265)            R0
