# dpf-monitor-v2
DPF MONITOR Alfa Romeo 159 Instrument Cluster Display
DPF MONITOR Alfa Romeo | Opening Ceremony | Sweep-up Gauges | Alfa Romeo 159

https://www.youtube.com/watch?v=yD4FI52CANM


Below is presented the construction and commissioning instructions for the DPF MONITOR module prototype for the Alfa Romeo 159 JTDm. The module can be plugged directly into the OBDII socket. For its operation, no additional devices or modules in the ELM USB / RS232 / Bluetooth / WiFi interface style are required - the presented module is fully independent.

The main task of the module is the continuous monitoring of the DPF clogging / burnout status and on-demand display of the DPF status data on the central display between the so-called clocks. ICD Instruments Cluster Display.

An additional built-in function is the so-called Opening Ceremony, which is activated after inserting the key into the ignition.


List of used elements:
ATMEGA328P-AU TQFP32
PCA82C250T SO8
MCP2515-I/SO SO18L
L9637D SO08
7805DT TO252
S2M DO214AC
10uH 1812
27pF 1206
10uF UD5x5,8
47uF UD5x5,8
100nF 1206
510R 1206
47k 1206
120R 1206
10k 1206
8MHz SM49
16MHz SM49


user@iMac 20210518_ECU_v2_41_dev % avrdude -c USBasp -p m328p -U flash:w:20210518_ECU_v2_41_dev.ino.with_bootloader.eightanaloginputs.hex -B4

avrdude: set SCK frequency to 187500 Hz

avrdude: AVR device initialized and ready to accept instructions

Reading | ################################################## | 100% 0.00s

avrdude: Device signature = 0x1e950f (probably m328p)

avrdude: NOTE: "flash" memory has been specified, an erase cycle will be performed To disable this feature, specify the -D option.

avrdude: erasing chip

avrdude: set SCK frequency to 187500 Hz

avrdude: reading input file "20210518_ECU_v2_41_dev.ino.with_bootloader.eightanaloginputs.hex"

avrdude: input file 20210518_ECU_v2_41_dev.ino.with_bootloader.eightanaloginputs.hex auto detected as Intel Hex

avrdude: writing flash (32670 bytes):

Writing | ################################################## | 100% 9.33s

avrdude: 32670 bytes of flash written

avrdude: verifying flash memory against 20210518_ECU_v2_41_dev.ino.with_bootloader.eightanaloginputs.hex:

avrdude: load data flash data from input file 20210518_ECU_v2_41_dev.ino.with_bootloader.eightanaloginputs.hex:

avrdude: input file 20210518_ECU_v2_41_dev.ino.with_bootloader.eightanaloginputs.hex auto detected as Intel Hex

avrdude: input file 20210518_ECU_v2_41_dev.ino.with_bootloader.eightanaloginputs.hex contains 32670 bytes

avrdude: reading on-chip flash data:

Reading | ################################################## | 100% 4.72s

avrdude: verifying ...

avrdude: 32670 bytes of flash verified

avrdude: safemode: Fuses OK (E:FD, H:DA, L:FF)

avrdude done. Thank you.

user@iMac 20210518_ECU_v2_41_dev %







Compatibile ECU and cars with this tool:

Bosch EDC16C39 CF4/EOBD (engine 1.9/2.4)

ALFA, 147, 1.9 JTD ALFA, 147, 1.9 JTD 16V ALFA, 156 '02, 1.9 JTD 16V ALFA, 159, 1.9 MJET 16V ALFA, 159, 1.9 MJET 8V ALFA, 159, 2.4 MJET 20V ALFA, 166, '03 2.4 JTD 20V ALFA, BRERA, 2.4 MJET 20V ALFA, GT, 1.9 JTD 16V FIAT, BRAVO '07, 1.9 MJET 16V FIAT, BRAVO '07, 1.9 MJET 8V FIAT, CROMA '05, 1.9 MJET 16V FIAT, CROMA '05, 1.9 MJET 8V FIAT, CROMA '05, 2.4 MJET 20V FIAT, DOBLO', 1.9 JTD FIAT, MULTIPLA, '02 1.9 JTD FIAT, STILO, 1.9 JTD FIAT, STILO, 1.9 JTD 16V LANCIA, THESIS, 2.4 JTD 20V
