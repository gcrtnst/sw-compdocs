# Sensors

## Altimeter

An altitude sensor.

Outputs distance above sea-level in meters.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $20
- Tags: aeroplane,airplane,helicopter
- File: altimeter.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Altitude | The measured altitude of the component in metres above sea-level. |

## Angular Speed Sensor

This sensor outputs its current angular speed in rotations per second, allowing you to measure how fast your vehicle is rotating.

This sensor outputs the angular speed of the component about the component's y axis.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $20
- Tags: 
- File: angular_speed_sensor.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Angular Speed | The sensor's angular speed in rotations per second. |

## Astronomy Sensor

A sensor that provides raw space navigation data.

Outputs relative position data based on the optimal target trajectory between the earth and moon.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $150
- Tags: 
- File: astronomy_sensor.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| composite | Data | Outputs [1] x position in metres, [2] y position in metres (earth sea level is 0), [3] z position in metres, [4] euler rotation x, [5] euler rotation y, [6] euler rotation z, [7] angular velocity x, [8] angular velocity y, [9] angular velocity z, [10] local z tilt and [11] local x tilt to the respective composite channels. |

## Compass Sensor

A digital compass that outputs a number value representing the turn that must be made for it to face north.

The sensor has a display to visualise the direction of north. The measured output is taken relative to the white arrow on the face of the display.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x2
- Cost: $20
- Tags: 
- File: compass_sensor.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Backlight | Enables the backlight when receiving an on signal. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Compass Reading | The angle measured in turns that the needle is rotated from the white arrow on the display. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Contact Sensor

A sensor activated by contact pressure.

Setting the resistance property will tune the amount of contact required to depress the sensor. When depressed, an on signal will be produced.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x2
- Cost: $20
- Tags: 
- File: pressure_sensor.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Output | Outputs an on signal when the contact sensor is depressed. |

## Distance Sensor

A laser distance sensor with a maximum measurement range of 500m.

The reading can be read from the sensor's number output and is measured in metres (1 metre = 4 blocks).

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x2
- Cost: $20
- Tags: laser,lazer
- File: distance_sensor.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Distance | The measured distance in metres. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Fishfinder

A sensor that returns information about a fish within 100m when submerged.

This sensor outputs the relative angle, distance and depth to a random detected fish within its range using sound waves when submerged.

### PROPERTIES

- Mass: 10
- Dimensions (WxDxH): 1x1x1
- Cost: $500
- Tags: sonar
- File: fish_finder.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Activate | Enable the Fishfinder. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| composite | Fish Data | Outputs data for a detected fish. On/Off 1: Returns true when a fish is detected. Value 1: The yaw angle between the sensor and the detected fish measured in turns, Value 2: The horizontal distance from the sensor to the detected fish measured in metres, Value 3: The depth from the sensor to the fish measured in metres. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Gas Meter

A device to measure how much gas is within an enclosed volume.

This will output a quantity in litres and the total capacity in litres.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x2
- Cost: $20
- Tags: 
- File: gas_measure.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Gas Level | Returns the number of litres of gas in an enclosed volume. |
| number | Fluid Capacity | Returns the total capacity of an enclosed volume in litres, or 0 if not enclosed. |
| composite | Composite Data | Outputs the volumes of individual gas types on their respective channel. The data can be directly merged with a Liquid meter. The Air fluid type is equivalent to the sum of the oxygen, carbon dioxide and nitrogen values. Channels: 4-Air, 5-CO2, 8-Steam, 11-Oxygen, 12-Nitrogen, 13-Hydrogen. |

## GPS Sensor

Outputs its x and y world coordinates according to its location on the map.

The coordinates represent an offset from the centre of the world, measured in metres. You can check the world coordinates of any location by looking at your map.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x2x1
- Cost: $20
- Tags: 
- File: gps_sensor.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | X Coordinate | The x coordinate of this component on the world map. |
| number | Y Coordinate | The y coordinate of this component on the world map. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Humidity Sensor

A humidity sensor for measuring the current fog and visibility meteorological conditions.

The reading can be read from the sensor's number output and is measured from 0 (no fog) to 1 (max fog).

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x2
- Cost: $400
- Tags: 
- File: humidity_sensor.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Humidity Factor | The level of humidity in the air, relating to the fog visibility. |

## Impact Sensor

A sensor activated by a sudden change in velocity.

