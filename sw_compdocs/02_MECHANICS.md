# Mechanics

## Clutch

A clutch for managing the transmission of power between two nodes.

The number input controls the amount of power transmitted.

### PROPERTIES

- Mass: 2
- Dimensions (WxDxH): 1x1x2
- Cost: $50
- Tags: basic
- File: torque_clutch.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| number | Clutch Pressure | A number between 0 and 1 representing the clutch engagement factor. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| power | RPS B | Power connection B. |
| power | RPS A | Power connection A. |
| electric | Electric | The electric connection to power the component. |

## Compact Linear Track Base

A compact slider that moves along a modular linear track.

You can build the track using the Compact Linear Track Extension component. The speed of the slider can be set using its number input.

### PROPERTIES

- Mass: 5
  - Parent Mass: 2
  - Child Mass: 3
- Dimensions (WxDxH): 1x1x2
  - Parent Dimensions (WxDxH): 1x1x1
  - Child Dimensions (WxDxH): 1x1x1
- Cost: $20
- Tags: 
- Parent File: linear_compact_base.xml
- Child File: linear_compact_head.xml

### logic inputs

| Body | Type | Label | Description |
| --- | --- | --- | --- |
| Parent | number | Slider Speed |  |

### connections

| Body | Type | Label | Description |
| --- | --- | --- | --- |
| Parent | electric | Electric | Electrical power connection. |

## Compact Linear Track Extension

An extension piece that can be used to build compact linear tracks.

A Compact Linear Track Base must be attached somewhere along the track for it to function.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $20
- Tags: 
- File: linear_compact_module.xml

## Compact Robotic Pivot

A small robotic pivot that will orientate towards the input value within its range of motion.

The pivot has a range of motion of 0.25 turns in both directions. A standard input value sets the target orientation within the pivot's range of motion. The pivot's speed can be configured by selecting it with the select tool.

### PROPERTIES

- Mass: 2
  - Parent Mass: 1
  - Child Mass: 1
- Dimensions (WxDxH): 1x1x2
  - Parent Dimensions (WxDxH): 1x1x1
  - Child Dimensions (WxDxH): 1x1x1
- Cost: $40
- Tags: 
- Parent File: multibody_compact_pivot_robotic_a.xml
- Child File: multibody_compact_pivot_b.xml

### logic inputs

| Body | Type | Label | Description |
| --- | --- | --- | --- |
| Parent | number | Rotation Target | The standard value setting the orientation within the range of motion. |

### connections

| Body | Type | Label | Description |
| --- | --- | --- | --- |
| Parent | electric | Electric | Electrical power connection. |

## Compact Velocity Pivot

A small pivot that will continuously rotate at a set input speed.

Inputting a value of 0 will cause it to stop.

### PROPERTIES

- Mass: 2
  - Parent Mass: 1
  - Child Mass: 1
- Dimensions (WxDxH): 1x1x2
  - Parent Dimensions (WxDxH): 1x1x1
  - Child Dimensions (WxDxH): 1x1x1
- Cost: $40
- Tags: 
- Parent File: multibody_compact_pivot_velocity_a.xml
- Child File: multibody_compact_pivot_b.xml

### logic inputs

| Body | Type | Label | Description |
| --- | --- | --- | --- |
| Parent | number | Rotational Speed | The speed at which the pivot should rotate. |

### connections

| Body | Type | Label | Description |
| --- | --- | --- | --- |
| Parent | electric | Electric | Electrical power connection. |

## Door Frame Controller

Controller unit for sealing door frames.

Placing the controller as part of a door frame will let you lock the door when closed, and check whether the door is closed enough to be forming a seal. Only one controller should be placed per frame.

### PROPERTIES

- Mass: 10
- Dimensions (WxDxH): 2x1x1
- Cost: $100
- Tags: 
- File: door_frame_controller.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Lock Seal | Controls if the door panel will lock in place when sealed. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Seal State | Indicates if the door panel is closed and forming a seal. |

## Door Frame Corner

A corner piece for building openings to sealed fluid compartments.

To create a valid frame, there must be a continuous loop of frame parts in a consistent orientation with no other parts inside the frame.

### PROPERTIES

- Mass: 15
- Dimensions (WxDxH): 2x1x2
- Cost: $50
- Tags: 
- File: door_frame_corner.xml

## Door Frame Edge

A straight edge for building openings to sealed fluid compartments.

To create a valid frame, there must be a continuous loop of frame parts in a consistent orientation with no other parts inside the frame.

### PROPERTIES

- Mass: 5
- Dimensions (WxDxH): 1x1x1
- Cost: $10
- Tags: 
- File: door_frame_straight.xml

## Door Panel Corner

A corner piece for building door panels.

A valid door panel can be created with a loop of door panel pieces, filled with blocks flush to the outer face. Door panels must also fill a door frame and be built in their closed position within the frame to be valid.

### PROPERTIES

- Mass: 5
- Dimensions (WxDxH): 1x1x1
- Cost: $20
- Tags: 
- File: door_panel_corner.xml

## Door Panel Edge

