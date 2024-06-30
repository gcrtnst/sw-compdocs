# Electric

## Electric Battery Large

A large battery array for storing electrical charge.

### PROPERTIES

- Mass: 800
- Dimensions (WxDxH): 7x5x5
- Cost: $10000
- Tags: basic
- File: battery_large.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Charge | Data output giving the charge of the battery from 0 to 1. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric Store | Energy storage for the electrical system. |

## Electric Battery Medium

A medium battery for storing electrical charge.

### PROPERTIES

- Mass: 60
- Dimensions (WxDxH): 3x2x2
- Cost: $1200
- Tags: basic
- File: battery_medium.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Charge | Data output giving the charge of the battery from 0 to 1. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric Store | Energy storage for the electrical system. |

## Electric Battery Small

A small battery for storing electrical charge.

### PROPERTIES

- Mass: 10
- Dimensions (WxDxH): 2x1x1
- Cost: $150
- Tags: basic
- File: battery_small.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Charge | Data output giving the charge of the battery from 0 to 1. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric Store | Energy storage for the electrical system. |

## Electric Charger

A one-way charger.

The charger transfers electric one-way between its nodes when there is a significant discrepancy in charge. It can be used to recharge batteries.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x2x1
- Cost: $100
- Tags: 
- File: electric_diode.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric In | Input node for electric. |
| electric | Electric Out | Output node for electric. |

## Electric Circuit Breaker

A circuit breaker for electrical systems.

When turned on, the circuit breaker closes the circuit, allowing electrical energy to flow between terminals A and B.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x2
- Cost: $100
- Tags: basic
- File: electric_curcuit_breaker.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric A | Terminal A electrical connection. |
| electric | Electric B | Terminal B electrical connection. |

## Electric Relay

A relay for electrical systems.

When turned on, the relay closes the circuit, allowing electrical energy to flow between terminals A and B.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 3x1x1
- Cost: $100
- Tags: basic
- File: electric_relay.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Relay State | Input to set if the electrical connection is made. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric A | Terminal A electrical connection. |
| electric | Electric B | Terminal B electrical connection. |

## Large Generator

A large generator unit for converting mechanical power to electricity.

### PROPERTIES

- Mass: 400
- Dimensions (WxDxH): 5x5x5
- Cost: $12000
- Tags: basic
- File: generator_large.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Output | Data output giving the electrical generation of the generator. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| power | RPS | The torque power input to convert to electric energy. |
| electric | Electric | The electric connection to output electric energy. |

## Large Solar Cell

A large solar cell for generating electricity.

The cell generates electrical current based on time of day and angle towards the sun.

### PROPERTIES

- Mass: 40
- Dimensions (WxDxH): 5x5x1
- Cost: $8000
- Tags: basic
- File: solar_large.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | The electric connection to output electric energy. |

## Medium Generator

A medium generator unit for converting mechanical power to electricity.

### PROPERTIES

- Mass: 100
- Dimensions (WxDxH): 3x3x3
- Cost: $2000
- Tags: basic
- File: generator_medium.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Output | Data output giving the electrical generation of the generator. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| power | RPS | The torque power input to convert to electric energy. |
| electric | Electric | The electric connection to output electric energy. |

## Small Generator

A small generator unit for converting mechanical power to electricity.

### PROPERTIES

- Mass: 5
- Dimensions (WxDxH): 1x1x1
- Cost: $600
- Tags: basic
- File: generator_small.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Output | Data output giving the electrical generation of the generator. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| power | RPS | The torque power input to convert to electric energy. |
| electric | Electric | The electric connection to output electric energy. |

## Solar Cell

A solar cell for generating electricity.

The cell generates electrical current based on time of day and angle towards the sun.

### PROPERTIES

- Mass: 2
- Dimensions (WxDxH): 1x1x1
- Cost: $400
- Tags: basic
- File: solar.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | The electric connection to output electric energy. |
