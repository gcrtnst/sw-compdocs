# Vehicle Control

## Compact Pilot Seat

The compact pilot seat lets you translate keyboard presses into output signals that can control logic components.

It provides 4 number outputs that produce a standard value ranging from -1 to 1, and 6 on/off outputs. You can get in and out of the compact pilot seat by interacting with it using [f].

### PROPERTIES

- Mass: 7
- Dimensions (WxDxH): 3x3x5
- Cost: $100
- Tags: basic,seat,control,pilot
- File: seat_compact.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| audio | Headset Audio |  |
| video | Headset Video | Displays video UI overlay on a helmet mounted display. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Occupied | Outputs an on signal if this seat is occupied by a character. |
| on/off | Trigger [space] | Outputs an on signal when [space] is held, and off when it is not. |
| number | Look X | Outputs the character look direction in turns along the X-axis. |
| number | Look Y | Outputs the character look direction in turns along the Y-axis. |
| number | Axis 1 [a]/[d] | Outputs a standard value between -1 and 1, controlled using [a] and [d]. [a] causes the output value to move towards -1, and [d] moves it towards 1. |
| number | Axis 2 [w]/[s] | Outputs a standard value between -1 and 1, controlled using [w] and [s]. [s] causes the output value to move towards -1, and [w] moves it towards 1. |
| number | Axis 3 [left]/[right] | Outputs a standard value between -1 and 1, controlled using [left] and [right]. [left] causes the output value to move towards -1, and [right] moves it towards 1. |
| number | Axis 4 [up]/[down] | Outputs a standard value between -1 and 1, controlled using [up] and [down]. [down] causes the output value to move towards -1, and [up] moves it towards 1. |
| on/off | Hotkey 1 [1] | Outputs an on signal when [1] is held, and off when it is not. |
| on/off | Hotkey 2 [2] | Outputs an on signal when [2] is held, and off when it is not. |
| on/off | Hotkey 3 [3] | Outputs an on signal when [3] is held, and off when it is not. |
| on/off | Hotkey 4 [4] | Outputs an on signal when [4] is held, and off when it is not. |
| on/off | Hotkey 5 [5] | Outputs an on signal when [5] is held, and off when it is not. |
| on/off | Hotkey 6 [6] | Outputs an on signal when [6] is held, and off when it is not. |
| composite | Seat data | Outputs the axis, hotkey and occupied data from the seat. (On/Off 1+ : Hotkeys) (On/Off 31 : Trigger) (On/Off 32 : Occupied) (Value 1 : [a]/[d]) (Value 2 : [w]/[s]) (Value 3 : [left]/[right]) (Value 4 : [up]/[down]) (Value 9 : Look X)  (Value 10 : Look Y) |
| audio | Headset Audio |  |

## Control Fin Large

The fin can be attached to the surface of a vehicle to direct its motion.

It takes a number input between -1 and 1 that represent the two extremes of the fin's rotation.

### PROPERTIES

- Mass: 10
- Dimensions (WxDxH): 1x3x3
- Cost: $350
- Tags: boat,basic
- File: control_fin_large.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| number | Rotation | Accepts a value between -1 and 1 that represent the two extremes of the fin's rotation. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Control Fin Medium

The fin can be attached to the surface of a vehicle to direct its motion.

It takes a number input between -1 and 1 that represent the two extremes of the fin's rotation.

### PROPERTIES

- Mass: 5
- Dimensions (WxDxH): 1x3x2
- Cost: $150
- Tags: boat,basic
- File: control_fin_medium.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| number | Rotation | Accepts a value between -1 and 1 that represent the two extremes of the fin's rotation. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Control Fin Small

The fin can be attached to the surface of a vehicle to direct its motion.

It takes a number input between -1 and 1 that represent the two extremes of the fin's rotation.

### PROPERTIES

- Mass: 2
- Dimensions (WxDxH): 1x1x1
- Cost: $50
- Tags: boat,basic
- File: control_fin_small.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| number | Rotation | Accepts a value between -1 and 1 that represent the two extremes of the fin's rotation. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Control Handle

A compact control handle.

You can get in and out of the position by interacting with it using [f].

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 3x3x7
- Cost: $50
- Tags: basic,seat,control,pilot
- File: seat_handle.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| audio | Headset Audio |  |
| video | Headset Video | Displays video UI overlay on a helmet mounted display. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Occupied | Outputs an on signal if the handle is occupied by a character. |
| on/off | Trigger [space] | Outputs an on signal when [space] is held, and off when it is not. |
| number | Look X | Outputs the character look direction in turns along the X-axis. |
| number | Look Y | Outputs the character look direction in turns along the Y-axis. |
| number | Axis 1 [a]/[d] | Outputs a standard value between -1 and 1, controlled using [a] and [d]. [a] causes the output value to move towards -1, and [d] moves it towards 1. |
| number | Axis 2 [w]/[s] | Outputs a standard value between -1 and 1, controlled using [w] and [s]. [s] causes the output value to move towards -1, and [w] moves it towards 1. |
| number | Axis 3 [left]/[right] | Outputs a standard value between -1 and 1, controlled using [left] and [right]. [left] causes the output value to move towards -1, and [right] moves it towards 1. |
| number | Axis 4 [up]/[down] | Outputs a standard value between -1 and 1, controlled using [up] and [down]. [down] causes the output value to move towards -1, and [up] moves it towards 1. |
| on/off | Hotkey 1 [1] | Outputs an on signal when [1] is held, and off when it is not. |
| on/off | Hotkey 2 [2] | Outputs an on signal when [2] is held, and off when it is not. |
| on/off | Hotkey 3 [3] | Outputs an on signal when [3] is held, and off when it is not. |
| on/off | Hotkey 4 [4] | Outputs an on signal when [4] is held, and off when it is not. |
| on/off | Hotkey 5 [5] | Outputs an on signal when [5] is held, and off when it is not. |
| on/off | Hotkey 6 [6] | Outputs an on signal when [6] is held, and off when it is not. |
| composite | Seat data | Outputs the axis, hotkey and occupied data from the helm. (On/Off 1+ : Hotkeys) (On/Off 31 : Trigger) (On/Off 32 : Occupied) (Value 1 : [a]/[d]) (Value 2 : [w]/[s]) (Value 3 : [left]/[right]) (Value 4 : [up]/[down]) (Value 9 : Look X)  (Value 10 : Look Y) |
| audio | Headset Audio |  |

## Control Surface (Large)

The control surface can be attached to a surface of the vehicle to apply force as air or water is flowing over it.

It takes a number input between -1 and 1 that represent the two extremes of the fin's rotation.

### PROPERTIES

- Mass: 25
- Dimensions (WxDxH): 1x17x5
- Cost: $500
- Tags: airplane,aeroplane,basic
- File: control_surface_large.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| number | Rotation | Accepts a value between -1 and 1 that represent the two extremes of the rudder's rotation. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Control Surface (Medium)

The control surface can be attached to a surface of the vehicle to apply force as air or water is flowing over it.

It takes a number input between -1 and 1 that represent the two extremes of the fin's rotation.

### PROPERTIES

- Mass: 15
- Dimensions (WxDxH): 1x11x4
- Cost: $250
- Tags: airplane,aeroplane,basic
- File: control_surface_medium.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| number | Rotation | Accepts a value between -1 and 1 that represent the two extremes of the rudder's rotation. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Control Surface (Small)

The control surface can be attached to a surface of the vehicle to apply force as air or water is flowing over it.

It takes a number input between -1 and 1 that represent the two extremes of the fin's rotation.

### PROPERTIES

- Mass: 10
- Dimensions (WxDxH): 1x7x3
- Cost: $150
- Tags: airplane,aeroplane,basic
- File: control_surface_small.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| number | Rotation | Accepts a value between -1 and 1 that represent the two extremes of the rudder's rotation. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Driver seat

The driver seat lets you translate keyboard presses into output signals that can control logic components.

It provides 4 number outputs that produce a standard value ranging from -1 to 1, and 6 on/off outputs. You can get in and out of the driver seat by interacting with it using [f].

### PROPERTIES

- Mass: 10
- Dimensions (WxDxH): 3x4x5
- Cost: $100
- Tags: basic,seat,control,pilot
- File: seat_racing.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| audio | Headset Audio |  |
| video | Headset Video | Displays video UI overlay on a helmet mounted display. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Occupied | Outputs an on signal if this seat is occupied by a character. |
| on/off | Trigger [space] | Outputs an on signal when [space] is held, and off when it is not. |
| number | Look X | Outputs the character look direction in turns along the X-axis. |
| number | Look Y | Outputs the character look direction in turns along the Y-axis. |
| number | Axis 1 [a]/[d] | Outputs a standard value between -1 and 1, controlled using [a] and [d]. [a] causes the output value to move towards -1, and [d] moves it towards 1. |
| number | Axis 2 [w]/[s] | Outputs a standard value between -1 and 1, controlled using [w] and [s]. [s] causes the output value to move towards -1, and [w] moves it towards 1. |
| number | Axis 3 [left]/[right] | Outputs a standard value between -1 and 1, controlled using [left] and [right]. [left] causes the output value to move towards -1, and [right] moves it towards 1. |
| number | Axis 4 [up]/[down] | Outputs a standard value between -1 and 1, controlled using [up] and [down]. [down] causes the output value to move towards -1, and [up] moves it towards 1. |
| on/off | Hotkey 1 [1] | Outputs an on signal when [1] is held, and off when it is not. |
| on/off | Hotkey 2 [2] | Outputs an on signal when [2] is held, and off when it is not. |
| on/off | Hotkey 3 [3] | Outputs an on signal when [3] is held, and off when it is not. |
| on/off | Hotkey 4 [4] | Outputs an on signal when [4] is held, and off when it is not. |
| on/off | Hotkey 5 [5] | Outputs an on signal when [5] is held, and off when it is not. |
| on/off | Hotkey 6 [6] | Outputs an on signal when [6] is held, and off when it is not. |
| composite | Seat data | Outputs the axis, hotkey and occupied data from the seat. (On/Off 1+ : Hotkeys) (On/Off 31 : Trigger) (On/Off 32 : Occupied) (Value 1 : [a]/[d]) (Value 2 : [w]/[s]) (Value 3 : [left]/[right]) (Value 4 : [up]/[down]) (Value 9 : Look X)  (Value 10 : Look Y) |
| audio | Headset Audio |  |

## Fin Rudder

The fin rudder can be attached to the keel of a boat to control its yaw, allowing you to steer left and right.

It takes a number input between -1 and 1 that represent the two extremes of the fin's rotation.

### PROPERTIES

- Mass: 5
- Dimensions (WxDxH): 1x3x2
- Cost: $100
- Tags: boat,basic
- File: rudder_surface.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| number | Rotation | Accepts a value between -1 and 1 that represent the two extremes of the rudder's rotation. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Friction Pad

Friction pad that grips to surfaces.

High friction pad that grips any surface it touches.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $15
- Tags: 
- File: friction_block.xml

## Gyro

The gyroscope takes 4 standard value signals representing the desired yaw, pitch, roll and vertical motion of a helicopter.

It outputs stabilised values that can be sent to rotors and engines to make them much easier to control. An on/off input allows you to activate and deactivate the internal auto-hover circuit. When auto-hover is enabled, the gyroscope will attempt to keep your helicopter steady.

### PROPERTIES

- Mass: 10
- Dimensions (WxDxH): 5x3x1
- Cost: $500
- Tags: helicopter
- File: gyro.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| number | Roll | Accepts a standard value between -1 and 1 representing the desired roll speed. |
| number | Pitch | Accepts a standard value between -1 and 1 representing the desired pitch speed. |
| number | Yaw | Accepts a standard value between -1 and 1 representing the desired yaw speed. |
| number | Up/Down | Accepts a standard value between -1 and 1 representing the desired vertical speed. |
| on/off | Auto-hover | Enables the gyroscope's auto-hover circuit when receiving an on signal. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Stabilised Roll | Outputs a standard value between -1 and 1 representing a stabilised roll speed. |
| number | Stabilised Pitch | Outputs a standard value between -1 and 1 representing a stabilised pitch speed. |
| number | Stabilised Yaw | Outputs a standard value between -1 and 1 representing a stabilised yaw speed. |
| number | Stabilised Up/Down | Outputs a standard value between 0 and 1 representing a stabilised upward thrust. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Helm

A steering helm with steering wheel.

You can get in and out of the position by interacting with it using [f]. You can place a rescued survivor in any position by using [f] while carrying them.

### PROPERTIES

- Mass: 15
- Dimensions (WxDxH): 3x5x7
- Cost: $150
- Tags: basic,seat,control,pilot
- File: seat_helm.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| audio | Headset Audio |  |
| video | Headset Video | Displays video UI overlay on a helmet mounted display. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Occupied | Outputs an on signal if the helm is occupied by a character. |
| on/off | Trigger [space] | Outputs an on signal when [space] is held, and off when it is not. |
| number | Look X | Outputs the character look direction in turns along the X-axis. |
| number | Look Y | Outputs the character look direction in turns along the Y-axis. |
| number | Axis 1 [a]/[d] | Outputs a standard value between -1 and 1, controlled using [a] and [d]. [a] causes the output value to move towards -1, and [d] moves it towards 1. |
| number | Axis 2 [w]/[s] | Outputs a standard value between -1 and 1, controlled using [w] and [s]. [s] causes the output value to move towards -1, and [w] moves it towards 1. |
| number | Axis 3 [left]/[right] | Outputs a standard value between -1 and 1, controlled using [left] and [right]. [left] causes the output value to move towards -1, and [right] moves it towards 1. |
| number | Axis 4 [up]/[down] | Outputs a standard value between -1 and 1, controlled using [up] and [down]. [down] causes the output value to move towards -1, and [up] moves it towards 1. |
| on/off | Hotkey 1 [1] | Outputs an on signal when [1] is held, and off when it is not. |
| on/off | Hotkey 2 [2] | Outputs an on signal when [2] is held, and off when it is not. |
| on/off | Hotkey 3 [3] | Outputs an on signal when [3] is held, and off when it is not. |
| on/off | Hotkey 4 [4] | Outputs an on signal when [4] is held, and off when it is not. |
| on/off | Hotkey 5 [5] | Outputs an on signal when [5] is held, and off when it is not. |
| on/off | Hotkey 6 [6] | Outputs an on signal when [6] is held, and off when it is not. |
| composite | Seat data | Outputs the axis, hotkey and occupied data from the helm. (On/Off 1+ : Hotkeys) (On/Off 31 : Trigger) (On/Off 32 : Occupied) (Value 1 : [a]/[d]) (Value 2 : [w]/[s]) (Value 3 : [left]/[right]) (Value 4 : [up]/[down]) (Value 9 : Look X)  (Value 10 : Look Y) |
| audio | Headset Audio |  |

