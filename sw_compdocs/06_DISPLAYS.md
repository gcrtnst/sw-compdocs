# Displays

## Artificial Horizon

The artificial horizon shows you the orientation of your vehicle with respect to the horizon line.

The horizon ball rotates up and down as your vehicle's pitch changes, and the central line gives an indication of your vehicle's roll. This is a useful component to have in your helicopter to make it easier to fly at night and in thick fog. An on/off signal can be used to toggle the backlight.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $20
- Tags: basic
- File: artificial_horizon.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Backlight | Enables the backlight when receiving an on signal. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Buzzer

A buzzer that will play a selected sound when toggled from off to on.

The type of sound, volume, and pitch can be customised by selecting this component with the select tool. It has an audible range of 30m.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $100
- Tags: sound,audio,siren
- File: buzzer.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Buzzer | Plays the selected sound when toggled from off to on. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Clock

An analogue clock display that outputs a number value representing the time of day.

The clock has a display to visualise the time of day or night. The 12 o'clock position is the white arrow on the face of the display.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x2
- Cost: $100
- Tags: basic
- File: clock.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Backlight | Enables the backlight when receiving an on signal. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Time | The time as a factor of a day, from 0 (midnight) to 1 (midnight). |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Compass Ball

The compass rotates to point to north on the map.

It is one of several tools that can be used to aid navigation in low visibility situations. An on/off signal controls whether or not the compass' backlight is enabled.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $20
- Tags: basic
- File: compass.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Backlight | Enables the backlight when receiving an on signal. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Dial

A dial with a rotating needle for displaying numerical values.

The dial's face represents values ranging from -1 to 1 by default. This can be configured by selecting it with the select tool. Values outside this range will cause the needle to wrap around, but can be scaled to fit using additional logic components if necessary. An on/off signal can be used to toggle the backlight.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x2
- Cost: $20
- Tags: basic
- File: dial.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| number | Value to Display | The numerical value to display, ideally scaled to be within a -1 to 1 range. |
| on/off | Backlight | Enables the backlight when receiving an on signal. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Digital Display

Displays a 5 digit (6 with decimal point disabled) signed numerical value with optional decimal point.

The position of the decimal point can be configured by selecting this component with the select tool, allowing you to control the number of decimal places in the output.

### PROPERTIES

- Mass: 2
- Dimensions (WxDxH): 1x2x1
- Cost: $20
- Tags: basic
- File: digital_display.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| number | Value to Display | The numerical value to display. |
| on/off | Backlight | Enables the backlight when receiving an on signal. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Gauge Display

A display with two needles that can be positioned independently.

The primary needle is white and the secondary needle is red. The positions of the needles represent values ranging from -1 to 1 by default. This range can be configured by selecting the display with the select tool.

### PROPERTIES

- Mass: 2
- Dimensions (WxDxH): 1x2x2
- Cost: $20
- Tags: 
- File: gauge_display.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| number | Primary Display Value | The numerical value that sets the position of the white needle. |
| number | Secondary Display Value | The numerical value that sets the position of the red needle. |
| on/off | Backlight | Enables the backlight when receiving an on signal. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## HUD Large

A clear projection heads up display screen.

Displays video data.

### PROPERTIES

- Mass: 18
- Dimensions (WxDxH): 3x3x1
- Cost: $10000
- Tags: 
- File: monitor_hud_3.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| video | Video Signal |  |
| on/off | Power Switch | Controls whether or not the screen is switched on. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| composite | Touch Output |  |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric |  |

## HUD Small

A clear projection heads up display screen.

Displays video data.

### PROPERTIES

- Mass: 2
- Dimensions (WxDxH): 1x1x1
- Cost: $2000
- Tags: 
- File: monitor_hud_1.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| video | Video Signal |  |
| on/off | Power Switch | Controls whether or not the screen is switched on. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| composite | Touch Output |  |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric |  |

## Indicator Light

A simple light that can be used as an indicator in logic systems.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $20
- Tags: basic
- File: indicator.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Indicator Light | Switches the light on when receiving an on signal. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Indicator Light (RGB)

An advanced indicator that can be controlled using a microcontroller.

Three channels of the composite input can be used to set the red, green and blue components of the indicator's color using numbers between 0 and 1. The light can also operate in HSV mode, where the 3 inputs correspond to the hue, saturation and value (brightness) of the color between 0 and 1. The color mode and input channels can be customised by selecting this component with the select tool.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $50
- Tags: basic
- File: indicator_rgb.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| composite | Color Data | Composite link containing the indicator's color data. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Instrument Panel

A customisable panel that can have up to 4 different instruments, controlled by a composite signal from a microcontroller.

