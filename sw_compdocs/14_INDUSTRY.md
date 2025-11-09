# Industry

## Duct

A basic resource duct.

Transports resources through the connected system.

### PROPERTIES

- Mass: 12
- Dimensions (WxDxH): 3x3x3
- Cost: $50
- Tags: steam,coal,fishing
- File: steam_coal_duct.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Fill Level |  |

## Duct Large

A basic resource duct.

Transports resources through the connected system.

### PROPERTIES

- Mass: 112
- Dimensions (WxDxH): 5x9x5
- Cost: $150
- Tags: steam,coal,fishing
- File: steam_coal_duct_l.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Fill Level |  |

## Duct Medium

A basic resource duct.

Transports resources through the connected system.

### PROPERTIES

- Mass: 62
- Dimensions (WxDxH): 5x5x5
- Cost: $100
- Tags: steam,coal,fishing
- File: steam_coal_duct_m.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Fill Level |  |

## Electric Furnace

An electrically powered furnace.

Produces large amounts of heat from electricity.

### PROPERTIES

- Mass: 220
- Dimensions (WxDxH): 3x3x5
- Cost: $900
- Tags: firebox
- File: furnace_electric.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Enable | Activate the electric furnace. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Temperature | Temperature of the coolant that is being heated. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Coolant In | In port for fluid to be heated by the furnace. |
| fluid | Coolant Out | Out port for fluid to be heated by the furnace. |
| electric | Electric | Electrical power connection. |

## Firebox

A coal powered firebox.

Produces large amounts of heat. Can be supplied with a mineral duct. Consumes 1 coal to ignite the fire.

### PROPERTIES

- Mass: 100
- Dimensions (WxDxH): 3x5x3
- Cost: $100
- Tags: steam,coal
- File: steam_coal_firebox.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Ignition | Activate to consume a coal and ignite the firebox. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Coal Level |  |
| number | Temperature | Temperature of the coolant that is being heated. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Coolant In | In port for fluid to be heated by the firebox. |
| fluid | Coolant Out | Out port for fluid to be heated by the firebox. |
| fluid | Air | Port for supplying air to the fire. |
| fluid | Exhaust | Port for removing exhaust from burnt coal. |

## Firebox Large

A coal powered firebox.

Produces large amounts of heat. Can be supplied with a duct. Consumes 1 coal to ignite the fire.

### PROPERTIES

- Mass: 400
- Dimensions (WxDxH): 5x7x5
- Cost: $200
- Tags: steam,coal
- File: steam_coal_firebox_l.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Ignition | Activate to consume a coal and ignite the firebox. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Coal Level |  |
| number | Temperature | Temperature of the coolant that is being heated. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Coolant In | In port for fluid to be heated by the firebox. |
| fluid | Coolant Out | Out port for fluid to be heated by the firebox. |
| fluid | Air | Port for supplying air to the fire. |
| fluid | Exhaust | Port for removing exhaust from burnt coal. |

## Flexible Duct

A flexible resource duct.

Transports resources through the connected system. Flexible ducts can be connected together by rope nodes to transfer resources.

### PROPERTIES

- Mass: 20
- Dimensions (WxDxH): 3x3x2
- Cost: $50
- Tags: steam,coal,fishing
- File: steam_coal_flex.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| rope | Duct |  |

## Funnel Duct

A funnel for moving resources.

Can be toggled to slowly move resources out of the connected system.

### PROPERTIES

- Mass: 20
- Dimensions (WxDxH): 3x3x2
- Cost: $50
- Tags: steam,coal,fishing
- File: steam_coal_funnel.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Open |  |

## Hopper

A hopper that can accept bulk minerals, ingots, and fish.

Pouring resources into the receptacle will add it to the connected system.

### PROPERTIES

- Mass: 12
- Dimensions (WxDxH): 3x3x3
- Cost: $50
- Tags: steam,coal,fishing
- File: steam_coal_hopper.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Fill Level |  |

## Hopper Large

A hopper that can accept bulk minerals, ingots, and fish.

Pouring resources into the receptacle will add it to the connected system.

### PROPERTIES

- Mass: 112
- Dimensions (WxDxH): 5x9x5
- Cost: $150
- Tags: steam,coal,fishing
- File: steam_coal_hopper_l.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Fill Level |  |