## Keel (Large)

A large boat keel used for sailing.

The keel resists rolling forces while submerged, helping to keep a boat upright and stable. The keel also resists lateral sliding forces, causing the majority of a boats movement to be in the direction of the keel axis. When combined with the force provided by a sail, this allows a sailboat to move forward in a crosswind, or even upwind.

### PROPERTIES

- Mass: 2000
- Dimensions (WxDxH): 3x25x9
- Cost: $2000
- Tags: boat,basic
- File: keel_large.xml

## Keel (Medium)

A medium boat keel used for sailing.

The keel resists rolling forces while submerged, helping to keep a boat upright and stable. The keel also resists lateral sliding forces, causing the majority of a boats movement to be in the direction of the keel axis. When combined with the force provided by a sail, this allows a sailboat to move forward in a crosswind, or even upwind.

### PROPERTIES

- Mass: 1000
- Dimensions (WxDxH): 3x15x7
- Cost: $1000
- Tags: boat,basic
- File: keel_medium.xml

## Keel (Small)

A small boat keel used for sailing.

The keel resists rolling forces while submerged, helping to keep a boat upright and stable. The keel also resists lateral sliding forces, causing the majority of a boats movement to be in the direction of the keel axis. When combined with the force provided by a sail, this allows a sailboat to move forward in a crosswind, or even upwind.

### PROPERTIES

- Mass: 500
- Dimensions (WxDxH): 1x9x5
- Cost: $300
- Tags: boat,basic
- File: keel_small.xml

## Keep Active Block

A keep alive marking block.

When on a vehicle, the vehicle will not despawn when out of range.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $100
- Tags: no_sleep
- File: no_sleep.xml

## Large Landing Wheel

Large landing wheel that requires no engine power and spins freely.

You cannot control the forward and backward rotation of this wheel, but it can be locked into place by sending an on signal to the brake input.

### PROPERTIES

- Mass: 8
- Dimensions (WxDxH): 3x3x4
- Cost: $50
- Tags: basic
- File: wheel_coaster_large.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Brake | Locks the wheel into place when receiving an on signal. |
| number | Variable Brake | A value between 0 and 1 for soft braking |

## Map Icon Block

A vehicle tracking block.

When on a vehicle, the vehicle will show on the map and other vehicles in the group will be hidden. The custom name set here will be the name set on the map.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $100
- Tags: 
- File: map_icon.xml

## Medium Wheel

Medium wheel that can be controlled using an engine.

The wheel will rotate forwards and backwards depending on power received from a connected engine. It can be rotated left and right by sending a number signal to the steering input. It can also be locked into place by sending an on signal to the brake input.

### PROPERTIES

- Mass: 10
- Dimensions (WxDxH): 7x7x5
- Cost: $100
- Tags: steerable,steering,basic
- File: wheel_medium.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Brake | Locks the wheel into place when receiving an on signal. |
| number | Variable Brake | A value between 0 and 1 for soft braking |
| number | Steering | Accepts a value between -1 and 1 that represents the extremes of the wheels steering rotation |

### connections

| Type | Label | Description |
| --- | --- | --- |
| power | RPS | Receives power generated by an engine to control forward and backward rotation. |

## Pilot Seat

The pilot seat lets you translate keyboard presses into output signals that can control logic components.

It provides 4 number outputs that produce a standard value ranging from -1 to 1, and 6 on/off outputs. You can get in and out of the pilot seat by interacting with it using [f].

### PROPERTIES

- Mass: 24
- Dimensions (WxDxH): 3x4x6
- Cost: $100
- Tags: basic,seat,control,pilot
- File: seat.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| audio | Headset Audio |  |
| video | Headset Video | Displays video UI overlay on a helmet mounted display. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Occupied | Outputs an on signal if this seat is occupied by a character. |
| on/off | Trigger [space] | Outputs an on signal when [space] is held, and off when it is not. |
| number | Look X | Outputs the character look direction in turns along the X-axis. |
| number | Look Y | Outputs the character look direction in turns along the Y-axis. |
| number | Axis 1 [a]/[d] | Outputs a standard value between -1 and 1, controlled using [a] and [d]. [a] causes the output value to move towards -1, and [d] moves it towards 1. |
| number | Axis 2 [w]/[s] | Outputs a standard value between -1 and 1, controlled using [w] and [s]. [s] causes the output value to move towards -1, and [w] moves it towards 1. |
| number | Axis 3 [left]/[right] | Outputs a standard value between -1 and 1, controlled using [left] and [right]. [left] causes the output value to move towards -1, and [right] moves it towards 1. |
| number | Axis 4 [up]/[down] | Outputs a standard value between -1 and 1, controlled using [up] and [down]. [down] causes the output value to move towards -1, and [up] moves it towards 1. |
| on/off | Hotkey 1 [1] | Outputs an on signal when [1] is held, and off when it is not. |
| on/off | Hotkey 2 [2] | Outputs an on signal when [2] is held, and off when it is not. |
| on/off | Hotkey 3 [3] | Outputs an on signal when [3] is held, and off when it is not. |
| on/off | Hotkey 4 [4] | Outputs an on signal when [4] is held, and off when it is not. |
| on/off | Hotkey 5 [5] | Outputs an on signal when [5] is held, and off when it is not. |
| on/off | Hotkey 6 [6] | Outputs an on signal when [6] is held, and off when it is not. |
| composite | Seat data | Outputs the axis, hotkey and occupied data from the seat. (On/Off 1+ : Hotkeys) (On/Off 31 : Trigger) (On/Off 32 : Occupied) (Value 1 : [a]/[d]) (Value 2 : [w]/[s]) (Value 3 : [left]/[right]) (Value 4 : [up]/[down]) (Value 9 : Look X)  (Value 10 : Look Y) |
| audio | Headset Audio |  |

## Pilot Seat (HOTAS)

The pilot seat lets you translate controller presses into output signals that can control logic components.

It provides 10 number outputs that produce a standard value ranging from -1 to 1, and 48 on/off outputs. You can get in and out of the pilot seat by interacting with it using [f]. Designed for use with HOTAS controllers.

### PROPERTIES