Setting the impact threshold property will tune the sensitivity for impacts. When the instant change in velocity from an impact exceeds the threshold, an on signal is produced.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $20
- Tags: 
- File: impact_sensor.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Output | Outputs an on signal when instant change in velocity exceeds the impact threshold. |

## Laser Distance Sensor

A laser distance sensor with a maximum measurement range of 4000m.

The reading can be read from the sensor's number output and is measured in metres (1 metre = 4 blocks). Can be pivoted up to 0.125 turns using composite input.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x4
- Cost: $100
- Tags: 
- File: laser_distance_sensor.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Active | Controls whether or not the laser is active. |
| number | Wavelength | The specific light wavelength to emit (whole number). |
| composite | Pivot | Inputs for laser X/Y pivot. (Value 1 : Pivot X) (Value 2 : Pivot Y) |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Distance | The measured distance in metres. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Laser Point Sensor

A sensor that outputs a relative x and y position of a laser point that it can see within its field of view.

The closest point to the center of the sensor's field of view will be reported. It outputs a value of -1 to 1 on composite number channel 1 for the x position, and a value of -1 to 1 on composite number channel 2 for the y position. Composite on/off channel 1 is set to on when a point is visible. The -1 to 1 values map to an fov of -cos(0.5) to cos(0.5) in both the x and y directions.

### PROPERTIES

- Mass: 2
- Dimensions (WxDxH): 1x1x3
- Cost: $100
- Tags: 
- File: laser_point_sensor.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| number | Wavelength | The specific light wavelength to detect (whole number). |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| composite | Data Output | On/Off channel 1: is laser detected. Number channel 1, 2: X, Y position within the sensors 120 degree field of view. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Laser Sensor (Missile)

A short range sensor that returns information about detected laser points within its view.

This sensor is designed for missiles and acts along the Z axis, with an output node that passes data to course correct linked rocket fin components toward the closest target. The sensor also outputs data for up to 8 detected laser points.

### PROPERTIES

- Mass: 5
- Dimensions (WxDxH): 1x1x2
- Cost: $800
- Tags: 
- File: radar_advanced_missile_laser.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Activate | Enable the Laser Sensor. |
| number | Wavelength | The specific light wavelength to detect (whole number). |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| composite | Sensor Data | Outputs data for up to 8 targets. On/Off 1-8 : Target 1 Found, Target 2 Found, etc... Values 1-32 : Target 1 Distance, Target 1 Azimuth Angle, Target 1 Elevation Angle, Target 1 Time Since Detection, Target 2 Distance, Target 2 Azimuth Angle, Target 2 Elevation Angle, Target 2 Time Since Detection, etc... |
| composite | Missile Output | Outputs x and y data for the most immediate target. Link this directly into a rocket fins component. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Linear Speed Sensor

This sensor outputs its current linear speed in m/s, allowing you to measure how fast your vehicle is travelling.

This sensor outputs the speed of the component in one of 4 modes. Modes can be changed by selecting the sensor.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $20
- Tags: 
- File: linear_speed_sensor.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Linear Speed | The sensor's linear speed in m/s. |

## Liquid Meter

A device to measure how much liquid is within an enclosed volume.

This will output a quantity in litres and the total capacity in litres. If not inside an enclosed volume, it will give the height relative to the water surface.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x2
- Cost: $20
- Tags: fluid,measure
- File: water_measure.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Liquid Level | Returns the number of litres of liquid in an enclosed volume, or height relative to water if not enclosed. |
| number | Fluid Capacity | Returns the total capacity of an enclosed volume in litres, or 0 if not enclosed. |
| composite | Composite Data | Outputs the volumes of individual liquid types on their respective channel. The data can be directly merged with a Gas meter. Channels: 1-Water, 2-Diesel, 3-Jet Fuel, 6-Oil, 7-Seawater, 9-Slurry, 10-Saturated Slurry |

## Microphone

A microphone for transmitting player voice data.

A simple microphone that picks up voice data from nearby players. (Range : 15)

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x2
- Cost: $250
- Tags: 
- File: mic.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Activate | Activate the microphone. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| audio | Audio | Audio data connection. |
| on/off | Transmit | If the microphone is currently transmitting. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Physics Sensor

Sensor component that outputs various physics measurements such as position and velocity.

