# H907Pro
MF601/MF800/H907Pro/H909Pro/etc... - An MSM8916 Based LTE/4G Hotspot with LCD (or Not)

## Images
| ![i1](images/Exterior1.jpg?raw=true) | ![i4](images/Interior2.jpg?raw=true) |
|--------------------------------------|----------------------------------|
| ![i2](images/Interior1.jpg?raw=true) | ![i5](images/Board.jpg?raw=true) |
| ![i3](images/BoardLCD.jpg?raw=true)  | ![i6](images/BoardUnmarked.jpg?raw=true) |

## Labeling
On the cover:
```
4G LTE WIFI MODEM
Wifi HotsPt
Model: E5783
SSID:E5783-LCD-1C0A
Password: 1234567890
IP: 192.168.100.1
USer/Key: admin
Power: 5V - 1A
```

## PCB Note & Markings:
```
MF601STC_V02
Z8X 07-05 
E465280
HF01 Z02
94V-0
13U00004A
```
# IC Details:
 ![i7](images/BoardMarking1.jpg?raw=true)

### **$\textsf{\color{#ff0000}{QUALCOMM MSM8916-6VV}}$**
This is the main SOC for the LTE Hotspot

### **$\textsf{\color{#ff9c00}{SK Hynix H9TQ32A4GTMC}}$**
```
BGA168 EMCP 4G+1G (Storage+Memory)
```
Clearly this is an storage and RAM combo in a single ic, you can upgrade with other emcp with the same BGA layout as well, according to datasheet of the SOC itself and other phones with the same chip.

### **$\textsf{\color{#00f6ff}{Qualcomm PM8916}}$**
Main power regular for whole device itself, easy to find replacement and datasheet, i'll providing power probes in futher updates

### **$\textsf{\color{#d800ff}{SMMI S5643-11}}$**
Multi-Mode Multi-Band Power Amplifier Module made by Smart Micro, i've found out this is can be replace with better PA ic with the same pinout S5643-62, i've ordered hopefully my theory works out

### **$\textsf{\color{12ff00}{Unknown IC (Marking DGFH)}}$**
To my knowlegde this probaly a FEM (Front End Module) IC, haven't found anything online related to this ic for now

### **$\textsf{\color{0000ff}{Qualcomm WTR4905}}$**
WTR4905 is a High pass RF transceiver IC

### **$\textsf{\color{fffc00}{Qualcomm WCN3620}}$**
Wifi IC with 2.4Ghz wifi support and BT4.0, it can coassistant with LTE. Bluetooth is disable by default inside device build.prop, i'll try to enable it.

### At this point this LTE Hotspot is just a freaking 2014 phone with a super small LCD display with resolution up to 128x128 pixel :))