## Hopper Medium

A hopper that can accept bulk minerals, ingots, and fish.

Pouring resources into the receptacle will add it to the connected system.

### PROPERTIES

- Mass: 62
- Dimensions (WxDxH): 5x5x5
- Cost: $100
- Tags: steam,coal,fishing
- File: steam_coal_hopper_m.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Fill Level |  |

## Industrial Diesel Furnace

A diesel powered furnace.

Produces large amounts of heat by burning supplied diesel. Consumes a portion of the diesel reserve to ignite the fire.

### PROPERTIES

- Mass: 350
- Dimensions (WxDxH): 5x7x5
- Cost: $750
- Tags: firebox
- File: furnace_industrial.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Ignition | Activate to consume diesel and ignite the furnace. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Diesel Level |  |
| number | Temperature | Temperature of the coolant that is being heated. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Coolant In | In port for fluid to be heated by the furnace. |
| fluid | Coolant Out | Out port for fluid to be heated by the furnace. |
| fluid | Air In | Port for supplying air. |
| fluid | Exhaust Out | Port for removing exhaust from the furnace. |
| fluid | Diesel In | Port for supplying diesel fuel. |

## Lobster Pot

A trap for lobsters and crabs.

A portable trap for catching lobsters and crabs on the sea floor.

### PROPERTIES

- Mass: 45
- Dimensions (WxDxH): 5x5x3
- Cost: $150
- Tags: crab,fishing
- File: lobster_pot.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Release | When on, releases captured crabs and lobsters. When off, keeps them contained. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Fill Level |  |

## Net Anchor

An anchor point for a fishing net.

Draw a rope logic link between four Net Anchors in a loop to form a net.

### PROPERTIES

- Mass: 3
- Dimensions (WxDxH): 1x1x3
- Cost: $15
- Tags: basic,fishing
- File: rope_hook_net.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Release Catch |  |
| on/off | Extend |  |
| on/off | Retract |  |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| composite | Net Data | Outputs attached net data. Value 1: net fill level, Value 2: net extend factor. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| rope | Net Node |  |

## Nuclear Control Rod

A Control Rod.

Can be inserted into a fuel assembly to decrease the rate of reaction of adjacent rods.

### PROPERTIES

- Mass: 100
- Dimensions (WxDxH): 1x1x17
- Cost: $250
- Tags: reactor
- File: steam_nuclear_control_rod.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| number | Insertion Target |  |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Insertion |  |

## Nuclear Fuel Assembly

A Fuel assembly powered by uranium ingots.

A fuel rod can be inserted into the assembly to facilitate a fission reaction. Fuel rods consume uranium ingots from the workbench inventory to fuel.

### PROPERTIES

- Mass: 80
- Dimensions (WxDxH): 1x1x12
- Cost: $500
- Tags: reactor
- File: steam_nuclear_fuel_assembly.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Release Fuel Rod |  |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Fuel Rod Temperature |  |

## Nuclear Fuel Rod

A Radioactive Fuel Rod.

Can be inserted into a fuel assembly to start the nuclear fission process.

### PROPERTIES

- Mass: 80
- Dimensions (WxDxH): 1x1x9
- Cost: $2500
- Tags: reactor
- File: steam_nuclear_fuel_rod.xml

## Oil Rig Drill Clamp

A clamp for moving drill rods into place.

### PROPERTIES

- Mass: 30
- Dimensions (WxDxH): 3x3x2
- Cost: $100
- Tags: 
- File: oil_rig_drill_grabber.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Clamp Rod | Attach a drill rod to the clamp. |
| number | Slider Velocity | Slides an attached drill rod up or down the clamp. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Rod Clamped | Returns true when a drill rod is attached. |

## Oil Rig Drill Clamp (End)

A clamp for moving drill rods into place.

### PROPERTIES

- Mass: 5
- Dimensions (WxDxH): 1x1x2
- Cost: $500
- Tags: 
- File: oil_rig_drill_grabber_end.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Clamp Rod | Attach a drill rod to the clamp. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Rod Clamped | Returns true when a drill rod is attached. |

## Oil Rig Drill Connector

A clamp for moving drill rods into place.

It can connect drill rods together to lengthen them, or separate drill rods to shorten them.

### PROPERTIES