A straight edge piece for building door panels.

A valid door panel can be created with a loop of door panel pieces, filled with blocks flush to the outer face. Door panels must also fill a door frame and be built in their closed position within the frame to be valid.

### PROPERTIES

- Mass: 5
- Dimensions (WxDxH): 1x1x1
- Cost: $10
- Tags: 
- File: door_panel_straight.xml

## Electric Connector

A small electric connector that can be used to transfer electric energy between vehicles.

Two electric connectors will attach when they are within close proximity. When connected, electric energy will flow freely between the connectors.

### PROPERTIES

- Mass: 2
- Dimensions (WxDxH): 1x1x2
- Cost: $20
- Tags: magnet
- File: connector_electric.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Release Connector | Release the connector when receiving an on signal. |
| composite | Composite Data Send | Composite data to send to the connected connector. |
| video | Video Data Send | Video data to send to the connected connector. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Connected | Outputs an on signal if the connector is attached to another connector. |
| composite | Composite Data Receive | Composite data to receive from the connected connector. |
| video | Video Data Receive | Video data to receive from the connected connector. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Fluid Connector

A fluid connector that can be used to transfer fluid between vehicles.

Two fluid connectors will attach when they are within close proximity. When connected, fluid will flow freely between the connectors.

### PROPERTIES

- Mass: 2
- Dimensions (WxDxH): 1x1x2
- Cost: $20
- Tags: magnet
- File: connector_water.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Release Connector | Release the connector when receiving an on signal. |
| composite | Composite Data Send | Composite data to send to the connected connector. |
| video | Video Data Send | Video data to send to the connected connector. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Connected | Outputs an on signal if the connector is attached to another connector. |
| composite | Composite Data Receive | Composite data to receive from the connected connector. |
| video | Video Data Receive | Video data to receive from the connected connector. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Fluid | Fluid connection to link to another fluid connector. |

## Gearbox (Deprecated)

> [!WARNING]
> This component is deprecated.

Gearbox for changing the torque and speed across power connections.

The ratio can be toggled between two values which can be set in the properties.

### PROPERTIES

- Mass: 8
- Dimensions (WxDxH): 1x2x2
- Cost: $100
- Tags: 
- File: torque_gearbox.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Gear Switch | Toggle between the two gear ratios. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| power | RPS A | Power connection A. |
| power | RPS B | Power connection B. |
| electric | Electric | The electric connection to power the component. |

## Gearbox (Deprecated)

> [!WARNING]
> This component is deprecated.

Gearbox for changing the torque and speed across power connections.

The ratio can be toggled between two values which can be set in the properties. This gearbox operates up to a torque difference of 4000.

### PROPERTIES

- Mass: 8
- Dimensions (WxDxH): 1x2x2
- Cost: $100
- Tags: 
- File: torque_gearbox_2.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Gear Switch | Toggle between the two gear ratios. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| power | RPS A | Power connection A. |
| power | RPS B | Power connection B. |
| electric | Electric | The electric connection to power the component. |

## Gearbox 1x1

Gearbox for changing the torque and speed across power connections.

The ratio can be toggled between two values which can be set in the properties.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $50
- Tags: basic
- File: modular_engine_gearbox_1x1.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Gear Switch | Toggle between the two gear ratios. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| power | RPS A | Power connection A. |
| power | RPS B | Power connection B. |
| electric | Electric | The electric connection to power the component. |

## Gearbox 3x3

Gearbox for changing the torque and speed across power connections.

The ratio can be toggled between two values which can be set in the properties.

### PROPERTIES

- Mass: 9
- Dimensions (WxDxH): 3x3x2
- Cost: $100
- Tags: 
- File: modular_engine_gearbox_3x3.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Gear Switch | Toggle between the two gear ratios. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| power | RPS A | Power connection A. |
| power | RPS B | Power connection B. |
| electric | Electric | The electric connection to power the component. |

## Gearbox 5x5

Gearbox for changing the torque and speed across power connections.

The ratio can be toggled between two values which can be set in the properties.

### PROPERTIES

- Mass: 25
- Dimensions (WxDxH): 5x5x3
- Cost: $150
- Tags: 
- File: modular_engine_gearbox_5x5.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Gear Switch | Toggle between the two gear ratios. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| power | RPS A | Power connection A. |
| power | RPS B | Power connection B. |
| electric | Electric | The electric connection to power the component. |

## Hardpoint Connector Attachment

A hardpoint connector for building detachable vehicle sections.

A hardpoint body will connect to a hardpoint attachment when correctly aligned, fixing the two components in place while transferring logic and fluid.

### PROPERTIES

- Mass: 2
- Dimensions (WxDxH): 1x1x2
- Cost: $20
- Tags: 
- File: connector_hardpoint_b.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| composite | Composite Data Send | Composite data to send to the connected connector. |
| video | Video Data Send | Video data to send to the connected connector. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Launched | Outputs an on signal if the connector is sent a launch signal by the parent. |
| composite | Composite Data Receive | Composite data to receive from the connected connector. |
| video | Video Data Receive | Video data to receive from the connected connector. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Fluid | Fluid connection to link to another fluid connector. |
| electric | Electric | Electrical power connection. |

