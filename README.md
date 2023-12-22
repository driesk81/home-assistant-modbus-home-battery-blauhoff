# home-assistant-modbus-home-battery-blauhoff
## Let home assistant control your all in one home battery via modbus and esphome.

This yaml can be used to control Blauhoff all in one BMS systems, Ecactus and probably Copia will work as well (not tested)
The mean purpose is to make the BMS (battery management system) available in Home Assistant to make automated charge/discharge possible. 
use at your own risk.
 
# configuration: 
* Make sure that your wifi credentials are set and asign a ip address,gateway and subnetmask in the code below.
* This code is tested on a esp32 connected to a TTL to RS485 converter. 
* BMS settings can be selected via list options and are pushed when [change modus] button is pressed.
* Known issue:  Component modbus_controller took a long time for an operation (0.05 s) and Components should block for at most 20-30ms i seen no effect or solution.
* Please be kind this is the first yaml i have ever written :-)

# hardware used:
   * Blauhoff all in one BMS
   * ESP32
   * TTL to RS485 converter
   * some wire

# setup home assistant with: 
  * HACS
  * ESPHome
  * Power Flow Card

# setup 
Flash ESPHome to ESP32
Edit yaml on ESP32
 
 # Hardware setup
 
 ![setup](https://github.com/driesk81/home-assistant-modbus-home-battery-ecactus/assets/55897352/e2315b8a-ed8a-4822-b793-5e4281028a97)

 # Home assitant dashboard
 
 ![image](https://github.com/driesk81/home-assistant-modbus-home-battery-ecactus/assets/55897352/f6e18c19-a5ad-4ab8-90bd-63130ec8150a)
 ![image](https://github.com/driesk81/home-assistant-modbus-home-battery-ecactus/assets/55897352/095d6154-8d5e-41a0-9567-0aa620a13c8f)
 ![image](https://github.com/driesk81/home-assistant-modbus-home-battery-ecactus/assets/55897352/66d4971d-150e-4464-8f51-d36f7d1ae5d8)



 