- Mass: 50
- Dimensions (WxDxH): 3x5x6
- Cost: $250
- Tags: basic,seat,control,pilot
- File: seat_hotas.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| audio | Headset Audio |  |
| video | Headset Video | Displays video UI overlay on a helmet mounted display. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Occupied | Outputs an on signal if this seat is occupied by a character. |
| on/off | Trigger [space] | Outputs an on signal when [space] is held, and off when it is not. |
| number | Look X | Outputs the character look direction in turns along the X-axis. |
| number | Look Y | Outputs the character look direction in turns along the Y-axis. |
| number | Axis 1 [a]/[d] | Outputs a standard value between -1 and 1, controlled using [a] and [d]. [a] causes the output value to move towards -1, and [d] moves it towards 1. |
| number | Axis 2 [w]/[s] | Outputs a standard value between -1 and 1, controlled using [w] and [s]. [s] causes the output value to move towards -1, and [w] moves it towards 1. |
| number | Axis 3 [left]/[right] | Outputs a standard value between -1 and 1, controlled using [left] and [right]. [left] causes the output value to move towards -1, and [right] moves it towards 1. |
| number | Axis 4 [up]/[down] | Outputs a standard value between -1 and 1, controlled using [up] and [down]. [down] causes the output value to move towards -1, and [up] moves it towards 1. |
| number | Axis 5 | Outputs a standard value between -1 and 1, controlled using the controller axis. |
| number | Axis 6 | Outputs a standard value between -1 and 1, controlled using the controller axis. |
| number | Axis 7 | Outputs a standard value between -1 and 1, controlled using the controller axis. |
| number | Axis 8 | Outputs a standard value between -1 and 1, controlled using the controller axis. |
| on/off | Hotkey 1 [1] | Outputs an on signal when [1] is held, and off when it is not. |
| on/off | Hotkey 2 [2] | Outputs an on signal when [2] is held, and off when it is not. |
| on/off | Hotkey 3 [3] | Outputs an on signal when [3] is held, and off when it is not. |
| on/off | Hotkey 4 [4] | Outputs an on signal when [4] is held, and off when it is not. |
| on/off | Hotkey 5 [5] | Outputs an on signal when [5] is held, and off when it is not. |
| on/off | Hotkey 6 [6] | Outputs an on signal when [6] is held, and off when it is not. |
| on/off | Hotkey 7 | Outputs an on signal when the controller button is held, and off when it is not. |
| on/off | Hotkey 8 | Outputs an on signal when the controller button is held, and off when it is not. |
| on/off | Hotkey 9 | Outputs an on signal when the controller button is held, and off when it is not. |
| on/off | Hotkey 10 | Outputs an on signal when the controller button is held, and off when it is not. |
| on/off | Hotkey 11 | Outputs an on signal when the controller button is held, and off when it is not. |
| on/off | Hotkey 12 | Outputs an on signal when the controller button is held, and off when it is not. |
| on/off | Hotkey 13 | Outputs an on signal when the controller button is held, and off when it is not. |
| on/off | Hotkey 14 | Outputs an on signal when the controller button is held, and off when it is not. |
| on/off | Hotkey 15 | Outputs an on signal when the controller button is held, and off when it is not. |
| on/off | Hotkey 16 | Outputs an on signal when the controller button is held, and off when it is not. |
| on/off | Hotkey 17 | Outputs an on signal when the controller button is held, and off when it is not. |
| on/off | Hotkey 18 | Outputs an on signal when the controller button is held, and off when it is not. |
| on/off | Hotkey 19 | Outputs an on signal when the controller button is held, and off when it is not. |
| on/off | Hotkey 20 | Outputs an on signal when the controller button is held, and off when it is not. |
| on/off | Hotkey 21 | Outputs an on signal when the controller button is held, and off when it is not. |
| on/off | Hotkey 22 | Outputs an on signal when the controller button is held, and off when it is not. |
| on/off | Hotkey 23 | Outputs an on signal when the controller button is held, and off when it is not. |
| on/off | Hotkey 24 | Outputs an on signal when the controller button is held, and off when it is not. |
| on/off | Hotkey 25 | Outputs an on signal when the controller button is held, and off when it is not. |
| on/off | Hotkey 26 | Outputs an on signal when the controller button is held, and off when it is not. |
| on/off | Hotkey 27 | Outputs an on signal when the controller button is held, and off when it is not. |
| on/off | Hotkey 28 | Outputs an on signal when the controller button is held, and off when it is not. |
| on/off | Hotkey 29 | Outputs an on signal when the controller button is held, and off when it is not. |
| on/off | Hotkey 30 | Outputs an on signal when the controller button is held, and off when it is not. |
| on/off | Hotkey 31 | Outputs an on signal when the controller button is held, and off when it is not. |
| on/off | Hotkey 32 | Outputs an on signal when the controller button is held, and off when it is not. |
| on/off | Hotkey 33 | Outputs an on signal when the controller button is held, and off when it is not. |
| on/off | Hotkey 34 | Outputs an on signal when the controller button is held, and off when it is not. |
| on/off | Hotkey 35 | Outputs an on signal when the controller button is held, and off when it is not. |
| on/off | Hotkey 36 | Outputs an on signal when the controller button is held, and off when it is not. |
| on/off | Hotkey 37 | Outputs an on signal when the controller button is held, and off when it is not. |
| on/off | Hotkey 38 | Outputs an on signal when the controller button is held, and off when it is not. |
| on/off | Hotkey 39 | Outputs an on signal when the controller button is held, and off when it is not. |
| on/off | Hotkey 40 | Outputs an on signal when the controller button is held, and off when it is not. |
| on/off | Hotkey 41 | Outputs an on signal when the controller button is held, and off when it is not. |
| on/off | Hotkey 42 | Outputs an on signal when the controller button is held, and off when it is not. |
| on/off | Hotkey 43 | Outputs an on signal when the controller button is held, and off when it is not. |
| on/off | Hotkey 44 | Outputs an on signal when the controller button is held, and off when it is not. |
| on/off | Hotkey 45 | Outputs an on signal when the controller button is held, and off when it is not. |
| on/off | Hotkey 46 | Outputs an on signal when the controller button is held, and off when it is not. |
| on/off | Hotkey 47 | Outputs an on signal when the controller button is held, and off when it is not. |
| on/off | Hotkey 48 | Outputs an on signal when the controller button is held, and off when it is not. |
| composite | Seat data | Outputs the axis, hotkey and occupied data from the seat. (On/Off 1+ : Hotkeys) (On/Off 31 : Trigger) (On/Off 32 : Occupied) (Value 1 : [a]/[d]) (Value 2 : [w]/[s]) (Value 3 : [left]/[right]) (Value 4 : [up]/[down]) (Values 5/6/7/8 : Controller Axes) (Value 9 : Look X)  (Value 10 : Look Y) |
| audio | Headset Audio |  |

## Radio RX Huge

A radio data transmitter and receiver.

Sends and receives data on the specified frequency. Transmit Mode defaults to receive. (Max effective range at ground level : 20km)

### PROPERTIES