Outputs physics information to a composite logic node. Requires Electric for GPS position functionality. This component is directed along its local Y axis.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $20
- Tags: 
- File: physics_sensor.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| composite | Composite Output | Outputs [1] x position, [2] y position, [3] z position, [4] euler rotation x, [5] euler rotation y, [6] euler rotation z, [7] linear velocity x, [8] linear velocity y, [9] linear velocity z, [10] angular velocity x, [11] angular velocity y, [12] angular velocity z, [13] absolute linear velocity, [14] absolute angular velocity, [15] local z tilt, [16] local x tilt and [17] compass heading (-0.5 to 0.5) to the respective composite channels. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Player Sensor

A sensor that outputs the number of players detected within an area.

If the sensor is facing into a sealed room, only players inside that room will be detected. Likewise, players inside sealed rooms will not be detected if the sensor is placed on the outside. The size of the area and types of players to detect can be changed by selecting this component with the select tool.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x2
- Cost: $50
- Tags: 
- File: player_sensor.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Number Detected | The number of players detected by the sensor. |
| on/off | Detected | Outputs an on signal if any players are detected. |

## Radar (AWACS)

A long range radar that returns information about a detected object within its view.

This sensor outputs the distance and relative angle to a detected object within its range and field of view using radio waves. Sensitivity is based on FOV, target size, and distance.

### PROPERTIES

- Mass: 1100
- Dimensions (WxDxH): 37x37x5
- Cost: $10000
- Tags: 
- File: radar_advanced_awacs.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Activate | Enable the Radar. |
| composite | Gimbal Input | Inputs rotation data for radar in manual mode. Value 1: The yaw angle of the radar measured in turns, Value 2: The pitch angle of the radar measured in turns from -0.125 to 0.125. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| composite | Radar Data | Outputs data for up to 8 targets. On/Off 1-8 : Target 1 Found, Target 2 Found, etc... Values 1-32 : Target 1 Distance, Target 1 Azimuth Angle, Target 1 Elevation Angle, Target 1 Time Since Detection, Target 2 Distance, Target 2 Azimuth Angle, Target 2 Elevation Angle, Target 2 Time Since Detection, etc... |
| number | Radar Rotation | Current radar rotation from forward in turns. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Radar (Basic)

A radar that returns information about a detected object within its view.

This sensor outputs the distance and relative angle to a detected object within its range and field of view using radio waves. Sensitivity is based on FOV, target size, and distance.

### PROPERTIES

- Mass: 10
- Dimensions (WxDxH): 3x3x1
- Cost: $1000
- Tags: 
- File: radar_advanced.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Activate | Enable the Radar. |
| composite | Gimbal Input | Inputs rotation data for radar in manual mode. Value 1: The yaw angle of the radar measured in turns, Value 2: The pitch angle of the radar measured in turns from -0.125 to 0.125. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| composite | Radar Data | Outputs data for up to 8 targets. On/Off 1-8 : Target 1 Found, Target 2 Found, etc... Values 1-32 : Target 1 Distance, Target 1 Azimuth Angle, Target 1 Elevation Angle, Target 1 Time Since Detection, Target 2 Distance, Target 2 Azimuth Angle, Target 2 Elevation Angle, Target 2 Time Since Detection, etc... |
| number | Radar Rotation | Current radar rotation from forward in turns. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Radar (Dish)

A radar that returns information about a detected object within its view.

This sensor outputs the distance and relative angle to a detected object within its range and field of view using radio waves. Sensitivity is based on FOV, target size, and distance.

### PROPERTIES

- Mass: 550
- Dimensions (WxDxH): 19x20x10
- Cost: $5000
- Tags: 
- File: radar_advanced_dish.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Activate | Enable the Radar. |
| composite | Gimbal Input | Inputs rotation data for radar in manual mode. Value 1: The yaw angle of the radar measured in turns, Value 2: The pitch angle of the radar measured in turns from -0.125 to 0.125. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| composite | Radar Data | Outputs data for up to 8 targets. On/Off 1-8 : Target 1 Found, Target 2 Found, etc... Values 1-32 : Target 1 Distance, Target 1 Azimuth Angle, Target 1 Elevation Angle, Target 1 Time Since Detection, Target 2 Distance, Target 2 Azimuth Angle, Target 2 Elevation Angle, Target 2 Time Since Detection, etc... |
| number | Radar Rotation | Current radar rotation from forward in turns. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Radar (Missile)