## Hardpoint Connector Attachment (Round)

A hardpoint connector for building detachable vehicle sections.

A hardpoint body will connect to a hardpoint attachment when correctly aligned, fixing the two components in place while transferring logic and fluid.

### PROPERTIES

- Mass: 2
- Dimensions (WxDxH): 1x1x2
- Cost: $20
- Tags: 
- File: connector_hardpoint_b_round.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| composite | Composite Data Send | Composite data to send to the connected connector. |
| video | Video Data Send | Video data to send to the connected connector. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Launched | Outputs an on signal if the connector is sent a launch signal by the parent. |
| composite | Composite Data Receive | Composite data to receive from the connected connector. |
| video | Video Data Receive | Video data to receive from the connected connector. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Fluid | Fluid connection to link to another fluid connector. |
| electric | Electric | Electrical power connection. |

## Hardpoint Connector Body

A hardpoint connector for building detachable vehicle sections.

A hardpoint body will connect to a hardpoint attachment when correctly aligned, fixing the two components in place while transferring logic and fluid. The hardpoint body can release the connection by receiving an on/off input signal.

### PROPERTIES

- Mass: 2
- Dimensions (WxDxH): 1x3x1
- Cost: $20
- Tags: 
- File: connector_hardpoint_a.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Release | Release the connector when receiving an on signal. |
| on/off | Launch | Release the connector and activate the ordinance when receiving an on signal. |
| composite | Composite Data Send | Composite data to send to the connected connector. |
| video | Video Data Send | Video data to send to the connected connector. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Ordinance Type | Returns the ordinance type of the attached object. |
| composite | Composite Data Receive | Composite data to receive from the connected connector. |
| video | Video Data Receive | Video data to receive from the connected connector. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Fluid | Fluid connection to link to another fluid connector. |
| electric | Electric | Electrical power connection. |

## Hinge Connector

A small magnetic connector that can be used to attach two or more vehicles together.

Two connectors will attach when they are within close proximity and both are switched on. They will connect along their long edge and hinge along this axis. An on/off output allows you to check whether or not this connector is currently attached to anything.

### PROPERTIES

- Mass: 3
- Dimensions (WxDxH): 1x3x2
- Cost: $40
- Tags: magnet
- File: connector_hinge.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Magnet Toggle | Enables the connector's magnet when receiving an on signal. |
| composite | Composite Data Send | Composite data to send to the connected connector. |
| video | Video Data Send | Video data to send to the connected connector. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Connected | Outputs an on signal if the connector is attached to another connector. |
| composite | Composite Data Receive | Composite data to receive from the connected connector. |
| video | Video Data Receive | Video data to receive from the connected connector. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Hinged Dock Door

Hinged door that can be opened and closed using an on/off signal.

### PROPERTIES

- Mass: 20
- Dimensions (WxDxH): 9x1x5
- Cost: $300
- Tags: door,basic
- File: door_dock_large.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Open/Close | Opens the door when receiving an on signal, and closes it when receiving an off signal. |
| on/off | Magnet Toggle | Enables the door's magnet when receiving an on signal. |
| on/off | On/Off Sent | An on/off signal to send to a connected door. |
| number | Number Sent | A number signal to send to a connected door. |
| composite | Composite input | Composite data input. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Connected | Outputs an on signal if the door is attached to another door. |
| on/off | On/Off Received | The on/off signal received from a connected door. |
| number | Number Received | The number value received from a connected door. |
| composite | Composite output | Composite data output. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Hinged Dock Hatch

Hinged door that can be opened and closed using an on/off signal.

### PROPERTIES

- Mass: 15
- Dimensions (WxDxH): 5x1x5
- Cost: $200
- Tags: door,basic
- File: door_dock_small.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Open/Close | Opens the door when receiving an on signal, and closes it when receiving an off signal. |
| on/off | Magnet Toggle | Enables the door's magnet when receiving an on signal. |
| on/off | On/Off Sent | An on/off signal to send to a connected door. |
| number | Number Sent | A number signal to send to a connected door. |
| composite | Composite input | Composite data input. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Connected | Outputs an on signal if the door is attached to another door. |
| on/off | On/Off Received | The on/off signal received from a connected door. |
| number | Number Received | The number value received from a connected door. |
| composite | Composite output | Composite data output. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Hinged Door

Hinged door that can be opened and closed by hand and locked using an on/off signal.

### PROPERTIES

- Mass: 20
- Dimensions (WxDxH): 7x1x4
- Cost: $200
- Tags: door,basic
- File: door_manual_large.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Lock | Locks the door when receiving an on signal. |

## Hinged Hatch

Hinged door that can be opened and closed by hand and locked using an on/off signal.

### PROPERTIES

- Mass: 15
- Dimensions (WxDxH): 3x1x4
- Cost: $150
- Tags: door,basic
- File: door_manual_small.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Lock | Locks the door when receiving an on signal. |

## Key Button

A button that must be held down for a set duration before activating.