- Mass: 20
- Dimensions (WxDxH): 1x1x9
- Cost: $3000
- Tags: 
- File: rx_huge_v2.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| audio | Audio Send | Input for audio data to send. |
| composite | Data Send | Input for composite data to send. |
| number | Frequency | Radio Send/Receive Frequency. |
| on/off | Transmit Mode | Whether the radio is transmitting or receiving. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| audio | Audio Recv | Output for received audio data. |
| composite | Data Recv | Output for received composite data. |
| number | Signal Strength | Strength of connection signal. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical input. |

## Radio RX Large

A radio data transmitter and receiver.

Sends and receives data on the specified frequency. Transmit Mode defaults to receive. (Max effective range at ground level : 4km)

### PROPERTIES

- Mass: 12
- Dimensions (WxDxH): 1x1x5
- Cost: $1000
- Tags: 
- File: rx_large_v2.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| audio | Audio Send | Input for audio data to send. |
| composite | Data Send | Input for composite data to send. |
| number | Frequency | Radio Send/Receive Frequency. |
| on/off | Transmit Mode | Whether the radio is transmitting or receiving. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| audio | Audio Recv | Output for received audio data. |
| composite | Data Recv | Output for received composite data. |
| number | Signal Strength | Strength of connection signal. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical input. |

## Radio RX Medium

A radio data transmitter and receiver.

Sends and receives data on the specified frequency. Transmit Mode defaults to receive. (Max effective range at ground level : 1km)

### PROPERTIES

- Mass: 8
- Dimensions (WxDxH): 1x1x4
- Cost: $500
- Tags: 
- File: rx_med_v2.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| audio | Audio Send | Input for audio data to send. |
| composite | Data Send | Input for composite data to send. |
| number | Frequency | Radio Send/Receive Frequency. |
| on/off | Transmit Mode | Whether the radio is transmitting or receiving. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| audio | Audio Recv | Output for received audio data. |
| composite | Data Recv | Output for received composite data. |
| number | Signal Strength | Strength of connection signal. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical input. |

## Radio RX Small

A radio data transmitter and receiver.

Sends and receives data on the specified frequency. Transmit Mode defaults to receive. (Max effective range at ground level : 100m)

### PROPERTIES

- Mass: 5
- Dimensions (WxDxH): 1x1x2
- Cost: $200
- Tags: 
- File: rx_small_v2.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| audio | Audio Send | Input for audio data to send. |
| composite | Data Send | Input for composite data to send. |
| number | Frequency | Radio Send/Receive Frequency. |
| on/off | Transmit Mode | Whether the radio is transmitting or receiving. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| audio | Audio Recv | Output for received audio data. |
| composite | Data Recv | Output for received composite data. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical input. |

## Radio Video Recv

A radio receiver for receiving video signals.

Receives a video signal on the frequency specified.

### PROPERTIES

- Mass: 10
- Dimensions (WxDxH): 1x1x4
- Cost: $1000
- Tags: 
- File: rx_video_r.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| number | Frequency Recv |  |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| video | Video Recv |  |
| number | Signal Strength |  |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric |  |

## Radio Video Xmit

A radio transmitter for sending video signals.

Sends a video signal on the frequency specified. (Max Effective Range : 10000m)

### PROPERTIES

- Mass: 10
- Dimensions (WxDxH): 1x1x4
- Cost: $2000
- Tags: 
- File: rx_video_x.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| video | Video Send |  |
| number | Frequency Send |  |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric |  |

## Rudder

The rudder can be attached to the underside of a boat to control its yaw, allowing you to steer left and right.

It takes a number input between -1 and 1 that represent the two extremes of the rudder's rotation.

### PROPERTIES

- Mass: 10
- Dimensions (WxDxH): 3x3x4
- Cost: $150
- Tags: boat,basic
- File: rudder.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| number | Rotation | Accepts a value between -1 and 1 that represent the two extremes of the rudder's rotation. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## RX Directional

A powerful directional radio and video data transmitter and receiver.

Must be pointed at the target RX device. Sends and receives data on the specified frequency. Transmit Mode defaults to receive. (Max effective range at ground level : 8000km)

### PROPERTIES

- Mass: 20
- Dimensions (WxDxH): 5x5x4
- Cost: $5000
- Tags: 
- File: rx_directional.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| audio | Audio Send | Input for audio data to send. |
| composite | Data Send | Input for composite data to send. |
| number | Frequency | Radio Send/Receive Frequency. |
| on/off | Transmit Mode | Whether the radio is transmitting or receiving. |
| number | Target Pitch | Target dish pitch in turns. Max 0.1 |
| number | Target Yaw | Target dish yaw in turns. |
| video | Video Send | Input for video data to send. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| audio | Audio Recv | Output for received audio data. |
| composite | Data Recv | Output for received composite data. |
| number | Signal Strength | Strength of connection signal. |
| video | Video Recv | Output for recieved video data. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical input. |

## RX Directional (Large)

A powerful directional radio and video data transmitter and receiver.

Must be pointed at the target RX device. Sends and receives data on the specified frequency. Transmit Mode defaults to receive. (Max effective range at ground level : 10000km)

### PROPERTIES

- Mass: 35
- Dimensions (WxDxH): 9x9x6
- Cost: $8000
- Tags: 
- File: rx_directional_large.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| audio | Audio Send | Input for audio data to send. |
| composite | Data Send | Input for composite data to send. |
| number | Frequency | Radio Send/Receive Frequency. |
| on/off | Transmit Mode | Whether the radio is transmitting or receiving. |
| number | Target Pitch | Target dish pitch in turns. Max 0.1 |
| number | Target Yaw | Target dish yaw in turns. |
| video | Video Send | Input for video data to send. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| audio | Audio Recv | Output for received audio data. |
| composite | Data Recv | Output for received composite data. |
| number | Signal Strength | Strength of connection signal. |
| video | Video Recv | Output for recieved video data. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical input. |

## Saddle Seat

A small padded seat with control handlebars.

You can get in and out of the seat by interacting with it using [f]. You can place a rescued survivor in any seat by using [f] while carrying them.

### PROPERTIES

- Mass: 5
- Dimensions (WxDxH): 3x4x4
- Cost: $75
- Tags: basic,seat
- File: seat_saddle.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| audio | Headset Audio |  |
| video | Headset Video | Displays video UI overlay on a helmet mounted display. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Occupied | Outputs an on signal if the seat is occupied by a character. |
| on/off | Trigger [space] | Outputs an on signal when [space] is held, and off when it is not. |
| number | Look X | Outputs the character look direction in turns along the X-axis. |
| number | Look Y | Outputs the character look direction in turns along the Y-axis. |
| number | Axis 1 [a]/[d] | Outputs a standard value between -1 and 1, controlled using [a] and [d]. [a] causes the output value to move towards -1, and [d] moves it towards 1. |
| number | Axis 2 [w]/[s] | Outputs a standard value between -1 and 1, controlled using [w] and [s]. [s] causes the output value to move towards -1, and [w] moves it towards 1. |
| number | Axis 3 [left]/[right] | Outputs a standard value between -1 and 1, controlled using [left] and [right]. [left] causes the output value to move towards -1, and [right] moves it towards 1. |
| number | Axis 4 [up]/[down] | Outputs a standard value between -1 and 1, controlled using [up] and [down]. [down] causes the output value to move towards -1, and [up] moves it towards 1. |
| on/off | Hotkey 1 [1] | Outputs an on signal when [1] is held, and off when it is not. |
| on/off | Hotkey 2 [2] | Outputs an on signal when [2] is held, and off when it is not. |
| on/off | Hotkey 3 [3] | Outputs an on signal when [3] is held, and off when it is not. |
| on/off | Hotkey 4 [4] | Outputs an on signal when [4] is held, and off when it is not. |
| on/off | Hotkey 5 [5] | Outputs an on signal when [5] is held, and off when it is not. |
| on/off | Hotkey 6 [6] | Outputs an on signal when [6] is held, and off when it is not. |
| composite | Seat data | Outputs the axis, hotkey and occupied data from the seat. (On/Off 1+ : Hotkeys) (On/Off 31 : Trigger) (On/Off 32 : Occupied) (Value 1 : [a]/[d]) (Value 2 : [w]/[s]) (Value 3 : [left]/[right]) (Value 4 : [up]/[down]) (Value 9 : Look X)  (Value 10 : Look Y) |
| audio | Headset Audio |  |

## Ski

A wide hinged ski.

This component has low friction moving along its length, but grips laterally.

### PROPERTIES

- Mass: 12
- Dimensions (WxDxH): 3x13x2
- Cost: $200
- Tags: 
- File: ski.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| number | Steering | Accepts a value between -1 and 1 that represents the extremes of the steering rotation. |

## Ski (Small)

A small hinged ski.

This component has low friction moving along its length, but grips laterally.

### PROPERTIES

- Mass: 8
- Dimensions (WxDxH): 1x9x2
- Cost: $100
- Tags: 
- File: ski_small.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| number | Steering | Accepts a value between -1 and 1 that represents the extremes of the steering rotation. |

## Small Wheel

Small wheel that can be controlled using an engine.

The wheel will rotate forwards and backwards depending on power received from a connected engine. It can be rotated left and right by sending a number signal to the steering input. It can also be locked into place by sending an on signal to the brake input.

### PROPERTIES

- Mass: 5
- Dimensions (WxDxH): 3x3x4
- Cost: $30
- Tags: steerable,steering,basic
- File: wheel_small.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Brake | Locks the wheel into place when receiving an on signal. |
| number | Variable Brake | A value between 0 and 1 for soft braking |
| number | Steering | Accepts a value between -1 and 1 that represents the extremes of the wheels steering rotation |

### connections

| Type | Label | Description |
| --- | --- | --- |
| power | RPS | Receives power generated by an engine to control forward and backward rotation. |

## Space Seat

The space seat lets you translate keyboard presses into output signals that can control logic components.

It provides 4 number outputs that produce a standard value ranging from -1 to 1, and 6 on/off outputs. You can get in and out of the space seat by interacting with it using [f].

### PROPERTIES

- Mass: 3
- Dimensions (WxDxH): 3x3x7
- Cost: $500
- Tags: basic,seat,control,pilot
- File: seat_space.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| audio | Headset Audio |  |
| video | Headset Video | Displays video UI overlay on a helmet mounted display. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Occupied | Outputs an on signal if the handle is occupied by a character. |
| on/off | Trigger [space] | Outputs an on signal when [space] is held, and off when it is not. |
| number | Look X | Outputs the character look direction in turns along the X-axis. |
| number | Look Y | Outputs the character look direction in turns along the Y-axis. |
| number | Axis 1 [a]/[d] | Outputs a standard value between -1 and 1, controlled using [a] and [d]. [a] causes the output value to move towards -1, and [d] moves it towards 1. |
| number | Axis 2 [w]/[s] | Outputs a standard value between -1 and 1, controlled using [w] and [s]. [s] causes the output value to move towards -1, and [w] moves it towards 1. |
| number | Axis 3 [left]/[right] | Outputs a standard value between -1 and 1, controlled using [left] and [right]. [left] causes the output value to move towards -1, and [right] moves it towards 1. |
| number | Axis 4 [up]/[down] | Outputs a standard value between -1 and 1, controlled using [up] and [down]. [down] causes the output value to move towards -1, and [up] moves it towards 1. |
| on/off | Hotkey 1 [1] | Outputs an on signal when [1] is held, and off when it is not. |
| on/off | Hotkey 2 [2] | Outputs an on signal when [2] is held, and off when it is not. |
| on/off | Hotkey 3 [3] | Outputs an on signal when [3] is held, and off when it is not. |
| on/off | Hotkey 4 [4] | Outputs an on signal when [4] is held, and off when it is not. |
| on/off | Hotkey 5 [5] | Outputs an on signal when [5] is held, and off when it is not. |
| on/off | Hotkey 6 [6] | Outputs an on signal when [6] is held, and off when it is not. |
| composite | Seat data | Outputs the axis, hotkey and occupied data from the helm. (On/Off 1+ : Hotkeys) (On/Off 31 : Trigger) (On/Off 32 : Occupied) (Value 1 : [a]/[d]) (Value 2 : [w]/[s]) (Value 3 : [left]/[right]) (Value 4 : [up]/[down]) (Value 9 : Look X)  (Value 10 : Look Y) |
| audio | Headset Audio |  |

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Fluid In |  |

## Tank Drive Wheel (Huge)

Huge drive wheel for tracked vehicles.

The wheel will form a track with other wheels of the same size and orientation that are placed in line and on the same body.

### PROPERTIES

- Mass: 80
- Dimensions (WxDxH): 7x7x5
- Cost: $450
- Tags: steerable,steering
- File: wheel_tank_drive_7.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Brake | Locks the wheel into place when receiving an on signal. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| power | RPS | Receives power generated by an engine to control forward and backward rotation. |

## Tank Drive Wheel (Large)

Large drive wheel for tracked vehicles.

The wheel will form a track with other wheels of the same size and orientation that are placed in line and on the same body.

### PROPERTIES

- Mass: 40
- Dimensions (WxDxH): 5x5x3
- Cost: $350
- Tags: steerable,steering
- File: wheel_tank_drive_5.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Brake | Locks the wheel into place when receiving an on signal. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| power | RPS | Receives power generated by an engine to control forward and backward rotation. |

## Tank Drive Wheel (Medium)

Medium drive wheel for tracked vehicles.

The wheel will form a track with other wheels of the same size and orientation that are placed in line and on the same body.

### PROPERTIES

- Mass: 30
- Dimensions (WxDxH): 5x5x3
- Cost: $300
- Tags: steerable,steering
- File: wheel_tank_drive_5_2.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Brake | Locks the wheel into place when receiving an on signal. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| power | RPS | Receives power generated by an engine to control forward and backward rotation. |

## Tank Drive Wheel (Small)

Small drive wheel for tracked vehicles.

The wheel will form a track with other wheels of the same size and orientation that are placed in line and on the same body.

### PROPERTIES

- Mass: 20
- Dimensions (WxDxH): 3x3x2
- Cost: $200
- Tags: steerable,steering
- File: wheel_tank_drive_1.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Brake | Locks the wheel into place when receiving an on signal. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| power | RPS | Receives power generated by an engine to control forward and backward rotation. |