The 4 instruments can be selected in the properties window. Each type of instrument has options for choosing the composite channels that they read from or write to. Composite signals are bridged from the input node to the output node to enable displays to be chained together. Instruments marked as '(On/Off)' require multiple on/off signals to control each of their segments individually.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x2
- Cost: $200
- Tags: 
- File: instrument_display.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| composite | In Signal | Input signal containing data to be displayed. |
| on/off | Backlight | Enables the backlight when receiving an on signal. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| composite | Out Signal | Output signal containing data set by buttons on the display. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Laser Beacon

A beacon that produces a laser point light, visible by laser point sensors.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x2
- Cost: $5
- Tags: 
- File: laser_beacon.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Beacon Light | Switches the beacon on when receiving an on signal. |
| number | Wavelength | The specific light wavelength to emit (whole number). |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Monitor 1x1

A video screen.

Displays video data.

### PROPERTIES

- Mass: 4
- Dimensions (WxDxH): 1x1x1
- Cost: $500
- Tags: 
- File: monitor_1.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| video | Video Signal |  |
| on/off | Power Switch | Controls whether or not the screen is switched on. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| composite | Touch Output |  |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric |  |

## Monitor 1x2

A video screen.

Displays video data.

### PROPERTIES

- Mass: 8
- Dimensions (WxDxH): 2x1x1
- Cost: $1000
- Tags: 
- File: monitor_1x2.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| video | Video Signal |  |
| on/off | Power Switch | Controls whether or not the screen is switched on. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| composite | Touch Output |  |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric |  |

## Monitor 1x3

A video screen.

Displays video data.

### PROPERTIES

- Mass: 12
- Dimensions (WxDxH): 3x1x1
- Cost: $1500
- Tags: 
- File: monitor_1x3.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| video | Video Signal |  |
| on/off | Power Switch | Controls whether or not the screen is switched on. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| composite | Touch Output |  |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric |  |

## Monitor 2x2

A video screen.

Displays video data.

### PROPERTIES

- Mass: 16
- Dimensions (WxDxH): 2x2x1
- Cost: $2000
- Tags: 
- File: monitor_2.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| video | Video Signal |  |
| on/off | Power Switch | Controls whether or not the screen is switched on. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| composite | Touch Output |  |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric |  |

## Monitor 2x3

A video screen.

Displays video data.

### PROPERTIES

- Mass: 24
- Dimensions (WxDxH): 3x2x1
- Cost: $3000
- Tags: 
- File: monitor_2x3.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| video | Video Signal |  |
| on/off | Power Switch | Controls whether or not the screen is switched on. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| composite | Touch Output |  |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric |  |

## Monitor 3x3

A video screen.

Displays video data.

### PROPERTIES

- Mass: 36
- Dimensions (WxDxH): 3x3x1
- Cost: $4500
- Tags: 
- File: monitor_3.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| video | Video Signal |  |
| on/off | Power Switch | Controls whether or not the screen is switched on. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| composite | Touch Output |  |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric |  |

## Monitor 5x3

A video screen.

Displays video data.

### PROPERTIES

- Mass: 60
- Dimensions (WxDxH): 5x3x1
- Cost: $7500
- Tags: 
- File: monitor_5.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| video | Video Signal |  |
| on/off | Power Switch | Controls whether or not the screen is switched on. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| composite | Touch Output |  |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric |  |

## Monitor 9x5

A video screen.

Displays video data.

### PROPERTIES

- Mass: 180
- Dimensions (WxDxH): 9x5x1
- Cost: $20000
- Tags: 
- File: monitor_9.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| video | Video Signal |  |
| on/off | Power Switch | Controls whether or not the screen is switched on. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| composite | Touch Output |  |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric |  |

## Paintable Indicator

A backlit indicator for displaying painted detail.

This block has a paintable surface where small grid squares can be painted individually. Use additive painting mode to paint the backlight grid. The backlight can be enabled by using an on signal and a name can be set with the select tool that will be visible when the indicator is looked at by a player.

### PROPERTIES

- Mass: 2
- Dimensions (WxDxH): 1x1x1
- Cost: $100
- Tags: sign,basic
- File: sign.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Backlight | Switches the backlight on when receiving an on signal. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Paintable Sign

Sign block for displaying painted detail.

This block has a paintable surface where small grid squares can be painted individually.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $50
- Tags: basic
- File: sign_na.xml

## Speaker (Small)

A speaker capable of playing audio data to players within its range.

A small speaker capable of playing audio data to nearby players. (Range : 15)

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x2
- Cost: $250
- Tags: 
- File: speaker.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| audio | Audio | Audio data connection. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Is Transmit | If the speaker is currently transmitting. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |
