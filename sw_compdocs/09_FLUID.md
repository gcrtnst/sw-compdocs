# Fluid

## Air Filter

Port used to allow air in and out of a fluid system.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $50
- Tags: air
- File: air_filter.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Air | Allows fluid to flow in and out of an enclosed volume. |

## Air Ram

Port used to allow air in and out of a fluid system.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $50
- Tags: air
- File: modular_engine_air_ram.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Air | Allows fluid to flow in and out of an enclosed volume. |

## Air Scoop Intake 1x1

An air intake component.

An air intake component that performs better at higher velocity.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $30
- Tags: 
- File: scoop_intake_2.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Fluid | Air output port. |

## Air-Air Heat Exchanger 2x2

A heat exchanger that averages heat between two air systems.

A heat exchanger that averages heat between two air systems at a rate proportional to the component's size.

### PROPERTIES

- Mass: 4
- Dimensions (WxDxH): 2x2x1
- Cost: $30
- Tags: 
- File: heat_exchanger_2_2.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Temp A | Compartment temperature. |
| number | Temp B | Compartment temperature. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Air A In | Input air port. |
| fluid | Air A Out | Output air port. |
| fluid | Air B In | Input air port. |
| fluid | Air B Out | Output air port. |

## Air-Air Heat Exchanger 2x5

A heat exchanger that averages heat between two air systems.

A heat exchanger that averages heat between two air systems at a rate proportional to the component's size.

### PROPERTIES

- Mass: 10
- Dimensions (WxDxH): 2x5x5
- Cost: $70
- Tags: 
- File: heat_exchanger_5_5.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Temp A | Compartment temperature. |
| number | Temp B | Compartment temperature. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Air A In | Input air port. |
| fluid | Air A Out | Output air port. |
| fluid | Air B In | Input air port. |
| fluid | Air B Out | Output air port. |

## Air-Air Heat Exchanger 3x9

A heat exchanger that averages heat between two air systems.

A heat exchanger that averages heat between two air systems at a rate proportional to the component's size.

### PROPERTIES

- Mass: 27
- Dimensions (WxDxH): 3x9x9
- Cost: $100
- Tags: 
- File: heat_exchanger_9_9.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Temp A | Compartment temperature. |
| number | Temp B | Compartment temperature. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Air A In | Input air port. |
| fluid | Air A Out | Output air port. |
| fluid | Air B In | Input air port. |
| fluid | Air B Out | Output air port. |

## Air-Liquid Heat Exchanger 1x2

A heat exchanger that averages heat between air and a liquid.

An intercooler that averages heat between air and a liquid at a rate proportional to the component's size.

### PROPERTIES

- Mass: 2
- Dimensions (WxDxH): 1x2x1
- Cost: $15
- Tags: 
- File: air_exchanger.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Temp A | Compartment air temperature. |
| number | Temp B | Compartment water temperature. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Air In | Input air port. |
| fluid | Air Out | Output air port. |
| fluid | Fluid In | Input fluid port. |
| fluid | Fluid Out | Output fluid port. |

## Air-Liquid Heat Exchanger 5x2

A heat exchanger that averages heat between air and a liquid.

An intercooler that averages heat between air and a liquid at a rate proportional to the component's size.

### PROPERTIES

- Mass: 7
- Dimensions (WxDxH): 1x5x2
- Cost: $30
- Tags: 
- File: air_exchanger_5_2.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Temp A | Compartment air temperature. |
| number | Temp B | Compartment water temperature. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Air In | Input air port. |
| fluid | Air Out | Output air port. |
| fluid | Fluid In | Input fluid port. |
| fluid | Fluid Out | Output fluid port. |

## Air-Liquid Heat Exchanger 5x3

A heat exchanger that averages heat between air and a liquid.

An intercooler that averages heat between air and a liquid at a rate proportional to the component's size.

### PROPERTIES

- Mass: 45
- Dimensions (WxDxH): 3x5x3
- Cost: $50
- Tags: 
- File: air_exchanger_5_3.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Temp A | Compartment air temperature. |
| number | Temp B | Compartment water temperature. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Air In | Input air port. |
| fluid | Air Out | Output air port. |
| fluid | Fluid In |  Input fluid port. |
| fluid | Fluid Out | Output fluid port. |