## Tank Drive Wheel (Small/Wide)

Widened small drive wheel for tracked vehicles.

The wheel will form a track with other wheels of the same size and orientation that are placed in line and on the same body.

### PROPERTIES

- Mass: 35
- Dimensions (WxDxH): 3x3x3
- Cost: $250
- Tags: steerable,steering
- File: wheel_tank_drive_1_wide.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Brake | Locks the wheel into place when receiving an on signal. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| power | RPS | Receives power generated by an engine to control forward and backward rotation. |

## Tank Wheel (Huge)

Huge wheel for tracked vehicles.

A drive wheel is required to rotate the connected track. The wheel will form a track with other wheels of the same size and orientation that are placed in line and on the same body.

### PROPERTIES

- Mass: 80
- Dimensions (WxDxH): 7x7x5
- Cost: $350
- Tags: steerable,steering
- File: wheel_tank_7.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Brake | Locks the wheel into place when receiving an on signal. |

## Tank Wheel (Large)

Large wheel for tracked vehicles.

A drive wheel is required to rotate the connected track. The wheel will form a track with other wheels of the same size and orientation that are placed in line and on the same body.

### PROPERTIES

- Mass: 40
- Dimensions (WxDxH): 5x5x3
- Cost: $250
- Tags: steerable,steering
- File: wheel_tank_5.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Brake | Locks the wheel into place when receiving an on signal. |

## Tank Wheel (Medium)

Medium wheel for tracked vehicles.

A drive wheel is required to rotate the connected track. The wheel will form a track with other wheels of the same size and orientation that are placed in line and on the same body.

### PROPERTIES

- Mass: 30
- Dimensions (WxDxH): 5x5x3
- Cost: $200
- Tags: steerable,steering
- File: wheel_tank_5_2.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Brake | Locks the wheel into place when receiving an on signal. |

## Tank Wheel (Small)

Small wheel for tracked vehicles.

A drive wheel is required to rotate the connected track. The wheel will form a track with other wheels of the same size and orientation that are placed in line and on the same body.

### PROPERTIES

- Mass: 20
- Dimensions (WxDxH): 3x3x2
- Cost: $100
- Tags: steerable,steering
- File: wheel_tank_1.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Brake | Locks the wheel into place when receiving an on signal. |

## Tank Wheel (Small/Wide)

Widened small wheel for tracked vehicles.

A drive wheel is required to rotate the connected track. The wheel will form a track with other wheels of the same size and orientation that are placed in line and on the same body.

### PROPERTIES

- Mass: 20
- Dimensions (WxDxH): 3x3x3
- Cost: $100
- Tags: steerable,steering
- File: wheel_tank_1_wide.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Brake | Locks the wheel into place when receiving an on signal. |

## Wheel 3x3

Small steerable wheel with power connection and braking.

The wheel will rotate forwards and backwards depending on power received. It can be rotated left and right by sending a number signal to the steering input. It can also be locked into place by sending an on signal to the brake input.

### PROPERTIES

- Mass: 10
- Dimensions (WxDxH): 3x3x2
- Cost: $100
- Tags: steerable,steering,basic
- File: wheel_advanced_3.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Brake | Locks the wheel into place when receiving an on signal. |
| number | Variable Brake | A value between 0 and 1 for soft braking |
| number | Steering | Accepts a value between -1 and 1 that represents the extremes of the wheels steering rotation |

### connections

| Type | Label | Description |
| --- | --- | --- |
| power | RPS | Receives power generated by an engine to control forward and backward rotation. |

## Wheel 3x3 (Suspension)

Small steerable wheel with suspension, power connection, and braking.

The wheel will rotate forwards and backwards depending on power received. It can be rotated left and right by sending a number signal to the steering input. It can also be locked into place by sending an on signal to the brake input.

### PROPERTIES

- Mass: 15
- Dimensions (WxDxH): 3x3x3
- Cost: $150
- Tags: steerable,steering
- File: wheel_advanced_3_sus.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Brake | Locks the wheel into place when receiving an on signal. |
| number | Variable Brake | A value between 0 and 1 for soft braking |
| number | Steering | Accepts a value between -1 and 1 that represents the extremes of the wheels steering rotation |

### connections

| Type | Label | Description |
| --- | --- | --- |
| power | RPS | Receives power generated by an engine to control forward and backward rotation. |

## Wheel 5x5

Medium steerable wheel with power connection and braking.

The wheel will rotate forwards and backwards depending on power received. It can be rotated left and right by sending a number signal to the steering input. It can also be locked into place by sending an on signal to the brake input.

### PROPERTIES

- Mass: 20
- Dimensions (WxDxH): 5x5x3
- Cost: $150
- Tags: steerable,steering,basic
- File: wheel_advanced_5.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Brake | Locks the wheel into place when receiving an on signal. |
| number | Variable Brake | A value between 0 and 1 for soft braking |
| number | Steering | Accepts a value between -1 and 1 that represents the extremes of the wheels steering rotation |

### connections

| Type | Label | Description |
| --- | --- | --- |
| power | RPS | Receives power generated by an engine to control forward and backward rotation. |

## Wheel 5x5 (Suspension)

Medium steerable wheel with suspension, power connection, and braking.

The wheel will rotate forwards and backwards depending on power received. It can be rotated left and right by sending a number signal to the steering input. It can also be locked into place by sending an on signal to the brake input.

### PROPERTIES

- Mass: 30
- Dimensions (WxDxH): 5x5x5
- Cost: $200
- Tags: steerable,steering
- File: wheel_advanced_5_sus.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Brake | Locks the wheel into place when receiving an on signal. |
| number | Variable Brake | A value between 0 and 1 for soft braking |
| number | Steering | Accepts a value between -1 and 1 that represents the extremes of the wheels steering rotation |

### connections

| Type | Label | Description |
| --- | --- | --- |
| power | RPS | Receives power generated by an engine to control forward and backward rotation. |

## Wheel 7x7

Large steerable wheel with power connection and braking.

The wheel will rotate forwards and backwards depending on power received. It can be rotated left and right by sending a number signal to the steering input. It can also be locked into place by sending an on signal to the brake input.

### PROPERTIES

- Mass: 40
- Dimensions (WxDxH): 7x7x4
- Cost: $200
- Tags: steerable,steering,basic
- File: wheel_advanced_7.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Brake | Locks the wheel into place when receiving an on signal. |
| number | Variable Brake | A value between 0 and 1 for soft braking |
| number | Steering | Accepts a value between -1 and 1 that represents the extremes of the wheels steering rotation |

### connections

| Type | Label | Description |
| --- | --- | --- |
| power | RPS | Receives power generated by an engine to control forward and backward rotation. |

## Wheel 7x7 (Suspension)

Large steerable wheel with suspension, power connection, and braking.

The wheel will rotate forwards and backwards depending on power received. It can be rotated left and right by sending a number signal to the steering input. It can also be locked into place by sending an on signal to the brake input.

### PROPERTIES