Once activated, interacting with the button again will deactivate it instantly. The hold duration can be customised by selecting this component with the select tool. The external input can be used to simulate interacting with the button down using the output of another component. The button's default state can be configured by selecting it with the select component.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x2
- Cost: $20
- Tags: basic
- File: button_key.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | External Input | Allows an external on/off signal to hold the button down. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Activated | Outputs an on signal when interacting with the button for the set duration. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Large Connector

A magnetic connector that can be used to attach two or more vehicles together.

Two large connectors will attach when they are within close proximity and both are switched on. The additional inputs and outputs allow you to send and receive power and signals between two connected magnets, giving you a limited amount of control over a linked vehicle. An additional on/off output allows you to check whether or not this connector is currently attached to anything.

### PROPERTIES

- Mass: 20
- Dimensions (WxDxH): 3x3x2
- Cost: $50
- Tags: magnet
- File: connector_large.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Magnet Toggle | Enables the connector's magnet when receiving an on signal. |
| on/off | On/Off Sent | An on/off signal to send to a connected magnet. |
| number | Number Sent | A number signal to send to a connected magnet. |
| composite | Composite Data Send | Composite data to send to the connected connector. |
| video | Video Data Send | Video data to send to the connected connector. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Number Received | The number value received from a connected magnet. |
| on/off | Connected | Outputs an on signal if the connector is attached to another connector. |
| on/off | On/Off Received | The on/off signal received from a connected magnet. |
| composite | Composite Data Receive | Composite data to receive from the connected connector. |
| video | Video Data Receive | Video data to receive from the connected connector. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| power | RPS | Power connection for transfering mechanical energy to another connector. |
| electric | Electric | Electrical power connection. |
| fluid | Fluid | Fluid connection for transfering fluid to another connector. |

## Large Keypad

A keypad that allows 2 numbers to be input.

Interacting with the keypad will show a menu where the 2 numbers can be entered, along with a button for quickly inputting waypoint coordinates. A short pulse will be emitted from the keypad's pulse node when the confirm button is clicked and the stored numbers will be continuously output from the other output nodes. An on/off signal controls whether or not the keypad's backlight is enabled.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x2x2
- Cost: $40
- Tags: button,input
- File: button_keypad_large.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Backlight | Enables the backlight when receiving an on signal. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Output A | Outputs the first stored value. |
| number | Output B | Outputs the second stored value. |
| on/off | Pulse | Emits a short pulse when a value is entered. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Linear Track Base

A slider that moves along a modular linear track.

You can build the track using the Linear Track Extension component. This base component provides 3 blocks that can be built on. A pair of on/off signals allow you to control the up and down motion of the slider, and a numerical output lets you measure the slider's offset from its starting position. Multiple slider bases can run along the same track. The up/down speed can be configured by selecting this component with the select tool.

### PROPERTIES

- Mass: 6
  - Parent Mass: 3
  - Child Mass: 3
- Dimensions (WxDxH): 3x1x3
  - Parent Dimensions (WxDxH): 3x1x2
  - Child Dimensions (WxDxH): 3x1x1
- Cost: $40
- Tags: 
- Parent File: linear_base.xml
- Child File: linear_head.xml

### logic inputs

| Body | Type | Label | Description |
| --- | --- | --- | --- |
| Parent | on/off | Down | Moves the slider in the track's down direction (indicated by the hollow arrow). |
| Parent | on/off | Up | Moves the slider in the track's up direction (indicated by the filled arrow). |

### logic outputs

| Body | Type | Label | Description |
| --- | --- | --- | --- |
| Parent | number | Slider Position | The measured offset of the slider from its starting position. |

### connections

| Body | Type | Label | Description |
| --- | --- | --- | --- |
| Parent | electric | Electric | Electrical power connection. |
| Parent | power | RPS | Power connection for transfering mechanical energy. |
| Parent | fluid | Fluid | Fluid connection for transfering fluid. |
| Child | power | RPS | Power connection for transfering mechanical energy. |
| Child | fluid | Fluid | Fluid connection for transfering fluid. |

## Linear Track Extension

An extension piece that can be used to build linear tracks.

A Linear Track Base must be attached somewhere along the track for it to function.

### PROPERTIES

- Mass: 3
- Dimensions (WxDxH): 3x1x2
- Cost: $10
- Tags: 
- File: linear_module.xml

## Lockable Button

A toggle button that can only be interacted with when unlocked.

An on signal must be sent to the button's unlock node to allow player interaction. The button's default state can be configured by selecting it with the select component.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x2
- Cost: $20
- Tags: 
- File: button_lock.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Unlock | Allows the button to be interacted with when receiving an on signal. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Toggled | Outputs an on/off signal that can be toggled by interacting with [q]/[e] when unlocked. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Mag All

A small connector that will attach to most surfaces.

While the connector is active the end will glow and it will stick to most surfaces that it touches. The connection will break if enough stress (200) is applied.

### PROPERTIES