## Air-Liquid Heat Exchanger 9x3

A heat exchanger that averages heat between air and a liquid.

An intercooler that averages heat between air and a liquid at a rate proportional to the component's size.

### PROPERTIES

- Mass: 81
- Dimensions (WxDxH): 3x9x3
- Cost: $80
- Tags: 
- File: air_exchanger_9_3.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Temp A | Compartment air temperature. |
| number | Temp B | Compartment water temperature. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Air In | Input air port. |
| fluid | Air Out | Output air port. |
| fluid | Fluid In | Input fluid port. |
| fluid | Fluid Out | Output fluid port. |

## Air-Liquid Heat Exchanger 9x5

A heat exchanger that averages heat between air and a liquid.

An intercooler that averages heat between air and a liquid at a rate proportional to the component's size.

### PROPERTIES

- Mass: 225
- Dimensions (WxDxH): 5x9x5
- Cost: $150
- Tags: 
- File: air_exchanger_9_5.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Temp A | Compartment air temperature. |
| number | Temp B | Compartment water temperature. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Air In | Input air port. |
| fluid | Air Out | Output air port. |
| fluid | Fluid In | Input fluid port. |
| fluid | Fluid Out | Output fluid port. |

## Catalytic Converter

Reduces particles from exhausts.

Catalytic converter that removes fumes and decreases the number of exhaust particles emitted from an exhaust.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $100
- Tags: 
- File: catalytic_converter.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Exhaust In |  |
| fluid | Exhaust Out |  |

## Centrifugal Separator

A tank that can be spun to separate contained fluids.

Provide torque to begin spinning the separator, fluid output ports will separate with increased effectiveness based on the spin speed.

### PROPERTIES

- Mass: 80
- Dimensions (WxDxH): 5x5x9
- Cost: $480
- Tags: oil
- File: separator.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| power | RPS | RPS input node for spinning the centrifuge. |
| fluid | Fluid In | Input fluid port. |
| fluid | Fluid Out | Main output fluid port. |
| fluid | Dense Fluid Out | Output port that will filter the denser fluid when the centrifuge is operating at high speed. |

## Desalinator

A pipe that slowly converts seawater to freshwater.

A pipe with a fine desalination filter that slowly converts seawater to freshwater and allows free flow of freshwater.

### PROPERTIES

- Mass: 5
- Dimensions (WxDxH): 1x1x5
- Cost: $400
- Tags: basic
- File: desalinator.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Fluid In | Seawater connection. |
| fluid | Fluid Out | Freshwater connection. |

## Fluid Exhaust

An exhaust port for fluid systems.

Fluid can flow in and out of the port as part of a fluid system.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x2
- Cost: $100
- Tags: basic
- File: fluid_exhaust.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Fluid | Allows fluid to flow in and out of an enclosed volume or the ocean. |

## Fluid Filter

> [!WARNING]
> This component is deprecated.

The fluid filter can prevent liquids or gases crossing the valve.

The valve can be configured to select which fluid groups may pass across the two directional valve. Liquids or gases.

### PROPERTIES

- Mass: 5
- Dimensions (WxDxH): 1x1x2
- Cost: $400
- Tags: basic
- File: fluid_filter_v2.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Fluid A | Fluid connection. |
| fluid | Fluid B | Fluid connection. |

## Fluid Filter (Deprecated)

> [!WARNING]
> This component is deprecated.

The fluid filter only allows certain types of fluid across the valve.

The valve can be configured to select which fluids may pass across the two directional valve.

### PROPERTIES

- Mass: 5
- Dimensions (WxDxH): 1x1x2
- Cost: $400
- Tags: basic
- File: fluid_filter.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Flow Rate | Fluid flow rate in L/s. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Fluid A | Fluid connection. |
| fluid | Fluid B | Fluid connection. |

## Fluid Flow Valve

A one way valve for controlling fluid flow.

Allows fluid to move from the input side of the valve to the output but resists fluid flow in the other direction.

### PROPERTIES