A short range radar that returns information about a detected object within its view.

This sensor outputs the distance and relative angle to a detected object within its range and field of view using radio waves. This sensor is designed for missiles and its radar acts along the Z axis. Sensitivity is based on FOV, target size, and distance.

### PROPERTIES

- Mass: 5
- Dimensions (WxDxH): 1x1x2
- Cost: $800
- Tags: 
- File: radar_advanced_missile.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Activate | Enable the Radar. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| composite | Radar Data | Outputs data for up to 8 targets. On/Off 1-8 : Target 1 Found, Target 2 Found, etc... Values 1-32 : Target 1 Distance, Target 1 Azimuth Angle, Target 1 Elevation Angle, Target 1 Time Since Detection, Target 2 Distance, Target 2 Azimuth Angle, Target 2 Elevation Angle, Target 2 Time Since Detection, etc... |
| composite | Missile Output | Outputs x and y data for the most immediate target. Link this directly into a rocket fins component. |
| number | Radar Rotation | Current radar rotation from forward in turns. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Radar (Phalanx)

A radar that returns information about a detected object within its view.

This sensor outputs the distance and relative angle to a detected object within its range and field of view using radio waves. Sensitivity is based on FOV, target size, and distance.

### PROPERTIES

- Mass: 55
- Dimensions (WxDxH): 3x3x3
- Cost: $2000
- Tags: 
- File: radar_advanced_phalanx.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Activate | Enable the Radar. |
| composite | Gimbal Input | Inputs rotation data for radar in manual mode. Value 1: The yaw angle of the radar measured in turns, Value 2: The pitch angle of the radar measured in turns from -0.125 to 0.125. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| composite | Radar Data | Outputs data for up to 8 targets. On/Off 1-8 : Target 1 Found, Target 2 Found, etc... Values 1-32 : Target 1 Distance, Target 1 Azimuth Angle, Target 1 Elevation Angle, Target 1 Time Since Detection, Target 2 Distance, Target 2 Azimuth Angle, Target 2 Elevation Angle, Target 2 Time Since Detection, etc... |
| number | Radar Rotation | Current radar rotation from forward in turns. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Radar Detector

A sensor that can detect radar waves.

This sensor outputs an On signal when it detects a radio wave.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x2
- Cost: $1000
- Tags: 
- File: radar_detector.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Detected | Returns an On signal when it detects a radio wave. |

## Radiation Detector

A sensor to detect radiation.

Outputs radiation dose rate per second at its location.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $250
- Tags: geiger,radiation
- File: radiation_detector.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Radiation | The detected radiation dose rate. |

## Rain Sensor

A rain sensor for measuring the current meteorological conditions.

The reading can be read from the sensor's number output and is measured from 0 (no rain) to 1 (max rain).

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x2
- Cost: $180
- Tags: 
- File: rain_sensor.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Rain Factor | The amount of current rain fall from 0 to 1. |

## Sonar (Large)

A short range Sonar that returns information about a detected underwater object within its view.

This sensor outputs the distance and angle to a detected underwater object within its range and field of view using sound waves. (Range : 3000) (Max FOV : 0.125)

### PROPERTIES

- Mass: 25
- Dimensions (WxDxH): 7x7x2
- Cost: $1000
- Tags: 
- File: radar_sonar.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| number | FOV | The sensor's yaw field of view in turns from 0.01 to 0.125. |
| number | Facing Yaw | The sensor's yaw direction in turns from -0.5 to 0.5. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Target Distance | The distance to the target in meters. |
| number | Signal Strength | The strength of the returned signal. |
| number | Elevation Angle | The pitch angle between the sensor and the target in turns. |
| on/off | Target Found | Returns if an object has been detected. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Sonar (Large)

A sonar that returns information about a detected objects within 200km.

This sensor outputs the relative angle to detected objects within its range using underwater sound waves. The sensor will passively detect certain noisy components such as propellers or engines but can also send out a loud ping to detect quiet underwater bodies. While the ping input is held passive signals will be supressed. After activating a ping additional detected signals will appear momentarily in the data channel as the signal returns to the sonar. Activating another ping will override the previous ping and no further data will be returned from the old signal.

### PROPERTIES

- Mass: 200
- Dimensions (WxDxH): 7x7x5
- Cost: $4000
- Tags: 
- File: sonar_advanced_7.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Activate | Enable the Sonar. |
| on/off | Ping | Send a ping and listen for return sounds. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| composite | Sonar Data | Outputs data for up to 16 targets. On/Off 1-16 : Target 1 Found, Target 2 Found, Etc... Values 1-32: Target 1 Pivot, Target 1 Pitch, Target 2 Pivot, Target 2 Pitch, Etc... |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Sonar (Medium)

A sonar that returns information about a detected objects within 100km.

This sensor outputs the relative angle to detected objects within its range using underwater sound waves. The sensor will passively detect certain noisy components such as propellers or engines but can also send out a loud ping to detect quiet underwater bodies. While the ping input is held passive signals will be supressed. After activating a ping additional detected signals will appear momentarily in the data channel as the signal returns to the sonar. Activating another ping will override the previous ping and no further data will be returned from the old signal.

### PROPERTIES

- Mass: 50
- Dimensions (WxDxH): 5x5x3
- Cost: $2000
- Tags: 
- File: sonar_advanced_5.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Activate | Enable the Sonar. |
| on/off | Ping | Send a ping and listen for return sounds. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| composite | Sonar Data | Outputs data for up to 16 targets. On/Off 1-16 : Target 1 Found, Target 2 Found, Etc... Values 1-32: Target 1 Pivot, Target 1 Pitch, Target 2 Pivot, Target 2 Pitch, Etc... |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Sonar (Small)

A short range Sonar that returns information about a detected underwater object within its view.

This sensor outputs the distance and angle to a detected underwater object within its range and field of view using sound waves. (Range : 1000) (Max FOV : 0.125)

### PROPERTIES

- Mass: 10
- Dimensions (WxDxH): 3x3x1
- Cost: $1000
- Tags: 
- File: radar_sonar_small.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| number | FOV | The sensor's yaw field of view in turns from 0.01 to 0.125. |
| number | Facing Yaw | The sensor's yaw direction in turns from -0.5 to 0.5. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Target Distance | The distance to the target in meters. |
| number | Signal Strength | The strength of the returned signal. |
| number | Elevation Angle | The pitch angle between the sensor and the target in turns. |
| on/off | Target Found | Returns if an object has been detected. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Sonar (Small)

A sonar that returns information about a detected objects within 60km.

This sensor outputs the relative angle to detected objects within its range using underwater sound waves. The sensor will passively detect certain noisy components such as propellers or engines but can also send out a loud ping to detect quiet underwater bodies. While the ping input is held passive signals will be supressed. After activating a ping additional detected signals will appear momentarily in the data channel as the signal returns to the sonar. Activating another ping will override the previous ping and no further data will be returned from the old signal.

### PROPERTIES

- Mass: 10
- Dimensions (WxDxH): 3x3x1
- Cost: $1000
- Tags: 
- File: sonar_advanced.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Activate | Enable the Sonar. |
| on/off | Ping | Send a ping and listen for return sounds. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| composite | Sonar Data | Outputs data for up to 16 targets. On/Off 1-16 : Target 1 Found, Target 2 Found, Etc... Values 1-32: Target 1 Pivot, Target 1 Pitch, Target 2 Pivot, Target 2 Pitch, Etc... |
| composite | Torpedo Output | Outputs x and y data for the most immediate target. Link this directly into a rocket fins component. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Temperature Probe

A sensor to determine temperature.

A sensor that outputs the current temperature of an enclosed space in Celcius, if not within an enclosed volume it outputs the ambient air temperature at its location.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $250
- Tags: 
- File: temperature_probe.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Temperature | The detected temperature in degrees. |

## Tilt Sensor

A sensor that measures how much it has tilted, relative to the horizon.

The measurement is expressed in terms of turns, with an output range of -0.25 to 0.25 turns. A value of zero points towards the horizon.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $20
- Tags: 
- File: rotation_sensor.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Tilt | The measured tilt relative to the horizon. |

## Transponder Locator

An emergency search and rescue transponder locator.

Detects all transponder signals over great distances. Outputs the strongest signal strength detected, transponder signal strengths will decrease with distance.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x2
- Cost: $20
- Tags: basic,mission
- File: transponder_locator.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Active | Detects any transponder signals when active. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Transponder Pulse | Emits a periodic boolean pulse, with a frequency determined by the distance to the nearest transponder signal. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Wind Sensor

