# DTS1946-4P_to_HUAWEI_translator
# Forked from salakrzy/DTSU666_CHINT_to_HUAWEI_translator

This project uses ESP32 to translate MODBUS messages of DTS1946-4P Energy Meter into HUAWEI DTSU666H format.
This project translates the DTS1946-4P Power Meter registers addreses to Huawei DTSU666H Power Meter addreses.

All data received from DTS1946-4P meter can be send to MQTT Broker.

Project base on the eMODBUS librrary  https://github.com/eModbus/eModbus 

Information on how to prepare enviroment, compile and flash ESP32 modules can be found at:
https://docs.espressif.com/projects/esp-idf/en/latest/esp32/get-started/index.html#

Project uses the Arduino.h librrary. How to instal this librrary in espressif enviroment, you can read at
https://docs.espressif.com/projects/arduino-esp32/en/latest/esp-idf_component.html

You will find hints how to assemble the hardware in the /doc project directory, plug DTS1946-4P exactly as chint666 mentioned on the schemes.
This project can be easily loaded into adruinoIDE.

In used RS485 interface the R5 and R6 resistors are 20k ohm it is to much for MOdbus standard, if you have transmission errors, change this resistors to 2k ohm.
If you change the R5 and R6 resistors,  you don't need remove the R7 120 ohm resistor.