- Mass: 4
- Dimensions (WxDxH): 1x1x2
- Cost: $100
- Tags: basic
- File: fluid_valve_flow.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Flow Rate | Fluid flow rate in L/s. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Fluid In | Fluid connection for the valve input. |
| fluid | Fluid Out | Fluid connection for the valve output. |

## Fluid Heat Radiator

Radiator type cooler for fluid.

Fluid inside the cooler will lose temperature.

### PROPERTIES

- Mass: 10
- Dimensions (WxDxH): 3x1x3
- Cost: $200
- Tags: basic
- File: fluid_radiator.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Fluid A | Fluid Connection. |
| fluid | Fluid B | Fluid Connection. |

## Fluid Heat Radiator 3x3 (Electric)

Radiator type cooler for fluid.

Fluid inside the cooler will lose temperature, supplying electric for the fan will increase the rate of exchange.

### PROPERTIES

- Mass: 10
- Dimensions (WxDxH): 3x3x1
- Cost: $400
- Tags: 
- File: fluid_radiator_electric.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Fan On/Off |  |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Temperature |  |

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Fluid A | Fluid Connection. |
| fluid | Fluid B | Fluid Connection. |
| electric | Electric |  |

## Fluid Heat Radiator 5x5 (Electric)

Radiator type cooler for fluid.

Fluid inside the cooler will lose temperature, supplying electric for the fan will increase the rate of exchange.

### PROPERTIES

- Mass: 25
- Dimensions (WxDxH): 5x5x1
- Cost: $700
- Tags: 
- File: fluid_radiator_electric_5.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Fan On/Off |  |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Temperature |  |

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Fluid A | Fluid Connection. |
| fluid | Fluid B | Fluid Connection. |
| electric | Electric |  |

## Fluid Heat Sink

Heat sink type cooler for fluid.

Fluid inside the cooler will lose temperature.

### PROPERTIES

- Mass: 18
- Dimensions (WxDxH): 5x1x3
- Cost: $300
- Tags: 
- File: fluid_heat_sink.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Fluid A | Fluid Connection. |
| fluid | Fluid B | Fluid Connection. |

## Fluid Intake

Port used to allow fluid in and out of a fluid system.

Place the port inside of an enclosed volume to connect to that volume, or outside of the vehicle to connect to the exterior.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 3x1x2
- Cost: $100
- Tags: air
- File: fluid_intake.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Fluid | Allows fluid to flow in and out of an enclosed volume or the exterior. |

## Fluid Jet

A fluid impeller and jet nozzle for ocean propulsion.

Converts mechanical power and water into a high power jet for generating thrust.

### PROPERTIES

- Mass: 10
- Dimensions (WxDxH): 3x3x7
- Cost: $3000
- Tags: basic
- File: water_jet.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| number | Vertical Trim | Vertical nozzle angle to control jet direction. |
| number | Deflector A | Left bucket defector control input. |
| number | Deflector B | Right bucket defector control input. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Fluid Flow In | Fluid inlet to supply jet. |
| power | RPS | Mechanical power input to power jet. |
| electric | Electric | Electrical power connection. |

## Fluid On/Off Valve

An on/off fluid valve.

Controls flow from one side of the valve to the other. Fluid can flow in both directions.

### PROPERTIES

- Mass: 4
- Dimensions (WxDxH): 2x1x2
- Cost: $100
- Tags: basic
- File: fluid_valve_on_off.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Valve Control | Valve gate control for opening and closing the valve. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Flow Rate | Fluid flow rate in L/s. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Fluid In | Fluid input connection for the valve. |
| fluid | Fluid Out | Fluid output connection for the valve. |
| electric | Electric | Electrical power connection. |

## Fluid On/Off Valve (Manual)

An on/off fluid valve with a manual handle.

Interacting with [q]/[e] will open / close the valve. Controls flow from one side of the valve to the other. Fluid can flow in both directions.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $100
- Tags: basic
- File: fluid_valve_on_off_manual.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Flow Rate | Fluid flow rate in L/s. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Fluid In | Fluid input connection for the valve. |
| fluid | Fluid Out | Fluid output connection for the valve. |

## Fluid Port

Port used to allow fluid in and out of a fluid system.

