# Weather-Station-V1
The Weather Station V1 is a Solar- and Battery-powered Weather Station that measures humidity, pressure, temperature, and air quality, and sends all data over Wi-Fi for a client to receive.
<img width="1040" height="592" alt="image" src="https://github.com/user-attachments/assets/2a213a2a-b792-4a79-85fb-dfae104ab104" />
|FEATURES IN DEPTH|
The Weather Station V1 uses multiple sensors to collect data; here is the list:<br>
1.STS40-AD1B-R3(Temperature Sensor)<br>
2.BMP581(Pressure Sensor)<br>
3.ENS160-BGLT(Air qaulity Sensor)<br>
4.SAM-M10Q-00B(GPS IC)<br>
To view the data the Weather Station V1 collects, the PCB has an SD card slot that records data over long periods and an ESP32-C3 that can send data over WiFi.<br>
<img width="283" height="254" alt="image" src="https://github.com/user-attachments/assets/eb9d54af-3096-42ad-96b8-0720b0d4d727" />
<img width="209" height="257" alt="image" src="https://github.com/user-attachments/assets/78601759-6eac-4327-90fd-bdbc29bcbc01" /><br>
The Weather Station V1 can be powered with a solar panel. To hook up the solar panel, connect the power wires in the correct polarity to the blue screw-in terminal.<br>
<img width="429" height="325" alt="image" src="https://github.com/user-attachments/assets/50c366fd-2385-418f-9957-bec3741ddaac" /><br>
The Weather Station V1 features an LTC4162, which is a LiFePO4 battery step-down charger with a Power path. To set up the cell count properly, JP1 and JP4 must be bridged. 
The current configuration of the PCB requires 4 LiFePO4 batteries(https://www.digikey.com/en/products/detail/zeus-battery-products/PCIFR18650-1500/9828824)<br>
|PRODUCTION|
To produce the PCB, use your preferred PCB manufacturer (PCBway, JLCPCB, etc.).  The Bill of Materials is listed here(https://docs.google.com/spreadsheets/d/18tRwPWfDHP627m5xswZKQer6xHzLyA3w4jbUHwrpr4k/edit?gid=0#gid=0).
I would greatly recommend using a PCB stencil to make soldering components easier, as some of the components are quite small. 
|Purpose Of Project |
The purpose of the Weather Station V1 was to enhance my understanding of RF applications and battery- and solar-powered devices. Throughout making this project, I understood RF design better and overall PCB design.
I hope this knowledge will allow me to make better, more reliable, and cooler projects in the future. 