- Mass: 5
- Dimensions (WxDxH): 1x1x3
- Cost: $250
- Tags: magnet
- File: magall.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Magnet Toggle | Enables the connector's magnet when receiving an on signal. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Connected | Outputs an on signal if the connector is attached to another connector. |
| number | Force | Outputs the current force stress on the connector. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Piston Suspension

A shock absorber that can be used to improve handling of land-based vehicles.

A dampened hydraulic sprung piston.

### PROPERTIES

- Mass: 40
  - Parent Mass: 20
  - Child Mass: 20
- Dimensions (WxDxH): 1x1x3
  - Parent Dimensions (WxDxH): 1x1x2
  - Child Dimensions (WxDxH): 1x1x1
- Cost: $20
- Tags: 
- Parent File: multibody_piston_suspension_a.xml
- Child File: multibody_piston_suspension_b.xml

## Pivot

A basic pivot that can move freely.

The pivot can rotate to 0.25 turns in both directions.

### PROPERTIES

- Mass: 2
  - Parent Mass: 1
  - Child Mass: 1
- Dimensions (WxDxH): 1x1x3
  - Parent Dimensions (WxDxH): 1x1x2
  - Child Dimensions (WxDxH): 1x1x1
- Cost: $20
- Tags: hinge
- Parent File: multibody_pivot_a.xml
- Child File: multibody_pivot_b.xml

## Pneumatic Piston

A pneumatic piston that can be expanded and contracted.

A standard value input sets the target position that the piston rod should move to. There is also an output for taking a measurement of the rod's current position. The piston can expand by a length of 1 metre, making it a total of 2.25m (9 blocks) tall when expanded and 1.25m (5 blocks) tall when contracted. The piston's speed can be configured by selecting it with the select tool.

### PROPERTIES

- Mass: 8
  - Parent Mass: 5
  - Child Mass: 3
- Dimensions (WxDxH): 1x1x7
  - Parent Dimensions (WxDxH): 1x1x3
  - Child Dimensions (WxDxH): 1x1x2
- Cost: $100
- Tags: 
- Parent File: linear_matic_a.xml
- Child File: linear_matic_b.xml

### logic inputs

| Body | Type | Label | Description |
| --- | --- | --- | --- |
| Parent | number | Piston Rod Target Position | Takes a standard value representing the desired position of the rod. |

### logic outputs

| Body | Type | Label | Description |
| --- | --- | --- | --- |
| Parent | number | Piston Rod Position | The measured position of the rod between -0.5 and 0.5 metres. |

### connections

| Body | Type | Label | Description |
| --- | --- | --- | --- |
| Parent | electric | Electric | Electrical power connection. |
| Parent | fluid | Fluid | Fluid connection for transfering fluid. |
| Child | fluid | Fluid |  |

## Push Button

A button that outputs an on signal when you interact with [q]/[e], and an off signal when not interacting.

An external on/off signal can also be used to control whether or not the button is pressed, allowing you to chain multiple buttons together to unify their outputs.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x2
- Cost: $10
- Tags: basic
- File: button_push.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | External Input | Allows an external on/off signal to control whether or not the button is pressed. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Pressed | Outputs an on signal when you interact wtih [q]/[e], and an off signal otherwise. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Push Button (2 Sided)

A button that outputs an on signal when interacting with [q]/[e].

An external on/off signal can also be used to control whether or not the button is pressed, allowing you to chain multiple buttons together to unify their outputs.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x2
- Cost: $10
- Tags: basic
- File: button_push_2side.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | External Input | Allows an external on/off signal to control whether or not the button is pressed. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Pressed | Outputs an on signal when you interact with [q]/[e], and an off signal otherwise. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Reaction Wheel

A stabilization system that outputs a force to counter the input rotation.

This component can be wired directly to an aligned angular rotation sensor to stabilize its rotation.

### PROPERTIES

- Mass: 15
- Dimensions (WxDxH): 3x3x1
- Cost: $300
- Tags: 
- File: gyroscopic_stabilizer.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| number | Rotation | Input rotation value. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Reaction Wheel (Large)

A stabilization system that outputs a force to counter the input rotation.

This component can be wired directly to an aligned angular rotation sensor to stabilize its rotation.

### PROPERTIES

- Mass: 80
- Dimensions (WxDxH): 5x5x3
- Cost: $700
- Tags: 
- File: gyroscopic_stabilizer_large.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| number | Rotation | Input rotation value. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Reaction Wheel (Small)

A stabilization system that outputs a force to counter the input rotation.

This component can be wired directly to an aligned angular rotation sensor to stabilize its rotation.

### PROPERTIES

- Mass: 2
- Dimensions (WxDxH): 1x1x1
- Cost: $150
- Tags: 
- File: gyroscopic_stabilizer_small.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| number | Rotation | Input rotation value. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Robotic Door Hinge

A powered robotic hinge for custom sealable doors.

The hinge has a range of motion of 0.25 in each direction. A standard input value sets the target orientation within the pivot's range of motion. The measured rotation of the hinge can be read from its output. The hinge's speed can be configured by selecting it with the select tool.

### PROPERTIES

- Mass: 6
  - Parent Mass: 3
  - Child Mass: 3