Place the port inside of an enclosed volume to connect to that volume, or outside of the vehicle to connect to the ocean.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x2
- Cost: $50
- Tags: air,basic
- File: water_inlet.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Fluid | Allows fluid to flow in and out of an enclosed volume or the ocean. |

## Fluid Port (Deprecated)

> [!WARNING]
> This component is deprecated.

Port used to allow fluid in and out of a fluid system.

Place the port inside of an enclosed volume to connect to that volume, or outside of the vehicle to connect to the ocean.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x2
- Cost: $50
- Tags: pump
- File: water_outlet.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Fluid | Allows fluid to flow in and out of an enclosed volume or the ocean. |

## Fluid Port End

Port used to allow fluid in and out of a fluid system.

Place the port inside of an enclosed volume to connect to that volume, or outside of the vehicle to connect to the ocean.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $50
- Tags: air,basic
- File: fluid_port_end.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Fluid | Allows fluid to flow in and out of an enclosed volume or the ocean. |

## Fluid Pressure Sensor

A sensor for reading fluid pressure.

Measures the fluid pressure in the connected fluid network.

### PROPERTIES

- Mass: 4
- Dimensions (WxDxH): 1x1x2
- Cost: $100
- Tags: 
- File: fluid_pressure.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Pressure | The pressure reading of the fluid. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Fluid | Fluid to measure the pressure of. |

## Fluid Pump

A small fluid pump.

Connect to an inlet and outlet to create a pumping system to move fluid around a vehicle.

### PROPERTIES

- Mass: 4
- Dimensions (WxDxH): 3x1x1
- Cost: $100
- Tags: basic
- File: water_pump.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | On/Off | Controls whether or not the fluid is being pumped through. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Flow Rate | Fluid flow rate in L/s. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Fluid In | Connect to an inlet component to take fluid into the system. |
| fluid | Fluid Out | Connect to an outlet component to release fluid from the system. |
| electric | Electric | Electrical power connection. |

## Fluid Pump (Manual)

A small fluid pump with a manual handle.

Hold [q]/[e] to create pressure in the pump. Connect to an inlet and outlet to create a pumping system to move fluid around a vehicle.

### PROPERTIES

- Mass: 4
- Dimensions (WxDxH): 2x1x3
- Cost: $100
- Tags: basic
- File: water_pump_manual.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Flow Rate | Fluid flow rate in L/s. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Fluid In | Connect to an inlet component to take fluid into the system. |
| fluid | Fluid Out | Connect to an outlet component to release fluid from the system. |

## Fluid Slot Port

Port used to allow fluid in and out of a fluid system.

Place the port inside of an enclosed volume to connect to that volume, or outside of the vehicle to connect to the ocean.

### PROPERTIES

- Mass: 12
- Dimensions (WxDxH): 3x4x2
- Cost: $100
- Tags: basic
- File: water_suction_duct.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Fluid | Allows fluid to flow in and out of an enclosed volume or the ocean. |

## Fluid Spawner

A component to mark an enclosed area to be spawned with fluid inside.

The fluid spawner for helping with custom fluid tanks, so they can be spawned full, without a need to fill after spawning. Gases are spawned compressed (60atm).

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x2
- Cost: $20
- Tags: basic
- File: water_spawner.xml

## Fluid Tank Large

A tank for storing fluid.

The tank will spawn full of the selected fluid type.

### PROPERTIES

- Mass: 22
- Dimensions (WxDxH): 3x5x3
- Cost: $20
- Tags: basic
- File: fluid_tank_large.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Tank Content | The amount of fluid in the tank in litres. |
| number | Tank Pressure | The pressure in the tank in atmospheres. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Stored Fluid | The fluid connection for the stored contents. |
| fluid | Stored Fluid | The fluid connection for the stored contents. |

## Fluid Tank Medium

A tank for storing fluid.

The tank will spawn full of the selected fluid type.

### PROPERTIES

- Mass: 6
- Dimensions (WxDxH): 2x3x2
- Cost: $20
- Tags: basic
- File: fluid_tank_medium.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Tank Content | The amount of fluid in the tank in litres. |
| number | Tank Pressure | The pressure in the tank in atmospheres. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Stored Fluid | The fluid connection for the stored contents. |
| fluid | Stored Fluid | The fluid connection for the stored contents. |

