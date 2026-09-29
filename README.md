# Weather-Station-V1
The Weather Station V1 is a Solar- and Battery-powered Weather Station that measures humidity, pressure, temperature, and air quality, and sends all data over Wi-Fi for a client to receive.
<img width="1040" height="592" alt="image" src="https://github.com/user-attachments/assets/2a213a2a-b792-4a79-85fb-dfae104ab104" />
|FEATURES IN DEPTH|
The Weather Station V1 uses multiple sensors to collect data; here is the list:\n
1.STS40-AD1B-R3(Temperature Sensor)
2.BMP581(Pressure Sensor)
3.ENS160-BGLT(Air qaulity Sensor)
4.SAM-M10Q-00B(GPS IC)
To view the data the Weather Station V1 collects, the PCB has an SD card slot that records data over long periods and an ESP32-C3 that can send data over WiFi.
The Weather Station V1 can be powered with a solar panel. To hook up the solar panel, connect the power wires in the correct polarity to the blue screw-in terminal.
<img width="429" height="325" alt="image" src="https://github.com/user-attachments/assets/50c366fd-2385-418f-9957-bec3741ddaac" />
The Weather Station V1 features an LTC4162, which is a LiFePO4 battery step-down charger with a Power path. To set up the cell count properly, JP1 and JP4 must be bridged. 
The current configuration of the PCB requires 4 LiFePO4 batteries(https://www.digikey.com/en/products/detail/zeus-battery-products/PCIFR18650-1500/9828824) 