- Dimensions (WxDxH): 1x3x3
  - Parent Dimensions (WxDxH): 1x3x2
  - Child Dimensions (WxDxH): 1x3x1
- Cost: $400
- Tags: 
- Parent File: multibody_door_hinge_a.xml
- Child File: multibody_door_hinge_b.xml

### logic inputs

| Body | Type | Label | Description |
| --- | --- | --- | --- |
| Parent | number | Rotation Target | The standard value setting the orientation within the range of motion. |

### logic outputs

| Body | Type | Label | Description |
| --- | --- | --- | --- |
| Parent | number | Current Rotation | The hinge's measured rotation between -0.25 and 0.25. |

### connections

| Body | Type | Label | Description |
| --- | --- | --- | --- |
| Parent | electric | Electric | Electrical power connection. |

## Robotic Hinge

A powered robotic hinge that will orientate towards the input value within its range of motion.

The hinge has a range of motion of 0.25 turns in both directions. A standard input value sets the target orientation within the pivot's range of motion. The measured rotation of the hinge can be read from its output. The hinge's speed can be configured by selecting it with the select tool.

### PROPERTIES

- Mass: 6
  - Parent Mass: 3
  - Child Mass: 3
- Dimensions (WxDxH): 1x3x3
  - Parent Dimensions (WxDxH): 1x3x2
  - Child Dimensions (WxDxH): 1x3x1
- Cost: $400
- Tags: 
- Parent File: multibody_robotic_hinge_01_a.xml
- Child File: multibody_robotic_hinge_01_b.xml

### logic inputs

| Body | Type | Label | Description |
| --- | --- | --- | --- |
| Parent | number | Rotation Target | The standard value setting the orientation within the range of motion. |

### logic outputs

| Body | Type | Label | Description |
| --- | --- | --- | --- |
| Parent | number | Current Rotation | The hinge's measured rotation between -0.25 and 0.25. |

### connections

| Body | Type | Label | Description |
| --- | --- | --- | --- |
| Parent | electric | Electric | Electrical power connection. |
| Parent | power | RPS | Power connection for transfering mechanical energy. |
| Parent | fluid | Fluid | Fluid connection for transfering fluid. |
| Child | power | RPS | Power connection for transfering mechanical energy. |
| Child | fluid | Fluid | Fluid connection for transfering fluid. |

## Robotic Pivot (Fluid)

A robotic pivot that will orientate towards the input value within its range of motion.

The pivot has a range of motion of 0.25 turns in both directions. A standard input value sets the target orientation within the pivot's range of motion. The measured rotation of the pivot can be read from its output. The pivot's speed can be configured by selecting it with the select tool.

### PROPERTIES

- Mass: 10
  - Parent Mass: 9
  - Child Mass: 1
- Dimensions (WxDxH): 3x3x2
  - Parent Dimensions (WxDxH): 3x3x1
  - Child Dimensions (WxDxH): 1x1x1
- Cost: $200
- Tags: 
- Parent File: multibody_robotic_pivot_01_a_fluid.xml
- Child File: multibody_robotic_pivot_01_b_fluid.xml

### logic inputs

| Body | Type | Label | Description |
| --- | --- | --- | --- |
| Parent | number | Rotation Target | The standard value setting the orientation within the range of motion. |

### logic outputs

| Body | Type | Label | Description |
| --- | --- | --- | --- |
| Parent | number | Current Rotation | The pivot's measured rotation between -0.25 and 0.25. |

### connections

| Body | Type | Label | Description |
| --- | --- | --- | --- |
| Parent | electric | Electric | Electrical power connection. |
| Parent | fluid | Fluid | Fluid connection for transfering fluids. |
| Child | fluid | Fluid | Fluid connection for transfering fluids. |

## Robotic Pivot (Power)

A robotic pivot that will orientate towards the input value within its range of motion.

The pivot has a range of motion of 0.25 turns in both directions. A standard input value sets the target orientation within the pivot's range of motion. The measured rotation of the pivot can be read from its output. The pivot's speed can be configured by selecting it with the select tool.

### PROPERTIES

- Mass: 10
  - Parent Mass: 9
  - Child Mass: 1
- Dimensions (WxDxH): 3x3x2
  - Parent Dimensions (WxDxH): 3x3x1
  - Child Dimensions (WxDxH): 1x1x1
- Cost: $200
- Tags: 
- Parent File: multibody_robotic_pivot_01_a.xml
- Child File: multibody_robotic_pivot_01_b.xml

### logic inputs

| Body | Type | Label | Description |
| --- | --- | --- | --- |
| Parent | number | Rotation Target | The standard value setting the orientation within the range of motion. |

### logic outputs

| Body | Type | Label | Description |
| --- | --- | --- | --- |
| Parent | number | Current Rotation | The pivot's measured rotation between -0.25 and 0.25. |

### connections

| Body | Type | Label | Description |
| --- | --- | --- | --- |
| Parent | electric | Electric | Electrical power connection. |
| Parent | power | RPS | Power connection for transfering mechanical energy. |
| Child | power | RPS | Power connection for transfering mechanical energy. |