## Fluid Tank Small

A tank for storing fluid.

The tank will spawn full of the selected fluid type.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x2x1
- Cost: $20
- Tags: basic
- File: fluid_tank_small.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Tank Content | The amount of fluid in the tank in litres. |
| number | Tank Pressure | The pressure in the tank in atmospheres. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Stored Fluid | The fluid connection for the stored contents. |
| fluid | Stored Fluid | The fluid connection for the stored contents. |

## Fluid Variable Valve

A variable fluid valve.

Controls flow from one side of the valve to the other. Fluid can flow in both directions.

### PROPERTIES

- Mass: 4
- Dimensions (WxDxH): 2x1x2
- Cost: $100
- Tags: basic
- File: fluid_valve_variable.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| number | Valve Control | Valve gate control for opening and closing the valve. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Flow Rate | Fluid flow rate in L/s. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Fluid In | Fluid input connection for the valve. |
| fluid | Fluid Out | Fluid output connection for the valve. |
| electric | Electric | Electrical power connection. |

## Fractional Distillation Port

Port used to collect output in a distillation column.

Place the port inside of an enclosed volume to connect to that volume. Outputs different fluids based on height relative to the bottom of the compartment.

### PROPERTIES

- Mass: 36
- Dimensions (WxDxH): 3x3x5
- Cost: $80
- Tags: oil,refining,refine
- File: distillation_tray.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Fluid | Collects distilled fluids from an enclosed volume. |

## Gas Relief Valve

A relief valve for gases in a system.

The valve allows gases to pass across the two directional valve.

### PROPERTIES

- Mass: 2
- Dimensions (WxDxH): 1x1x1
- Cost: $150
- Tags: basic,fluid,filter
- File: relief_valve_gas.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Flow Rate | Fluid flow rate in L/s. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Fluid A |  |
| fluid | Fluid B |  |

## Gas Tank (Huge)

A tank for storing gas.

The tank will spawn full of the selected fluid type.

### PROPERTIES

- Mass: 22
- Dimensions (WxDxH): 5x5x9
- Cost: $20
- Tags: fluid
- File: fluid_tank_compressed_gas_5_9.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Tank Content | The amount of gas in the tank in litres. |
| number | Tank Pressure | The pressure in the tank in atmospheres. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Stored Gas | The fluid connection for the stored contents. |

## Gas Tank (Large)

A tank for storing gas.

The tank will spawn full of the selected fluid type.

### PROPERTIES

- Mass: 12
- Dimensions (WxDxH): 3x3x7
- Cost: $20
- Tags: fluid
- File: fluid_tank_compressed_gas_3_7.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Tank Content | The amount of gas in the tank in litres. |
| number | Tank Pressure | The pressure in the tank in atmospheres. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Stored Gas | The fluid connection for the stored contents. |

## Gas Tank (Medium)

A tank for storing gas.

The tank will spawn full of the selected fluid type.

### PROPERTIES

- Mass: 5
- Dimensions (WxDxH): 1x1x7
- Cost: $20
- Tags: fluid
- File: fluid_tank_compressed_gas_1_7.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Tank Content | The amount of fluid in the tank in litres. |
| number | Tank Pressure | The pressure in the tank in atmospheres. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Stored Gas | The fluid connection for the stored contents. |

## Gas Tank (Small)

A tank for storing gas.

The tank will spawn full of the selected fluid type.

### PROPERTIES

- Mass: 2
- Dimensions (WxDxH): 1x1x3
- Cost: $20
- Tags: fluid
- File: fluid_tank_compressed_gas_1_3.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Tank Content | The amount of gas in the tank in litres. |
| number | Tank Pressure | The pressure in the tank in atmospheres. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Stored Gas | The fluid connection for the stored contents. |

## Hydrogen Electrolyser

A machine that separates water into hydrogen and oxygen.

Submerge the electrodes into a volume of water and provide electric to separate freshwater.

### PROPERTIES

