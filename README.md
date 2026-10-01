# Weather-Station-V1
The Weather Station V1 is a Solar- and Battery-powered Weather Station that measures humidity, pressure, temperature, and air quality, and sends all data over Wi-Fi for a client to receive or records it to an SD card.
<img width="1040" height="592" alt="image" src="https://github.com/user-attachments/assets/2a213a2a-b792-4a79-85fb-dfae104ab104" />
## |FEATURES IN DEPTH|<br>
The Weather Station V1 uses multiple sensors to collect data; here is the list:<br>
1.STS40-AD1B-R3(Temperature Sensor)<br>
2.BMP581(Pressure Sensor)<br>
3.ENS160-BGLT(Air qaulity Sensor)<br>
4.SAM-M10Q-00B(GPS IC)<br>
To view the data the Weather Station V1 collects, the PCB has an SD card slot that records data over long periods and an ESP32-C3 that can send data over WiFi.<br>
<img width="283" height="254" alt="image" src="https://github.com/user-attachments/assets/eb9d54af-3096-42ad-96b8-0720b0d4d727" />
<img width="209" height="257" alt="image" src="https://github.com/user-attachments/assets/78601759-6eac-4327-90fd-bdbc29bcbc01" /><br>
The Weather Station V1 can be powered with a solar panel. To hook up the solar panel, connect the power wires with the correct polarity to the blue screw-in terminal.<br>
<img width="429" height="325" alt="image" src="https://github.com/user-attachments/assets/50c366fd-2385-418f-9957-bec3741ddaac" /><br>
The Weather Station V1 features an LTC4162, which is a LiFePO4 battery step-down charger with a Power path. To set up the cell count properly, JP1 and JP4 must be bridged. 
The current configuration of the PCB requires 4 LiFePO4 batteries(https://www.digikey.com/en/products/detail/zeus-battery-products/PCIFR18650-1500/9828824)
The PCB has THT 18650 Battery holder footprint on the bottom side of the board, allowing for quick and easy connection of batteries to the PCB.<br>
<img width="646" height="517" alt="image" src="https://github.com/user-attachments/assets/ac735c87-fc3e-4118-975c-a809f7d4c57f" /><br>
The board has a USB-C port for each MCU to make programming as easy as possible, but in case the user does not want to use USB programming, there are also header pins on the other side of the
board that allow for ESP32 UART programming and STM32 serial wire debug and programming.<br>
<img width="234" height="152" alt="image" src="https://github.com/user-attachments/assets/7517952c-5eb3-4fa8-90c6-91cde3e78ec5" />
<img width="172" height="77" alt="image" src="https://github.com/user-attachments/assets/ff867981-08c1-4b19-8030-401d74fc0352" />
<img width="187" height="107" alt="image" src="https://github.com/user-attachments/assets/8a38d112-d87d-40e5-bf3b-fb82a8bf159f" /><br>
## |PRODUCTION|<br>
To produce the PCB, use your preferred PCB manufacturer (PCBway, JLCPCB, etc.).  The Bill of Materials is listed here:<br>
| Designator | Footprint | Qty | Value / Part | Part Link |
|---|---|---:|---|---|
| BT5 | BAT_BK-18650-PC8 | 1 | BK-18650-PC8 | [Link](https://www.digikey.com/en/products/detail/mpd-memory-protection-devices/BK-18650-PC8/2330515)|
| C1 | 0603 | 1 | 330nF | [Link](https://www.digikey.com/en/products/detail/tdk/CGA3E3X7R1H334K080AB/4931465)|
| C10, C27, C3, C38, C39, C4, C40, C41, C45, C46, C5, C50, C51, C52, C53, C54, C6, C62, C63, C64, C9 | 0402 | 21 | 0.1uF |[Link](https://www.digikey.com/en/products/detail/samsung-electro-mechanics/CL05A104KA5NNNC/3886701?s=N4IgTCBcDaIMIBkAMBWAggRiQFgNJpQDli4QBdAXyA) |
| C11, C37, C44, C57, C65 | 0402 | 5 | 10uF |[Link](https://www.digikey.com/en/products/detail/murata-electronics/GRM155R60J106ME15D/5877401) |
| C12, C13, C16, C42, C43, C61, C66 | 0402 | 7 | 1uF |[Link](https://www.digikey.com/en/products/detail/samsung-electro-mechanics/CL05A105KO5NNNC/3886725) |
| C14 | 0402 | 1 | 22nF |[Link](https://www.digikey.com/en/products/detail/murata-electronics/GRM155R71H223KA12D/965898) |
| C15, C18, C2, C24, C26, C7 | 1210 | 6 | 10uF |[Link](https://www.digikey.com/en/products/detail/murata-electronics/GCJ32EC71H106KA01K/9867929) |
| C17, C22, C23, C29, C60, C67, C68, C69 | 0603 | 8 | 0.1uF |[Link](https://www.digikey.com/en/products/detail/kemet/C0603C104K5RACTU/1465594)|
| C25, C28 | CAP_EEH-ZA1V151P_PAN | 2 | 150uF |[Link](https://www.digikey.com/en/products/detail/panasonic-industry/EEH-ZA1V151P/3088122) |
| C34, C35, C36 | 0805 | 3 | 220nF |[Link](https://www.digikey.com/en/products/detail/kemet/C0805C224K5RACTU/754753) |
| C47, C48 | 0201 | 2 | C |Will Post link when Done with testing|
| C49 | 0603 | 1 | 4.7uF |[Link](https://www.digikey.com/en/products/detail/murata-electronics/GRM188R61E475KE11D/3900465) |
| C55, C8 | 0603 | 2 | 22uF |[Link](https://www.digikey.com/en/products/detail/holy-stone-enterprise-co-ltd/C0603B226M010T/16895513) |
| C56 | WCAP-PSHP_8X8.7_DXL_ | 1 | 470uF |[Link](https://www.digikey.com/en/products/detail/w%C3%BCrth-elektronik/875115252003/5147615) |
| C58 | 0402 | 1 | 470pF |[Link](https://www.digikey.com/en/products/detail/murata-electronics/GRM1555C1H471JA01D/587210) |
| C59 | 0402 | 1 | 100pF |[Link](https://www.digikey.com/en/products/detail/murata-electronics/GRM1555C1H101JA01D/3693829) |
| D1, D5, D6 | D_SOD-123F | 3 | 40V |[Link](https://www.digikey.com/en/products/detail/smc-diode-solutions/DSS14U/8341859) |
| D2 | D_SMA | 1 | D |[Link](https://www.digikey.com/en/products/detail/mcc-micro-commercial-components/SK310A-LTP/2642015) |
| D3 | D_SOD-123 | 1 | Zener 16V |[Link](https://www.digikey.com/en/products/detail/diodes-incorporated/DDZ9703-7/5218356) |
| D4 | D_SMA | 1 | 100V |[Link](https://www.digikey.com/en/products/detail/mcc-micro-commercial-components/SK310A-LTP/2642015) |
| ESP32_USB1, STM32_USB1 | SAMESKY_UJ20-C-H-G-SMT-P16-TR | 2 | UJ20-C-H-G-SMT-1-P16-TR |[Link](https://www.digikey.com/en/products/detail/same-sky-formerly-cui-devices/UJ20-C-H-G-SMT-P16-TR/24818595) |
| FB1, FB2 | 0603 | 2 | 120R |[Link](https://www.digikey.com/en/products/detail/pulse-electronics/PE-0603PFB121ST/5050544) |
| J1 | GCT_MEM2075-00-140-01-A | 1 | MEM2075-00-140-01-A |[Link](https://www.digikey.com/en/products/detail/gct/MEM2075-00-140-01-A/9859614) |
| J2 | TE_CONREVSMA002 | 1 | CONREVSMA002 |[Link](https://www.digikey.com/en/products/detail/te-connectivity-linx/CONREVSMA002/340145) |
| J3 | PinHeader_1x05_P2.54mm_Vertical | 1 | Conn_01x05_Pin |2.54mm Male Header Pins|
| J4 | PinHeader_1x04_P2.54mm_Vertical | 1 | Conn_01x04_Pin |2.54mm Male Header Pins|
| J5 | OST_OSTTC020162 | 1 | Solar Panel |[Link](https://www.amazon.com/dp/B01IFJ73X4?lv=shuf&rnid=2661611011&crid=3QHAHQSNMHFSL&keywords=solar%2Bpanels&sprefix=solar%2Bpanels%2Caps%2C245&th=1&dib_tag=se&dib=eyJ2IjoiMSJ9.NCFwgk3sAcXWyB454Pk5SPNcQemk34eTFudncpU4z0kJxmG-NXfIaFsG7l4m57yuxXUE0gBqu5lgGJoBbALUTFjF2K6-mGWYJWMwcwzsFfhhP3rzPJ4SUP1idMQb-H-VBpm4El9aRgOr08ZAze0ncVoFDJLv6Px1nW_MmPlfGzO2yde_wccv_r7rToX8MT91kRBLzjtbjo7iDcouW79qZ-3ntSCusWl1HjOpdd0R_DA.tXCmzJyMkYVnmj8B4maCWZT6sQgtKzylotzIh5rUZ2Y&qid=1789531833&refinements=p_36%3A-3800&sr=8-4&channelId=500&ref_=sr_1_4&plpRedirect=mhFallback) |
| JP1, JP2, JP3, JP4, JP5, JP6, JP7 | SolderJumper-2_P1.3mm_Open_TrianglePad1.0x1.5mm | 7 | Jumper_2_Open ||
| JP8, JP9 | PinSocket_1x02_P2.54mm_Vertical | 2 | Jumper_2_Open |2.54mm Male Header Pins|
| L1 | IND_PA4342.402NLT | 1 | 4uH |[Link](https://www.digikey.com/en/products/detail/pulse-electronics/PA4342-402NLT/5641799) |
| L2 | 0201 | 1 | L |Will Post link when Done with testing|
| L3 | 1008 | 1 | 1.5uH |[Link](https://www.digikey.com/en/products/detail/murata-electronics/DFE252012P-1R5M-P2/5247259) |
| Q10, Q9 | NPNBEC_SOT-23_OSI | 2 | BSR14 |[Link](https://www.digikey.com/en/products/detail/onsemi/BSR14/965251) |
| Q11, Q14 | WDFN8_511DR_OSI-L | 2 | FDMC8327L |[Link](https://www.digikey.com/en/products/detail/onsemi/FDMC8327L/4314821?curr=usd&utm_campaign=buynow&utm_medium=aggregator&utm_source=octopart) |
| Q3, Q4, Q5, Q6 | TDSON-8-1 | 4 | CSD18534Q5A |[Link](https://www.digikey.com/en/products/detail/texas-instruments/CSD18534Q5A/3830016) |
| R1 | 1206 | 1 | 16mΩ |[Link](https://www.digikey.com/en/products/detail/littelfuse-inc/L4CL1206LR016DNR/18795436) |
| R10, R11 | 2512 | 2 | 10MΩ |[Link](https://www.digikey.com/en/products/detail/bourns-inc/CHV2512-JW-106ELF/5175992) |
| R12, R13, R8, R9 | 0603 | 4 | 330Ω |[Link](https://www.digikey.com/en/products/detail/yageo/RC0603FR-07330RL/727162) |
| R14 | 0603 | 1 | 63.4k |[Link](https://www.digikey.com/en/products/detail/yageo/RT0603BRD0763K4L/1072610) |
| R15, R16 | 0402 | 2 | 10k |[Link](https://www.digikey.com/en/products/detail/yageo/RC0402JR-0710KL/726418?s=N4IgTCBcDaIEoGEAMAWJYBScC0SDsAjEgNIAyIAugL5A) |
| R2, R3, R39, R40 | 0402 | 4 | 4.7kΩ |[Link](https://www.digikey.com/en/products/detail/yageo/RC0402JR-074K7L/726477) |
| R20, R25 | 0603 | 2 | 300Ω |[Link](https://www.digikey.com/en/products/detail/yageo/RC0603FR-07300RL/724356) |
| R21, R22 | 2512 | 2 | 80.6Ω |[Link](https://www.digikey.com/en/products/detail/koa-speer-electronics-inc/RK73H3ATTE80R6F/10423948) |
| R23, R24, R26, R47, R48, R51, R52, R7 | 2010 | 8 | 100Ω |[Link](https://www.digikey.com/en/products/detail/yageo/RT2010FKE07100RL/5945596) |
| R27, R28, R29, R30 | 0402 | 4 | 5.1kΩ |[Link](https://www.digikey.com/en/products/detail/yageo/RC0402FR-075K1L/726624?s=N4IgTCBcDaIEoGEAMAWJYBicC0SDsArANICMAMiALoC%2BQA) |
| R31, R32, R33, R34, R37, R38, R43, R45, R49 | 0402 | 9 | 10kΩ |[Link](https://www.digikey.com/en/products/detail/yageo/RC0402JR-0710KL/726418?s=N4IgTCBcDaIEoGEAMAWJYBScC0SDsAjEgNIAyIAugL5A) |
| R35, R36 | 0402 | 2 | 22Ω |[Link](https://www.digikey.com/en/products/detail/yageo/RC0402FR-0722RL/726562) |
| R41 | 0402 | 1 | 100k |[Link](https://www.digikey.com/en/products/detail/yageo/RC0402FR-07100KL/726526) |
| R42 | 0402 | 1 | 31.6kΩ |[Link](https://www.digikey.com/en/products/detail/panasonic-industry/ERA-2AEB3162X/2026187) |
| R44, R53 | 0402 | 2 | 100kΩ |[Link](https://www.digikey.com/en/products/detail/yageo/RC0402FR-07100KL/726526) |
| R46 | MSRSF3920P1L00D2P0 | 1 | 1mΩ |[Link](https://www.digikey.com/en/products/detail/susumu/MSRSF3920P-1L00-D2P0/24396792) |
| R50 | 0805 | 1 | 32mΩ |[Link](https://www.digikey.com/en/products/detail/ohmite/MCS1632R025DER/22672428) |
| S1 | SW_SKRPABE010 | 1 | SKRPABE010 |[Link](https://www.digikey.com/en/products/detail/alps-alpine/SKRPABE010/18768948) |
| TH1 | PinHeader_1x02_P1.00mm_Vertical | 1 | 103AT2 |[Link](https://www.digikey.com/en/products/detail/semitec-usa-corp/103AT-2/16579059?s=N4IgTCBcDaIIwAYDMBBAKhAugXyA) |
| U1 | UFQFPN-32_STM | 1 | STM32U385KGU6 |[Link](https://www.digikey.com/en/products/detail/stmicroelectronics/STM32U385KGU6/26092104) |
| U10 | VQFN20_RGR_TEX | 1 | BQ76907RGRR |[Link](https://www.digikey.com/en/products/detail/texas-instruments/BQ76907RGRR/22077514) |
| U11 | SOT-23-5 | 1 | MIC5504-1.8YM5 |[Link](https://www.digikey.com/en/products/detail/microchip-technology/MIC5504-1-8YM5-TR/5209404) |
| U12, U13 | PSON50P145X100X60-6N | 2 | TPD4S012DRYR |[Link](https://www.digikey.com/en/products/detail/texas-instruments/TPD4S012DRYR/2037539) |
| U14 | IC_MCP16362T-E_NMX | 1 | MCP16362T-E_NMX |[Link](https://www.digikey.com/en/products/detail/microchip-technology/MCP16362T-E-NMXVAO/14291783) |
| U2 | QFN10_BMP581_BOS | 1 | BMP581 |[Link](https://www.digikey.com/en/products/detail/bosch-sensortec/BMP581/16036134) |
| U3 | STS4X | 1 | STS4X |[Link](https://www.digikey.com/en/products/detail/sensirion-ag/STS40-AD1B-R3/16020549) |
| U4 | XDCR_ENS210-LQFM | 1 | ENS210-LQFM |[Link](https://www.digikey.com/en/products/detail/sciosense/ENS210-LQFM/6490747) |
| U5 | XDCR_ENS160-BGLT | 1 | ENS160-BGLT |[Link](https://www.digikey.com/en/products/detail/sciosense/ENS160-BGLT/16129831) |
| U6 | QFN50P500X500X90-33N | 1 | LTC4162IUFD-FAD_PBF |[Link](https://www.digikey.com/en/products/detail/analog-devices-inc/LTC4162IUFD-FAD-PBF/9446112) |
| U7 | XCVR_SAM-M10Q-00B | 1 | SAM-M10Q-00B |[Link](https://www.digikey.com/en/products/detail/u-blox/SAM-M10Q-00B/16672678) |
| U8 | QFN50P500X500X90-33N | 1 | ESP32-C3FH4 |[Link](https://www.digikey.com/en/products/detail/espressif-systems/ESP32-C3FH4/14115592) |
| Y3 | OSC_ECS-2520S33-400-FN-TR | 1 | 40MHZ |[Link](https://www.digikey.com/en/products/detail/ecs-inc/ECS-2520S33-400-FN-TR/6578428) |

I would greatly recommend using a PCB stencil to make soldering components easier, as some of the components are quite small. Remember, in order for the battery functionality to work, JP1 and JP4 must be bridged.<br>
<br>
## |Purpose Of Project |<br>
The purpose of the Weather Station V1 was to enhance my understanding of RF applications and battery- and solar-powered devices. Throughout making this project, I understood RF design better and overall PCB design.
I hope this knowledge will allow me to make better, more reliable, and cooler projects in the future. 