- Mass: 50
- Dimensions (WxDxH): 3x7x2
- Cost: $100
- Tags: 
- File: oil_rig_drill_connector.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Clamp Rod | Attach a drill rod to the clamp. |
| number | Slider Velocity | Moves an attached drill rod up or down the clamp. |
| on/off | Connect/Disconnect | Connects or disconnects a pair of drill rods when the ends are aligned at the connection point. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Rod Clamped | Returns true when a drill rod is attached. |
| on/off | Connector Aligned | Returns true when the connection point aligns over the end of a pair of drill rods. |

## Oil Rig Drill Swivel

A swivel for transferring fluids through a drill rod.

The swivel connects to the end of a drill rod, and has fluid ports for drilling slurry and crude oil. Pumping a supply of drilling slurry through a drill rod is required for effective drilling.

### PROPERTIES

- Mass: 30
- Dimensions (WxDxH): 3x3x5
- Cost: $1000
- Tags: 
- File: oil_rig_drill_swivel.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Clamp Rod | Attach a drill rod to the swivel. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Rod Clamped | Returns true when a drill rod is attached. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Fluid In | Fluid port to transfer drilling slurry through an attached rod linked to a well. |
| fluid | Fluid Out | Fluid port to transfer drilling slurry from an attached rod linked to a well. |

## Oil Rig Pumpjack

A pumpjack for extracting crude oil from a drilled oil well.

Pulling the piston of the pumpjack with enough force will lift the piston, pulling fluid through the pump. A mechanical force capable of repeatedly cycling the piston is required to pump fluid effectively.

### PROPERTIES

- Mass: 700
  - Parent Mass: 200
  - Child Mass: 500
- Dimensions (WxDxH): 3x3x21
  - Parent Dimensions (WxDxH): 3x3x11
  - Child Dimensions (WxDxH): 1x1x10
- Cost: $1000
- Tags: 
- Parent File: oil_rig_pumpjack.xml
- Child File: oil_rig_pumpjack_b.xml

### connections

| Body | Type | Label | Description |
| --- | --- | --- | --- |
| Parent | fluid | Fluid Out |  |

## Oil Rig Rod Storage

A storage rack for drill rods.

Contains a single drill rod when spawned.

### PROPERTIES

- Mass: 10
- Dimensions (WxDxH): 1x41x2
- Cost: $50
- Tags: 
- File: oil_rig_drill_storage.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Rod Stored | Returns true when a drill rod is stored in the component. |

## Oil Rig Rotary Table

A rotary table for drilling in an oil rig.

Torque provided by an external motor rotates the table, which can rotate a drill rod placed through the center of the table.

### PROPERTIES

- Mass: 500
- Dimensions (WxDxH): 7x7x3
- Cost: $1000
- Tags: 
- File: oil_rig_drill_driver.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Clamp | Attach a drill rod to the table. This will transfer any rotation of the table to the attached drill rod. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | RPS | The rotations per second of the table. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| power | Torque | Torque connection to power the rotation of the table. |

## Oil Rig Well Head

A well head for oil drilling.

Once anchored to the terrain, a drill rod can be inserted into a well head to begin drilling a well. In order to drill effectively a drill rod should be driven by a rotary table and forced downward toward the terrain. A continuous supply of drilling slurry must be provided through the drill rod via a swivel, and the saturated drilling slurry extracted from the well head fluid port.

### PROPERTIES

- Mass: 1000
- Dimensions (WxDxH): 9x9x25
- Cost: $5000
- Tags: 
- File: oil_rig_well_head.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Anchor | Extend / retract piles to anchor the well head to the terrain, allowing for a new well to be drilled. The well head must be close to the terrain (~1m) and upright (+-30 degrees) to be anchored. Unanchoring the well will reset any drilling progress made. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Is Anchored | Returns true when the well head is anchored to the terrain. |
| number | Drill Depth | Returns the depth of an attached drill rod in meters. |
| number | Well Depth | Returns the depth of the drilled well in meters. |

## Steam Boiler

A boiler for evaporating water into steam.

The boiler should be connected to a firebox to supply heat for evaporation. Control the rate of evaporation to maintain consistent output steam pressure.

### PROPERTIES