- Mass: 16
- Dimensions (WxDxH): 1x3x6
- Cost: $575
- Tags: 
- File: electrolyser.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Enable |  |

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Oxygen Out |  |
| fluid | Hydrogen Out |  |
| electric | Electric |  |

## Impeller Pump

An Impeller Pump that can push fluid through a system.

An Impeller that will force fluid through the system when torque is applied.

### PROPERTIES

- Mass: 9
- Dimensions (WxDxH): 3x3x1
- Cost: $50
- Tags: 
- File: turbocharger.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Flow Rate | Fluid flow rate in L/s. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Fluid In |  |
| power | RPS |  |
| fluid | Fluid Out |  |

## Impeller Pump (Small)

An Impeller Pump that can push fluid through a system.

An Impeller that will force fluid through the system when torque is applied.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $40
- Tags: 
- File: turbocharger_small.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Flow Rate | Fluid flow rate in L/s. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Fluid In |  |
| power | RPS |  |
| fluid | Fluid Out |  |

## Large Fluid Pump

A large fluid pump.

Connect to an inlet and outlet to create a pumping system to move fluid around a vehicle.

### PROPERTIES

- Mass: 10
- Dimensions (WxDxH): 2x2x2
- Cost: $200
- Tags: basic
- File: water_pump_large.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | On/Off | Controls whether or not the fluid is being pumped. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Flow Rate | Fluid flow rate in L/s. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Fluid In | Connect to an inlet component to take fluid into the system. |
| fluid | Fluid Out | Connect to an outlet component to release fluid from the system. |
| electric | Electric | Electrical power connection. |

## Liquid Relief Valve

A relief valve for liquids in a system.

The valve allows liquids to pass across the two directional valve.

### PROPERTIES

- Mass: 2
- Dimensions (WxDxH): 1x1x1
- Cost: $150
- Tags: basic,fluid,filter
- File: relief_valve_liquid.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Flow Rate | Fluid flow rate in L/s. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Fluid A |  |
| fluid | Fluid B |  |

## Liquid-Liquid Heat Exchanger 2x2

A heat exchanger that averages heat between two liquid systems.

A heat exchanger that averages heat between two liquid systems at a rate proportional to the component's size.

### PROPERTIES

- Mass: 4
- Dimensions (WxDxH): 1x2x2
- Cost: $30
- Tags: 
- File: intercooler.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Temp A | Compartment temperature. |
| number | Temp B | Compartment temperature. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Fluid A In | Input fluid port. |
| fluid | Fluid A Out | Output fluid port. |
| fluid | Fluid B In | Input fluid port. |
| fluid | Fluid B Out | Output fluid port. |

## Liquid-Liquid Heat Exchanger 5x5

A heat exchanger that averages heat between two liquid systems.

A heat exchanger that averages heat between two liquid systems at a rate proportional to the component's size.

### PROPERTIES

- Mass: 16
- Dimensions (WxDxH): 1x5x5
- Cost: $50
- Tags: 
- File: intercooler_large.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Temp A | Compartment temperature. |
| number | Temp B | Compartment temperature. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Fluid A In | Input fluid port. |
| fluid | Fluid A Out | Output fluid port. |
| fluid | Fluid B In | Input fluid port. |
| fluid | Fluid B Out | Output fluid port. |

## Slurry Filter

A filter that slowly desaturates slurry.

A pipe with a solids filter that consumes fresh water to slowly convert saturated slurry to slurry and allows free flow of slurry.

### PROPERTIES

- Mass: 140
- Dimensions (WxDxH): 5x9x15
- Cost: $320
- Tags: 
- File: slurry_filter.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Water In | Water Input. |
| fluid | Water Out | Water Output. |
| fluid | Slurry In | Saturated Slurry input. |
| fluid | Slurry Out | Slurry output. |

## Steam Whistle

A steam powered signal whistle.

When open, the steam whistle produces sound as steam flows through the pipe connection. The whistle pitch can be set in the component properties menu.

### PROPERTIES

- Mass: 4
- Dimensions (WxDxH): 1x1x4
- Cost: $50
- Tags: steam power
- File: steam_whistle.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Open | Opens the steam whistle, allowing steam to flow through. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Fluid | Allows steam to flow out. |
