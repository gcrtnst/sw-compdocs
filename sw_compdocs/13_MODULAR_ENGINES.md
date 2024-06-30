# Modular Engines

## Modular Engine Air Manifold

A modular engine air manifold.

Attach a manifold to a cylinder to provide a connection for air to that cylinder. Cylinders that are chained directly adjacent to each other can share a single manifold.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $10
- Tags: 
- File: modular_engine_air_manifold.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| number | Throttle |  |

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Air |  |

## Modular Engine Alternator

A modular engine alternator.

Alternators convert mechanical energy from a Drive Belt into electric charge.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $30
- Tags: 
- File: modular_engine_alternator.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| number | Clutch Pressure |  |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric |  |

## Modular Engine Clutch 1x1

A modular engine clutch.

Attach a clutch to a crankshaft block to control the torque made available to the connected system.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $15
- Tags: 
- File: modular_engine_clutch.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| number | Clutch Pressure |  |

### connections

| Type | Label | Description |
| --- | --- | --- |
| power | RPS | The power supplied by the engine for inputting to other components. |

## Modular Engine Clutch 3x3

A modular engine clutch.

Attach a clutch to a crankshaft block to control the torque made available to the connected system.

### PROPERTIES

- Mass: 9
- Dimensions (WxDxH): 3x3x1
- Cost: $25
- Tags: 
- File: modular_engine_clutch_3x3.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| number | Clutch Pressure |  |

### connections

| Type | Label | Description |
| --- | --- | --- |
| power | RPS | The power supplied by the engine for inputting to other components. |

## Modular Engine Clutch 5x5

A modular engine clutch.

Attach a clutch to a crankshaft block to control the torque made available to the connected system.

### PROPERTIES

- Mass: 25
- Dimensions (WxDxH): 5x5x1
- Cost: $50
- Tags: 
- File: modular_engine_clutch_5x5.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| number | Clutch Pressure |  |

### connections

| Type | Label | Description |
| --- | --- | --- |
| power | RPS | The power supplied by the engine for inputting to other components. |

## Modular Engine Coolant Manifold

A modular engine coolant manifold.

Attach a manifold to a cylinder to provide a connection for coolant to that cylinder. Cylinders that are chained directly adjacent to each other can share a single manifold.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $10
- Tags: 
- File: modular_engine_coolant_manifold.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Coolant A |  |
| fluid | Coolant B |  |

## Modular Engine Crankshaft 1x1

A modular engine crankshaft block.

The crankshaft is the core of an engine. Attach cylinders to the outer surfaces to generate power. Multiple crankshaft blocks can be placed adajcent to each other to form larger engines.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $50
- Tags: 
- File: modular_engine_crankshaft.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | RPS | Output value giving data info on engine speed. |

## Modular Engine Crankshaft 3x1

A modular engine crankshaft block.

The crankshaft is the core of an engine. Attach cylinders to the outer surfaces to generate power. Multiple crankshaft blocks can be placed adajcent to each other to form larger engines.

### PROPERTIES

- Mass: 9
- Dimensions (WxDxH): 3x3x1
- Cost: $50
- Tags: 
- File: modular_engine_crankshaft_3x1.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | RPS | Output value giving data info on engine speed. |

## Modular Engine Crankshaft 3x3

A modular engine crankshaft block.

The crankshaft is the core of an engine. Attach cylinders to the outer surfaces to generate power. Multiple crankshaft blocks can be placed adajcent to each other to form larger engines.

### PROPERTIES

- Mass: 27
- Dimensions (WxDxH): 3x3x3
- Cost: $150
- Tags: 
- File: modular_engine_crankshaft_3x3.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | RPS | Output value giving data info on engine speed. |

## Modular Engine Crankshaft 5x5

A modular engine crankshaft block.

The crankshaft is the core of an engine. Attach cylinders to the outer surfaces to generate power. Multiple crankshaft blocks can be placed adajcent to each other to form larger engines.

### PROPERTIES