## Sliding Connector Gripper

A connector that will attach to and slide along a connector track.

The gripper will attach to a track when they are aligned and close enough, and will detach when it slides off the end or receives an on signal to the connector release input. The brake can be enabled to prevent the gripper from sliding along the track.

### PROPERTIES

- Mass: 2
- Dimensions (WxDxH): 1x1x2
- Cost: $20
- Tags: 
- File: connector_slider_gripper.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Release Connector | Releases the connector when receiving an on signal. |
| on/off | Brake | Enables the gripper's brake to keep it in place on the track. |

## Sliding Connector Track

A connector that can be used to build a track for grippers to attach to.

Gripper connectors will attach to the track when aligned and close enough, and will detach when they slide off the end.

### PROPERTIES

- Mass: 2
- Dimensions (WxDxH): 1x1x1
- Cost: $10
- Tags: 
- File: connector_slider_track.xml

## Sliding Door

Sliding door that can be opened and closed by hand and locked using an on/off signal.

### PROPERTIES

- Mass: 20
- Dimensions (WxDxH): 1x6x7
- Cost: $50
- Tags: door,basic
- File: door_manual.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Lock | Locks the door when receiving an on signal. |

## Sliding Door (Electric)

Sliding door that can be opened and closed using an on/off signal.

### PROPERTIES

- Mass: 20
- Dimensions (WxDxH): 1x6x7
- Cost: $70
- Tags: door,basic
- File: door.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Open/Close | Opens the door when receiving an on signal, and closes it when receiving an off signal. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Sliding Hatch

Sliding door that can be opened and closed by hand and locked using an on/off signal.

### PROPERTIES

- Mass: 20
- Dimensions (WxDxH): 1x6x3
- Cost: $40
- Tags: door,basic
- File: door_manual_sliding_small.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Lock | Locks the door when receiving an on signal. |

## Sliding Hatch (Electric)

Sliding hatch that can be opened and closed using an on/off signal.

### PROPERTIES

- Mass: 15
- Dimensions (WxDxH): 1x6x3
- Cost: $50
- Tags: door,basic
- File: hatch.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Hatch Open/Close | Opens the hatch when receiving an on signal, and closes it when receiving an off signal. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Small Connector

A small magnetic connector that can be used to attach two or more vehicles together.

Two small connectors will attach when they are within close proximity and both are switched on. An on/off output allows you to check whether or not this connector is currently attached to anything.

### PROPERTIES

- Mass: 2
- Dimensions (WxDxH): 1x1x2
- Cost: $20
- Tags: magnet
- File: connector_small.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Magnet Toggle | Enables the connector's magnet when receiving an on signal. |
| composite | Composite Data Send | Composite data to send to the connected connector. |
| video | Video Data Send | Video data to send to the connected connector. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Connected | Outputs an on signal if the connector is attached to another connector. |
| composite | Composite Data Receive | Composite data to receive from the connected connector. |
| video | Video Data Receive | Video data to receive from the connected connector. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Small Keypad

A keypad that allows a number to be input.

Interacting with the keypad will show a menu where the number can be entered. The stored numbers will be continuously output from the other output node. An on/off signal controls whether or not the keypad's backlight is enabled.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x2
- Cost: $20
- Tags: button,input
- File: button_keypad_small.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Backlight | Enables the backlight when receiving an on signal. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Output | Outputs the stored value. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Suspension

A shock absorber that can be used to improve handling of land-based vehicles.

Power can be passed through the suspension, allowing you to attach and control a wheel at the end.

### PROPERTIES

- Mass: 8
  - Parent Mass: 5
  - Child Mass: 3
- Dimensions (WxDxH): 2x3x4
  - Parent Dimensions (WxDxH): 2x3x3
  - Child Dimensions (WxDxH): 1x1x1
- Cost: $50
- Tags: 
- Parent File: multibody_suspension_a.xml
- Child File: multibody_suspension_b.xml

### connections

| Body | Type | Label | Description |
| --- | --- | --- | --- |
| Parent | power | RPS | Power connection for transfering mechanical energy. |
| Child | power | RPS | Power connection for transfering mechanical energy. |

## Throttle Lever

A throttle lever that acts as two buttons controlling one number output.

The output ranges from -1 to 1, and will increase/decrease depending on which half of the lever you interact with. The two on/off inputs can be used to control the lever externally with different buttons. The speed of the lever can be configured by selecting this component with the select tool.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 2x1x2
- Cost: $30
- Tags: basic
- File: button_throttle_lever.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Up | Increases the Throttle Value when input is held. |
| on/off | Down | Decreases the Throttle Value when input is held. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Throttle | Outputs the stored Throttle Value. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Toggle Button

A button that toggles between sending an on or off signal when you press [q]/[e] on it.

An external on/off signal can also be used to control whether or not the button is pressed, allowing you to chain multiple buttons together to unify their outputs. The button's default state can be configured by selecting it with the select component.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x2
- Cost: $10
- Tags: basic
- File: button_toggle.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | External Input | Allows an external on/off signal to control whether or not the button is pressed. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Toggled | Outputs an on/off signal that can be toggled by interacting with [q]/[e]. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Toggle Button (2 Sided)