- Mass: 60
- Dimensions (WxDxH): 7x7x6
- Cost: $250
- Tags: steerable,steering
- File: wheel_advanced_7_sus.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Brake | Locks the wheel into place when receiving an on signal. |
| number | Variable Brake | A value between 0 and 1 for soft braking |
| number | Steering | Accepts a value between -1 and 1 that represents the extremes of the wheels steering rotation |

### connections

| Type | Label | Description |
| --- | --- | --- |
| power | RPS | Receives power generated by an engine to control forward and backward rotation. |

## Wheel 9x9

XLarge steerable wheel with power connection and braking.

The wheel will rotate forwards and backwards depending on power received. It can be rotated left and right by sending a number signal to the steering input. It can also be locked into place by sending an on signal to the brake input.

### PROPERTIES

- Mass: 80
- Dimensions (WxDxH): 9x9x5
- Cost: $250
- Tags: steerable,steering,basic
- File: wheel_advanced_9.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Brake | Locks the wheel into place when receiving an on signal. |
| number | Variable Brake | A value between 0 and 1 for soft braking |
| number | Steering | Accepts a value between -1 and 1 that represents the extremes of the wheels steering rotation |

### connections

| Type | Label | Description |
| --- | --- | --- |
| power | RPS | Receives power generated by an engine to control forward and backward rotation. |

## Wheel 9x9 (Suspension)

XLarge steerable wheel with suspension, power connection, and braking.

The wheel will rotate forwards and backwards depending on power received. It can be rotated left and right by sending a number signal to the steering input. It can also be locked into place by sending an on signal to the brake input.

### PROPERTIES

- Mass: 120
- Dimensions (WxDxH): 9x10x8
- Cost: $300
- Tags: steerable,steering
- File: wheel_advanced_9_sus.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Brake | Locks the wheel into place when receiving an on signal. |
| number | Variable Brake | A value between 0 and 1 for soft braking |
| number | Steering | Accepts a value between -1 and 1 that represents the extremes of the wheels steering rotation |

### connections

| Type | Label | Description |
| --- | --- | --- |
| power | RPS | Receives power generated by an engine to control forward and backward rotation. |

## Wheel Coaster

Simple small wheel that requires no engine power and spins freely.

You cannot control the forward and backward rotation of this wheel, but it can be locked into place by sending an on signal to the brake input.

### PROPERTIES

- Mass: 4
- Dimensions (WxDxH): 3x3x3
- Cost: $25
- Tags: basic
- File: wheel_coaster.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Brake | Locks the wheel into place when receiving an on signal. |
| number | Variable Brake | A value between 0 and 1 for soft braking |

## Wing Front Section (Small)

The wing front surface cuts through the air while resisting movement against the flat plane of its surface. The aerofoil section also provides lift.

Wing surface to provide lift and cut through the air.

### PROPERTIES

- Mass: 5
- Dimensions (WxDxH): 1x3x7
- Cost: $100
- Tags: airplane,aeroplane,basic
- File: wing_small_front.xml

## Wing Section (Large)

The wing surface cuts through the air while resisting movement against the flat plane of its surface. The aerofoil section also provides lift.

Wing surface to provide lift and cut through the air.

### PROPERTIES

- Mass: 20
- Dimensions (WxDxH): 3x16x7
- Cost: $500
- Tags: airplane,aeroplane,basic
- File: wing_large.xml

## Wing Section (Medium)

The wing surface cuts through the air while resisting movement against the flat plane of its surface. The aerofoil section also provides lift.

Wing surface to provide lift and cut through the air.

### PROPERTIES

- Mass: 15
- Dimensions (WxDxH): 2x10x3
- Cost: $350
- Tags: airplane,aeroplane,basic
- File: wing_medium.xml

## Wing Section (Small)

The wing surface cuts through the air while resisting movement against the flat plane of its surface. The aerofoil section also provides lift.

Wing surface to provide lift and cut through the air.

### PROPERTIES

- Mass: 8
- Dimensions (WxDxH): 1x6x3
- Cost: $150
- Tags: airplane,aeroplane,basic
- File: wing_small.xml

## Wing Section (XLarge)

The wing surface cuts through the air while resisting movement against the flat plane of its surface. The aerofoil section also provides lift.

Wing surface to provide lift and cut through the air.

### PROPERTIES

- Mass: 30
- Dimensions (WxDxH): 3x22x7
- Cost: $800
- Tags: airplane,aeroplane,basic
- File: wing_xl.xml

## Wing Section (XXLarge)

The wing surface cuts through the air while resisting movement against the flat plane of its surface. The aerofoil section also provides lift.

Wing surface to provide lift and cut through the air.

### PROPERTIES

- Mass: 50
- Dimensions (WxDxH): 3x28x7
- Cost: $1500
- Tags: airplane,aeroplane
- File: wing_xxl.xml

## Data Logger (Bool) (Deprecated)

> [!WARNING]
> This component is deprecated.

A bool data logging block for unit tests.

Link to the bool output node of another component to record data for unit tests.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $1
- Tags: 
- File: data_logger_bool.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Bool In |  |

## Data Logger (Number) (Deprecated)

> [!WARNING]
> This component is deprecated.

A number data logging block for unit tests.

Link to the number output node of another component to record data for unit tests.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $1
- Tags: 
- File: data_logger_number.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| number | Number In |  |

## Radio RX Huge (Deprecated)

> [!WARNING]
> This component is deprecated.

A radio data transmitter and receiver.

Sends and receives data on the specified frequencies.

### PROPERTIES

- Mass: 20
- Dimensions (WxDxH): 1x1x9
- Cost: $5000
- Tags: 
- File: rx_huge.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| composite | Data Send |  |
| number | Frequency Send |  |
| number | Frequency Recv |  |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| composite | Data Recv |  |
| number | Signal Strength |  |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric |  |

## Radio RX Large (Deprecated)

> [!WARNING]
> This component is deprecated.

A radio data transmitter and receiver.

Sends and receives data on the specified frequencies.

### PROPERTIES

- Mass: 12
- Dimensions (WxDxH): 1x1x5
- Cost: $200
- Tags: 
- File: rx_large.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| composite | Data Send |  |
| number | Frequency Send |  |
| number | Frequency Recv |  |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| composite | Data Recv |  |
| number | Signal Strength |  |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric |  |

## Radio RX Medium (Deprecated)

> [!WARNING]
> This component is deprecated.

A radio data transmitter and receiver.

Sends and receives data on the specified frequencies.

### PROPERTIES

- Mass: 8
- Dimensions (WxDxH): 1x1x4
- Cost: $1000
- Tags: 
- File: rx_med.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| composite | Data Send |  |
| number | Frequency Send |  |
| number | Frequency Recv |  |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| composite | Data Recv |  |
| number | Signal Strength |  |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric |  |

## Radio RX Small (Deprecated)

> [!WARNING]
> This component is deprecated.

A radio data transmitter and receiver.

Sends and receives data on the specified frequencies.

### PROPERTIES

- Mass: 5
- Dimensions (WxDxH): 1x1x2
- Cost: $500
- Tags: 
- File: rx_small.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| composite | Data Send |  |
| number | Frequency Send |  |
| number | Frequency Recv |  |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| composite | Data Recv |  |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric |  |