- Mass: 100
- Dimensions (WxDxH): 5x5x5
- Cost: $350
- Tags: 
- File: modular_engine_crankshaft_5x5.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | RPS | Output value giving data info on engine speed. |

## Modular Engine Crankshaft Converter 3 to 1

A modular engine crankshaft block.

The crankshaft is the core of an engine. This component efficiently converts torque between different size crankshafts. Multiple crankshaft blocks can be placed adajcent to each other to form larger engines.

### PROPERTIES

- Mass: 9
- Dimensions (WxDxH): 3x3x1
- Cost: $75
- Tags: 
- File: modular_engine_crankshaft_converter_3x3.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | RPS | Output value giving data info on engine speed. |

## Modular Engine Crankshaft Converter 5 to 3

A modular engine crankshaft block.

The crankshaft is the core of an engine. This component efficiently converts torque between different size crankshafts. Multiple crankshaft blocks can be placed adajcent to each other to form larger engines.

### PROPERTIES

- Mass: 27
- Dimensions (WxDxH): 5x5x1
- Cost: $275
- Tags: 
- File: modular_engine_crankshaft_converter_5x5.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | RPS | Output value giving data info on engine speed. |

## Modular Engine Cylinder 1x1

A modular engine cylinder.

Attach a cylinder to a crankshafts outer surface to produce power for an engine. The cylinder requires a manifold to move air, fuel, and exhaust through the cylinder. Cylinders that are chained directly adjacent to each other can share a single manifold.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $50
- Tags: 
- File: modular_engine_cylinder_straight.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| composite | Composite Data | Outputs data from the cylinder. (Value 1 : Air Volume) (Value 2 : Fuel Volume) (Value 3 : Temperature) |

## Modular Engine Cylinder 3x3

A modular engine cylinder.

Attach a cylinder to a crankshafts outer surface to produce power for an engine. The cylinder requires a manifold to move air, fuel, and exhaust through the cylinder. Cylinders that are chained directly adjacent to each other can share a single manifold.

### PROPERTIES

- Mass: 27
- Dimensions (WxDxH): 3x3x3
- Cost: $100
- Tags: 
- File: modular_engine_piston_3x3.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| composite | Composite Data | Outputs data from the cylinder. (Value 1 : Air Volume) (Value 2 : Fuel Volume) (Value 3 : Temperature) |

## Modular Engine Cylinder 5x5

A modular engine cylinder.

Attach a cylinder to a crankshafts outer surface to produce power for an engine. The cylinder requires a manifold to move air, fuel, and exhaust through the cylinder. Cylinders that are chained directly adjacent to each other can share a single manifold.

### PROPERTIES

- Mass: 100
- Dimensions (WxDxH): 5x5x5
- Cost: $150
- Tags: 
- File: modular_engine_piston_5x5.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| composite | Composite Data | Outputs data from the cylinder. (Value 1 : Air Volume) (Value 2 : Fuel Volume) (Value 3 : Temperature) |

## Modular Engine Drive Belt 1x1

A modular engine drive belt.

The drive belt attaches to the crankshaft and provides an interface for starters, alternators and pumps.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $30
- Tags: 
- File: modular_engine_drive_belt.xml

## Modular Engine Drive Belt 3x3

A modular engine drive belt.

The drive belt attaches to the crankshaft and provides an interface for starters, alternators and pumps.

### PROPERTIES

- Mass: 9
- Dimensions (WxDxH): 3x3x1
- Cost: $80
- Tags: 
- File: modular_engine_power_manifold_3x3.xml

## Modular Engine Drive Belt 5x5

A modular engine drive belt.

The drive belt attaches to the crankshaft and provides an interface for starters, alternators and pumps.

### PROPERTIES

- Mass: 27
- Dimensions (WxDxH): 5x5x1
- Cost: $160
- Tags: 
- File: modular_engine_power_manifold_5x5.xml

## Modular Engine Exhaust Manifold (Corner)

A modular engine manifold.

