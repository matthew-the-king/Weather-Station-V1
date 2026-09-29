## Weather-Station-V1
The Weather Station V1 is a Solar- and Battery-powered Weather Station that measures humidity, pressure, temperature, and air quality, and sends all data over Wi-Fi for a client to receive.
<img width="1040" height="592" alt="image" src="https://github.com/user-attachments/assets/2a213a2a-b792-4a79-85fb-dfae104ab104" />
#|FEATURES IN DEPTH|<br>
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
The current configuration of the PCB requires 4 LiFePO4 batteries(https://www.digikey.com/en/products/detail/zeus-battery-products/PCIFR18650-1500/9828824)
The PCB has THT 18650 Battery holder footprint on the bottom side of the board, allowing for quick and easy connection of batteries to the PCB.<br>
<img width="646" height="517" alt="image" src="https://github.com/user-attachments/assets/ac735c87-fc3e-4118-975c-a809f7d4c57f" /><br>
The board has a USB-C port for each MCU to make programming as easy as possible, but in case the user does not want to use USB programming, there are also header pins on the other side of the
board that allow for ESP32 UART programming and STM32 serial wire debug and programming.<br>
<img width="234" height="152" alt="image" src="https://github.com/user-attachments/assets/7517952c-5eb3-4fa8-90c6-91cde3e78ec5" />
<img width="172" height="77" alt="image" src="https://github.com/user-attachments/assets/ff867981-08c1-4b19-8030-401d74fc0352" />
<img width="187" height="107" alt="image" src="https://github.com/user-attachments/assets/8a38d112-d87d-40e5-bf3b-fb82a8bf159f" /><br>
#|PRODUCTION|<br>
To produce the PCB, use your preferred PCB manufacturer (PCBway, JLCPCB, etc.).  The Bill of Materials is listed here(https://docs.google.com/spreadsheets/d/18tRwPWfDHP627m5xswZKQer6xHzLyA3w4jbUHwrpr4k/edit?gid=0#gid=0).
I would greatly recommend using a PCB stencil to make soldering components easier, as some of the components are quite small. Remember, in order for the battery functionality to work, JP1 and JP4 must be bridged.<br>
<br>
#|Purpose Of Project |<br>
The purpose of the Weather Station V1 was to enhance my understanding of RF applications and battery- and solar-powered devices. Throughout making this project, I understood RF design better and overall PCB design.
I hope this knowledge will allow me to make better, more reliable, and cooler projects in the future. 