- Mass: 500
- Dimensions (WxDxH): 5x7x5
- Cost: $250
- Tags: 
- File: steam_boiler.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Fluid Volume |  |
| number | Temperature |  |

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Coolant A | Port for supplying hot fluid to heat the contents of the boiler. |
| fluid | Coolant B | Port for supplying hot fluid to heat the contents of the boiler. |
| fluid | Water In |  |
| fluid | Steam Out |  |

## Steam Condenser

A condenser for converting steam back to water.

The condenser should be continously cooled to function efficiently.

### PROPERTIES

- Mass: 250
- Dimensions (WxDxH): 3x5x5
- Cost: $250
- Tags: 
- File: steam_condenser.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Fluid Volume |  |
| number | Temperature |  |

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Coolant A | Port for supplying cold fluid to cool the contents of the condenser. |
| fluid | Coolant B | Port for supplying cold fluid to cool the contents of the condenser. |
| fluid | Steam In |  |
| fluid | Water Out |  |

## Steam Piston (Large)

A steam powered piston that converts steam pressure into torque.

Steam pressurized through the outer coupling extends the piston and steam pressurized through the inner coupling retracts the piston. Alternating pressure to the couplings based on the piston position will allow the crankpin to rotate continuously.

### PROPERTIES

- Mass: 300
- Dimensions (WxDxH): 5x5x15
- Cost: $2400
- Tags: 
- File: steam_piston_5x5.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | RPS |  |
| number | Piston Position |  |

### connections

| Type | Label | Description |
| --- | --- | --- |
| power | RPS | Power connection A. |
| power | RPS | Power connection B. |
| fluid | Steam In |  |
| fluid | Steam Out |  |
| fluid | Steam In |  |
| fluid | Steam Out |  |

## Steam Piston (Medium)

A steam powered piston that converts steam pressure into torque.

Steam pressurized through the outer coupling extends the piston and steam pressurized through the inner coupling retracts the piston. Alternating pressure to the couplings based on the piston position will allow the crankpin to rotate continuously.

### PROPERTIES

- Mass: 120
- Dimensions (WxDxH): 3x3x9
- Cost: $600
- Tags: 
- File: steam_piston_3x3.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | RPS |  |
| number | Piston Position |  |

### connections

| Type | Label | Description |
| --- | --- | --- |
| power | RPS | Power connection A. |
| power | RPS | Power connection B. |
| fluid | Steam In |  |
| fluid | Steam Out |  |
| fluid | Steam In |  |
| fluid | Steam Out |  |

## Steam Piston (Small)

A steam powered piston that converts steam pressure into torque.

Steam pressurized through the outer coupling extends the piston and steam pressurized through the inner coupling retracts the piston. Alternating pressure to the couplings based on the piston position will allow the crankpin to rotate continuously.

### PROPERTIES

- Mass: 12
- Dimensions (WxDxH): 1x1x6
- Cost: $90
- Tags: 
- File: steam_piston.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | RPS |  |
| number | Piston Position |  |

### connections

| Type | Label | Description |
| --- | --- | --- |
| power | RPS | Power connection A. |
| power | RPS | Power connection B. |
| fluid | Steam In |  |
| fluid | Steam Out |  |
| fluid | Steam In |  |
| fluid | Steam Out |  |

## Steam Turbine

A steam powered turbine.

Produces torque based on the force generated by steam passing through the turbine.

### PROPERTIES

- Mass: 500
- Dimensions (WxDxH): 5x5x9
- Cost: $250
- Tags: 
- File: steam_turbine.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Steam In |  |
| fluid | Steam Out |  |
| power | RPS |  |
| power | RPS |  |

## Vacuum Duct

A vacuum for moving resources.

Can be toggled to move resources through the vacuum. The vacuum can transport resources from ducts and hoppers immediately in front of the vacuum nozzle.

### PROPERTIES

- Mass: 20
- Dimensions (WxDxH): 3x3x3
- Cost: $50
- Tags: steam,coal,fishing
- File: steam_coal_vacuum.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Active |  |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical input. |

## Mineral Converter (Deprecated)

> [!WARNING]
> This component is deprecated.

A basic mineral duct.

Transports minerals through the connected system.

### PROPERTIES

- Mass: 80
- Dimensions (WxDxH): 3x3x3
- Cost: $250000
- Tags: steam,coal
- File: mineral_converter.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Mineral Level |  |

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | water |  |
