# home-assistant-modbus-home-battery-ecactus
## Let home assistant control your all in one home battery via modbus and esphome.

This yaml can be used to control Ecactus and Blauhoff all in one BMS systems and probably copia as well (not tested)
The mean purpose is to make the BMS (battery management system) available in Home Assistant to make automated charge/discharge possible. 
use at your own risk.
 
# configuration: 
* Make sure that your wifi credentials are set and asign a ip address,gateway and subnetmask in the code below.
* This code is tested on a esp32 connected to a TTL to RS485 converter. 
* BMS settings can be selected via list options and are pushed when [change modus] button is pressed.
* Known issue:  Component modbus_controller took a long time for an operation (0.05 s) and Components should block for at most 20-30ms i seen no effect or solution.
Please be kind this is the first yaml i have ever written :-)

hardware used:
   * ESP32
   * TTL to RS485 converter
   * some wire

setup home assistant with: 
  * HACS
  * ESPHome
  * Power Flow Card

Flash ESPHome to ESP32
Edit yaml on ESP32
 
 # Hardware setup
 
 ![setup](https://github.com/driesk81/home-assistant-modbus-home-battery-ecactus/assets/55897352/e2315b8a-ed8a-4822-b793-5e4281028a97)
