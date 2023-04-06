# DTS1946-4P_to_HUAWEI_translator
# Forked from salakrzy/DTSU666_CHINT_to_HUAWEI_translator

AdruinoIDE ready project.

ESP32 will translate MODBUS messages and registers addreses of DTS1946-4P Energy Meter into HUAWEI DTSU666H format.

All data received from DTS1946-4P meter can be also send to MQTT Broker.
You will find hints on how to assemble the hardware in the /doc project directory, plug DTS1946-4P exactly as chint666 mentioned on the schemes.

In used RS485 interface the R5 and R6 resistors are 20k ohm it is to much for MOdbus standard, if you have transmission errors, change this resistors to 2k ohm.
If you change the R5 and R6 resistors,  you don't need remove the R7 120 ohm resistor.

Project is based on the eMODBUS librrary https://github.com/eModbus/eModbus 