A wind sensor for measuring relative wind speed and direction.

The sensor outputs the wind direction relative to the orientation of the base of the sensor (in number of turns from -0.5 to 0.5) and the wind speed in m/s. Wind data is relative to the speed of the sensor and only measures wind in the plane of the sensor.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x2
- Cost: $200
- Tags: 
- File: wind_sensor.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Wind Speed | The relative wind velocity. |
| number | Wind Direction | The direction of the wind relative to the component. |

## Radar (Deprecated)

> [!WARNING]
> This component is deprecated.

A short range Radar that returns information about a detected object within its view.

This sensor outputs the distance and angle to a detected object within its range and field of view using radio waves. (Range : 5000) (Max FOV : 0.125)

### PROPERTIES

- Mass: 10
- Dimensions (WxDxH): 3x3x1
- Cost: $1000
- Tags: 
- File: radar.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| number | FOV | The sensor's yaw field of view in turns from 0.01 to 0.125. |
| number | Facing Yaw | The sensor's yaw direction in turns from -0.5 to 0.5. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Target Distance | The distance to the target in meters. |
| number | Signal Strength | The strength of the returned signal. |
| number | Elevation Angle | The pitch angle between the sensor and the target in turns. |
| on/off | Target Found | Returns if an object has been detected. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Radar (Dish) (Deprecated)

> [!WARNING]
> This component is deprecated.

A medium range, fixed rotation Radar that returns information about a detected object within its view.

This fixed sensor outputs the distance and angle to a detected object within its range and field of view using radio waves. (Range : 20000) (Max FOV : 0.125)

### PROPERTIES

- Mass: 150
- Dimensions (WxDxH): 21x11x10
- Cost: $3000
- Tags: 
- File: radar_dish.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| number | FOV | The sensor's yaw field of view in turns from 0.01 to 0.125. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Target Distance | The distance to the target in meters. |
| number | Signal Strength | The strength of the returned signal. |
| number | Elevation Angle | The pitch angle between the sensor and the target in turns. |
| on/off | Target Found | Returns if an object has been detected. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Radar (Huge) (Deprecated)

> [!WARNING]
> This component is deprecated.

A long range, multi-target Radar that returns detailed information through composite channels about detected objects within its view.

This sensor outputs the distance and relative angles to up to 8 detected objects within its range and field of view using radio waves and outputs all detected targets through composite channels. (Range : 50000) (Max FOV : 0.125)

### PROPERTIES

- Mass: 1100
- Dimensions (WxDxH): 37x37x5
- Cost: $10000
- Tags: 
- File: radar_huge.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| number | FOV | The sensor's yaw field of view in turns from 0.01 to 0.125. |
| number | Facing Yaw | The sensor's yaw direction in turns from -0.5 to 0.5. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| composite | Radar Data | Outputs data for up to 8 targets. On/Off 1-8 : Target 1 Found, Target 2 Found, etc... Values 1-32 : Target 1 Distance, Target 1 Azimuth Angle, Target 1 Elevation Angle, Target 1 Time Since Detection, Target 2 Distance, Target 2 Azimuth Angle, Target 2 Elevation Angle, Target 2 Time Since Detection, etc... |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Radar (Large) (Deprecated)

> [!WARNING]
> This component is deprecated.

A medium range, highly configurable Radar that returns detailed information about a detected object within its view.

This sensor outputs the distance and relative angles to a detected object within its range and field of view using radio waves. This sensor uniquely allows the changing of it's pitch direction. (Range : 20000) (Max FOV : 0.250)

### PROPERTIES

- Mass: 300
- Dimensions (WxDxH): 7x7x16
- Cost: $5000
- Tags: 
- File: radar_large.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| number | FOV | The sensor's yaw and pitch field of view in turns from 0.01 to 0.125. |
| number | Facing Yaw | The sensor's yaw direction in turns from -0.5 to 0.5. |
| number | Facing Pitch | The sensor's pitch direction in turns from -0.25 to 0.25. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Target Distance | The distance to the target in meters. |
| number | Signal Strength | The strength of the returned signal. |
| number | Elevation Angle | The pitch angle between the sensor and the target in turns. |
| number | Azimuth Angle | The yaw angle between the sensor and the target in turns. |
| on/off | Target Found | Returns if an object has been detected. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |
