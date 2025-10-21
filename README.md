# Weather Station

## English Version

This project provides a compact weather monitoring system built with a Wemos D1 board running Tasmota firmware, communicating via MQTT to a Node-RED server.
Sensor data is sent as MQTT messages to a Node-RED system running on a Raspberry Pi, where it is processed and visualized.

### ✨ Features
	•	Wireless weather station based on Wemos D1 (ESP8266)
	•	Uses Tasmota firmware for easy configuration and MQTT integration
	•	Data transmission via MQTT
	•	Visualization and data logging in Node-RED
	•	Extendable with additional sensors (e.g., light, rain, wind)

### 🛠️ Technologies
	•	Wemos D1 (ESP8266) with Tasmota firmware
	•	MQTT for communication
	•	Node-RED for data processing and dashboard visualization
	•	Raspberry Pi as the central server (optional)
-------

## Magyar verzió

Ez a projekt egy kompakt időjárás-állomás, amely Wemos D1 (ESP8266) alapú mikrokontrollerrel és Tasmota firmware-rel működik, az adatokat MQTT kapcsolaton keresztül továbbítja egy Node-RED szerverre.
Az érzékelők adatai MQTT üzenetként kerülnek továbbításra a Raspberry Pi-n futó Node-RED rendszerre, ahol feldolgozásra és megjelenítésre kerülnek.

### ✨ Főbb jellemzők
	•	Vezeték nélküli időjárás-állomás Wemos D1 (ESP8266) alapokon
	•	Tasmota firmware a könnyű beállításhoz és MQTT integrációhoz
	•	Adatküldés MQTT-n keresztül
	•	Node-RED alapú megjelenítés és naplózás
	•	Bővíthető további szenzorokkal (pl. fény, csapadék, eső, szél)

### 🛠️ Használt technológiák
	•	Wemos D1 (ESP8266) Tasmota firmware-rel
	•	MQTT kommunikációhoz
	•	Node-RED az adatok feldolgozásához és vizualizálásához
	•	Raspberry Pi központi szerverként (opcionális)

### 📅 Fejlesztési ütemterv

	1. Alap rendszer és érzékelők (folyamatban)
	A Wemos D1 Tasmota firmware-rel működik, hőmérséklet-érzékelők csatlakoztatva.  
	Következő lépés: Raspberry Pi telepítése Node-RED és MQTT brokerrel az adatok megjelenítéséhez.

	2. Kültéri tesztelés (tervezett)  
	A szerkezet kihelyezése a szabadba teszteléshez.  
	A szenzorok működésének, Wi-Fi jelnek és adatküldésnek ellenőrzése.

	3. Mérőház és telepítés (tervezett)
	Időjárásálló mérőház építése, érzékelők (talajhőmérséklet, talajnedvesség) telepítése.

	4. Napelemes tápellátás (tervezett)
	Napelemes és akkumulátoros energiaellátás a teljesen önálló működéshez.
---------

### Wemos d1 (pro) PINs:

- GPIO04 - D2 SDA - BME280
- GPIO05 - D1 SCL - BME280
- GPIO14 - D5     -	DS18B20 x2 (air temperature, soil temperature)
- GPIO17 - ADC0   -	Capacitive Soil Moisture Sensor

<p align="center">
  <img src="screenshots/wemosd1/WeatherStationCircuit.jpg" width="45%">
</p>

### Tasmota WebUI:
<p align="center">
  <img src="screenshots/Tasmota/WebUIstartpage.png" width="35%">
</p>