Attach a manifold to a cylinder to provide an exhaust output connection for that cylinder. Cylinders that are chained directly adjacent to each other can share a single manifold.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $10
- Tags: 
- File: modular_engine_exhaust_manifold_corner.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Exhaust |  |

## Modular Engine Exhaust Manifold (Straight)

A modular engine manifold.

Attach a manifold to a cylinder to provide an exhaust output connection for that cylinder. Cylinders that are chained directly adjacent to each other can share a single manifold.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $10
- Tags: 
- File: modular_engine_exhaust_manifold_straight.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Exhaust |  |

## Modular Engine Fluid Pump

A modular engine fluid pump.

An pump that attaches to a Drive Belt to mechanically push fluid around a system.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $50
- Tags: 
- File: modular_engine_fluid_pump.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| number | Clutch Pressure |  |

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Fluid In |  |
| fluid | Fluid Out |  |

## Modular Engine Flywheel 1x1

A modular engine crankshaft flywheel.

The crankshaft is the core of an engine. A flywheel piece sits as part of the crankshaft and acts as a momentum (energy) store for a running engine, but also makes the engine harder to start.

### PROPERTIES

- Mass: 100
- Dimensions (WxDxH): 3x3x1
- Cost: $450
- Tags: 
- File: modular_engine_flywheel.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | RPS | Output value giving data info on engine speed. |

## Modular Engine Flywheel 3x3

A modular engine crankshaft flywheel.

The crankshaft is the core of an engine. A flywheel piece sits as part of the crankshaft and acts as a momentum (energy) store for a running engine, but also makes the engine harder to start.

### PROPERTIES

- Mass: 200
- Dimensions (WxDxH): 5x5x1
- Cost: $650
- Tags: 
- File: modular_engine_flywheel_3x3.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | RPS | Output value giving data info on engine speed. |

## Modular Engine Flywheel 5x5

A modular engine crankshaft flywheel.

The crankshaft is the core of an engine. A flywheel piece sits as part of the crankshaft and acts as a momentum (energy) store for a running engine, but also makes the engine harder to start.

### PROPERTIES

- Mass: 300
- Dimensions (WxDxH): 7x7x1
- Cost: $850
- Tags: 
- File: modular_engine_flywheel_5x5.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | RPS | Output value giving data info on engine speed. |

## Modular Engine Fuel Manifold

A modular engine fuel manifold.

Attach a manifold to a cylinder to provide a connection for fuel to that cylinder. Cylinders that are chained directly adjacent to each other can share a single manifold.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $10
- Tags: 
- File: modular_engine_intake_manifold.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| number | Throttle |  |

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Fuel |  |

## Modular Engine Manifold (Corner)

A modular engine manifold.

Attach a manifold to a cylinder to provide connections for air, fuel, and exhaust for that cylinder. Cylinders that are chained directly adjacent to each other can share a single manifold.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $10
- Tags: 
- File: modular_engine_manifold_corner.xml

## Modular Engine Manifold (Straight)

A modular engine manifold.

Attach a manifold to a cylinder to provide connections for air, fuel, and exhaust for that cylinder. Cylinders that are chained directly adjacent to each other can share a single manifold.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $10
- Tags: 
- File: modular_engine_manifold_straight.xml

## Modular Engine Manifold (T)

A modular engine manifold.

Attach a manifold to a cylinder to provide connections for air, fuel, and exhaust for that cylinder. Cylinders that are chained directly adjacent to each other can share a single manifold.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $10
- Tags: 
- File: modular_engine_manifold_t.xml

## Modular Engine Starter

A modular engine starter.

Attach a starter to a Drive Belt component and supply power to apply an inefficient force on the engine to get it started.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $30
- Tags: 
- File: modular_engine_starter.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Starter |  |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Modular Engine Temperature Sensor

A modular engine temperature sensor.

Attach to a crankshaft to provide temperature information.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $50
- Tags: 
- File: modular_engine_sensor_temperature.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Temperature |  |