A button that toggles between sending an on or off signal when you press [q]/[e] on it.

An external on/off signal can also be used to control whether or not the button is pressed, allowing you to chain multiple buttons together to unify their outputs. The button's default state can be configured by selecting it with the select component.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x2
- Cost: $10
- Tags: basic
- File: button_toggle_2side.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | External Input | Allows an external on/off signal to control whether or not the button is pressed. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Toggled | Outputs an on/off signal that can be toggled by interacting with [q]/[e]. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Turret Ring (Large)

A large turret ring that can rotate continuously.

A turret ring rotates in the same way as a velocity pivot. The gap inside the turret ring creates a door seal, and can be used to extend a sealed volume through the turret ring.

### PROPERTIES

- Mass: 72
  - Parent Mass: 36
  - Child Mass: 36
- Dimensions (WxDxH): 9x9x2
  - Parent Dimensions (WxDxH): 9x9x1
  - Child Dimensions (WxDxH): 9x9x1
- Cost: $100
- Tags: 
- Parent File: multibody_turret_large_a.xml
- Child File: multibody_turret_large_b.xml

### logic inputs

| Body | Type | Label | Description |
| --- | --- | --- | --- |
| Parent | number | Rotational Speed | The speed at which the turret should rotate. |

### logic outputs

| Body | Type | Label | Description |
| --- | --- | --- | --- |
| Parent | number | Current Rotation | The turrets measured rotation expressed in fractions of full turns. |

### connections

| Body | Type | Label | Description |
| --- | --- | --- | --- |
| Parent | electric | Electric | Electrical power connection. |

## Turret Ring (Medium)

A medium turret ring that can rotate continuously.

A turret ring rotates in the same way as a velocity pivot. The gap inside the turret ring creates a door seal, and can be used to extend a sealed volume through the turret ring.

### PROPERTIES

- Mass: 44
  - Parent Mass: 22
  - Child Mass: 22
- Dimensions (WxDxH): 7x7x2
  - Parent Dimensions (WxDxH): 7x7x1
  - Child Dimensions (WxDxH): 7x7x1
- Cost: $75
- Tags: 
- Parent File: multibody_turret_medium_a.xml
- Child File: multibody_turret_medium_b.xml

### logic inputs

| Body | Type | Label | Description |
| --- | --- | --- | --- |
| Parent | number | Rotational Speed | The speed at which the turret should rotate. |

### logic outputs

| Body | Type | Label | Description |
| --- | --- | --- | --- |
| Parent | number | Current Rotation | The turrets measured rotation expressed in fractions of full turns. |

### connections

| Body | Type | Label | Description |
| --- | --- | --- | --- |
| Parent | electric | Electric | Electrical power connection. |

## Turret Ring (Small)

A small turret ring that can rotate continuously.

A turret ring rotates in the same way as a velocity pivot. The gap inside the turret ring creates a door seal, and can be used to extend a sealed volume through the turret ring.

### PROPERTIES

- Mass: 28
  - Parent Mass: 14
  - Child Mass: 14
- Dimensions (WxDxH): 5x5x2
  - Parent Dimensions (WxDxH): 5x5x1
  - Child Dimensions (WxDxH): 5x5x1
- Cost: $50
- Tags: 
- Parent File: multibody_turret_small_a.xml
- Child File: multibody_turret_small_b.xml

### logic inputs

| Body | Type | Label | Description |
| --- | --- | --- | --- |
| Parent | number | Rotational Speed | The speed at which the turret should rotate. |

### logic outputs

| Body | Type | Label | Description |
| --- | --- | --- | --- |
| Parent | number | Current Rotation | The turrets measured rotation expressed in fractions of full turns. |

### connections

| Body | Type | Label | Description |
| --- | --- | --- | --- |
| Parent | electric | Electric | Electrical power connection. |

## Velocity Pivot

A pivot that will continuously rotate at a set input speed.

Inputting a value of 0 will cause it to stop. The pivot's current rotation can be read from its output. An output of 1 corresponds to one full turn, and -1 to a full turn in the opposite direction.

### PROPERTIES

- Mass: 10
  - Parent Mass: 9
  - Child Mass: 1
- Dimensions (WxDxH): 3x3x2
  - Parent Dimensions (WxDxH): 3x3x1
  - Child Dimensions (WxDxH): 1x1x1
- Cost: $25
- Tags: 
- Parent File: multibody_velocity_pivot_a.xml
- Child File: multibody_velocity_pivot_b.xml

### logic inputs

| Body | Type | Label | Description |
| --- | --- | --- | --- |
| Parent | number | Rotational Speed | The speed at which the pivot should rotate. |

### logic outputs

| Body | Type | Label | Description |
| --- | --- | --- | --- |
| Parent | number | Current Rotation | The pivot's measured rotation expressed in fractions of full turns. |

### connections

| Body | Type | Label | Description |
| --- | --- | --- | --- |
| Parent | electric | Electric | Electrical power connection. |
