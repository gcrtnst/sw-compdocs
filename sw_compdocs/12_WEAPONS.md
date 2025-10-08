# Weapons

## Artillery Cannon

An artillery cannon.

Artillery cannons fire high caliber explosive and armor-piercing shells over great distances.

### PROPERTIES

- Mass: 200
- Dimensions (WxDxH): 3x3x22
- Cost: $100
- Tags: weapon,cannon,artillery
- File: gun_xl.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Trigger | When true: fires a loaded shell. |
| on/off | Open Breech | When true: opens the breech to allow shells to be loaded. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Loaded | Returns true when a shell is loaded and ready to fire. |

## Artillery Cannon Barrel Extension

An artillery cannon barrel extension.

Barrel extensions increase weapon accuracy, but also produce more recoil force.

### PROPERTIES

- Mass: 80
- Dimensions (WxDxH): 3x3x4
- Cost: $50
- Tags: weapon,cannon,artillery
- File: gun_xl_barrel.xml

## Artillery Cannon Barrel Extension

An artillery cannon barrel extension.

Barrel extensions increase weapon accuracy, but also produce more recoil force.

### PROPERTIES

- Mass: 80
- Dimensions (WxDxH): 3x3x4
- Cost: $50
- Tags: weapon,cannon,artillery
- File: gun_xl_barrel_1.xml

## Artillery Cannon Barrel Extension

An artillery cannon barrel extension.

Barrel extensions increase weapon accuracy, but also produce more recoil force.

### PROPERTIES

- Mass: 80
- Dimensions (WxDxH): 3x3x4
- Cost: $50
- Tags: weapon,cannon,artillery
- File: gun_xl_barrel_2.xml

## Artillery Cannon Barrel Extension

An artillery cannon barrel extension.

Barrel extensions increase weapon accuracy, but also produce more recoil force.

### PROPERTIES

- Mass: 80
- Dimensions (WxDxH): 3x3x4
- Cost: $50
- Tags: weapon,cannon,artillery
- File: gun_xl_barrel_3.xml

## Artillery Cannon Belt (Connector)

An artillery cannon ammo belt.

Cannon ammo belts can store and transfer ammo shells. Connector belts allow ammo transfers between vehicles. Spawned ammo type can be set in component properties window.

### PROPERTIES

- Mass: 4
- Dimensions (WxDxH): 1x4x1
- Cost: $100
- Tags: weapon,cannon,belt,artillery
- File: gun_belt_receiver_xl.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Contains Ammo | Returns true if the belt contains a shell. |
| on/off | Connected | Returns true when two nearby receivers are aligned, and can transfer ammo between them. |

## Artillery Cannon Belt (Corner Inner)

An artillery cannon ammo belt.

Cannon ammo belts can store and transfer ammo shells. Spawned ammo type can be set in component properties window.

### PROPERTIES

- Mass: 15
- Dimensions (WxDxH): 1x4x4
- Cost: $100
- Tags: weapon,cannon,belt,artillery
- File: gun_belt_corner_flat_xl.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Contains Ammo | Returns true if the belt contains a shell. |

## Artillery Cannon Belt (Corner Outer)

An artillery cannon ammo belt.

Cannon ammo belts can store and transfer ammo shells. Spawned ammo type can be set in component properties window.

### PROPERTIES

- Mass: 15
- Dimensions (WxDxH): 1x4x4
- Cost: $100
- Tags: weapon,cannon,belt,artillery
- File: gun_belt_corner_flat_reverse_xl.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Contains Ammo | Returns true if the belt contains a shell. |

## Artillery Cannon Belt (Corner)

An artillery cannon ammo belt.

Cannon ammo belts can store and transfer ammo shells. Spawned ammo type can be set in component properties window.

### PROPERTIES

- Mass: 4
- Dimensions (WxDxH): 1x4x1
- Cost: $100
- Tags: weapon,cannon,belt,artillery
- File: gun_belt_corner_xl.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Contains Ammo | Returns true if the belt contains a shell. |

## Artillery Cannon Belt (Feeder)

An artillery cannon ammo belt.

Cannon ammo belts can store and transfer ammo shells. Feeder belts transfer ammo forwards using electric power. Spawned ammo type can be set in component properties window.

### PROPERTIES

- Mass: 5
- Dimensions (WxDxH): 1x5x1
- Cost: $100
- Tags: weapon,cannon,belt,artillery
- File: gun_belt_loader_xl.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Feed | Transfer shells in the direction of the arrow. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Contains Ammo | Returns true if the belt contains a shell. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Artillery Cannon Belt (Flexible)

An artillery cannon ammo belt.

Flexible belts can be connected together by rope nodes to transfer ammo. Cannon ammo belts can store and transfer ammo shells. Spawned ammo type can be set in component properties window.

### PROPERTIES

- Mass: 4
- Dimensions (WxDxH): 1x4x2
- Cost: $100
- Tags: weapon,cannon,belt,artillery
- File: gun_belt_flex_xl.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| rope | Ammo |  |

## Artillery Cannon Belt (Junction)

An artillery cannon ammo belt.

Cannon ammo belts can store and transfer ammo shells. Junction belts redirect the path of ammo transfer. Spawned ammo type can be set in component properties window.

### PROPERTIES

- Mass: 4
- Dimensions (WxDxH): 1x4x1
- Cost: $100
- Tags: weapon,cannon,belt,artillery
- File: gun_belt_junction_xl.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Junction Switch | Switches the ammo transfer T-junction between the left and right sides. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Contains Ammo | Returns true if the belt contains a shell. |

## Artillery Cannon Belt (Straight)

An artillery cannon ammo belt.

Cannon ammo belts can store and transfer ammo shells. Spawned ammo type can be set in component properties window.

### PROPERTIES

- Mass: 4
- Dimensions (WxDxH): 1x4x1
- Cost: $100
- Tags: weapon,cannon,belt,artillery
- File: gun_belt_straight_xl.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Contains Ammo | Returns true if the belt contains a shell. |

## Artillery Cannon Muzzle Brake

A artillery cannon muzzle brake.

A muzzle brake will reduce weapon recoil force when added to the end of a weapon barrel.

### PROPERTIES

- Mass: 80
- Dimensions (WxDxH): 3x3x5
- Cost: $50
- Tags: weapon,cannon,artillery
- File: gun_xl_muzzle.xml

## Artillery Cannon Muzzle Brake

A artillery cannon muzzle brake.

A muzzle brake will reduce weapon recoil force when added to the end of a weapon barrel.

### PROPERTIES

- Mass: 80
- Dimensions (WxDxH): 3x3x5
- Cost: $50
- Tags: weapon,cannon,artillery
- File: gun_xl_muzzle_1.xml

## Artillery Cannon Muzzle Brake

A artillery cannon muzzle brake.

A muzzle brake will reduce weapon recoil force when added to the end of a weapon barrel.

### PROPERTIES

- Mass: 80
- Dimensions (WxDxH): 3x3x5
- Cost: $50
- Tags: weapon,cannon,artillery
- File: gun_xl_muzzle_2.xml

## Autocannon Ammo Drum (Large)

A large capacity autocannon ammo drum.

Ammo drums store autocannon cartridges of the caliber specified in the component properties window. Differing calibers cannot be mixed within a single ammo drum.

### PROPERTIES

- Mass: 40
- Dimensions (WxDxH): 4x4x3
- Cost: $100
- Tags: weapon,autocannon,belt
- File: gun_drum_large.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Ammo Count | Outputs the total ammo count stored in the drum. |

## Autocannon Ammo Drum (Medium)

A medium capacity autocannon ammo drum.

Ammo drums store autocannon cartridges of the caliber specified in the component properties window. Differing calibers cannot be mixed within a single ammo drum.

### PROPERTIES

- Mass: 20
- Dimensions (WxDxH): 3x3x3
- Cost: $100
- Tags: weapon,autocannon,belt
- File: gun_drum_medium.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Ammo Count | Outputs the total ammo count stored in the drum. |

## Autocannon Ammo Drum (Small)

A small capacity autocannon ammo drum.

Ammo drums store autocannon cartridges of the caliber specified in the component properties window. Differing calibers cannot be mixed within a single ammo drum.

### PROPERTIES

- Mass: 10
- Dimensions (WxDxH): 2x2x3
- Cost: $100
- Tags: weapon,autocannon,belt
- File: gun_drum_small.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Ammo Count | Outputs the total ammo count stored in the drum. |

## Autocannon Belt (Connector)

An autocannon ammo belt.

Autocannon belts can transfer all calibers of autocannon ammo. Connector belts allow ammo transfers between vehicles.

### PROPERTIES

- Mass: 3
- Dimensions (WxDxH): 1x3x1
- Cost: $100
- Tags: weapon,autocannon,belt
- File: gun_belt_receiver.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Contains Ammo | Returns true if the belt contains a shell. |
| on/off | Connected |  |

## Autocannon Belt (Corner Flat)

An autocannon ammo belt.

Autocannon belts can transfer all calibers of autocannon ammo.

### PROPERTIES

- Mass: 9
- Dimensions (WxDxH): 1x3x3
- Cost: $100
- Tags: weapon,autocannon,belt
- File: gun_belt_corner_flat.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Contains Ammo | Returns true if the belt contains a shell. |

## Autocannon Belt (Corner)

An autocannon ammo belt.

Autocannon belts can transfer all calibers of autocannon ammo.

### PROPERTIES

- Mass: 3
- Dimensions (WxDxH): 1x3x1
- Cost: $100
- Tags: weapon,autocannon,belt
- File: gun_belt_corner.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Contains Ammo | Returns true if the belt contains a shell. |

## Autocannon Belt (Feeder)

An autocannon ammo belt.

Autocannon belts can transfer all calibers of autocannon ammo. Feeder belts transfer ammo forwards using electric power.

### PROPERTIES

- Mass: 4
- Dimensions (WxDxH): 1x4x1
- Cost: $100
- Tags: weapon,autocannon,belt
- File: gun_belt_loader.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Feed | Transfer cartridges in the direction of the arrow. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Contains Ammo | Returns true if the belt contains a shell. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Autocannon Belt (Flexible)

An autocannon ammo belt.

Flexible belts can be connected together by rope nodes to transfer ammo. Autocannon belts can transfer all calibers of autocannon ammo.

### PROPERTIES

- Mass: 3
- Dimensions (WxDxH): 1x3x2
- Cost: $100
- Tags: weapon,autocannon,belt
- File: gun_belt_flex.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| rope | Ammo |  |

## Autocannon Belt (Junction)

An autocannon ammo belt.

Autocannon belts can transfer all calibers of autocannon ammo. Junction belts redirect the path of ammo transfer.

### PROPERTIES

- Mass: 3
- Dimensions (WxDxH): 1x3x1
- Cost: $100
- Tags: weapon,autocannon,belt
- File: gun_belt_junction.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Junction Switch | Switches the ammo transfer T-junction between the left and right sides. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Contains Ammo | Returns true if the belt contains a shell. |

## Autocannon Belt (Straight)

An autocannon ammo belt.

Autocannon belts can transfer all calibers of autocannon ammo.

### PROPERTIES

- Mass: 3
- Dimensions (WxDxH): 1x3x1
- Cost: $100
- Tags: weapon,autocannon,belt
- File: gun_belt_straight.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Contains Ammo | Returns true if the belt contains a shell. |

## Battle Cannon

A battle cannon.

Battle cannons provide powerful, consistent firepower in a compact form.

### PROPERTIES

- Mass: 100
- Dimensions (WxDxH): 3x2x12
- Cost: $100
- Tags: weapon,cannon,battle
- File: gun_l.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Trigger | When true: fires a loaded shell. |
| on/off | Open Breech | When true: opens the breech to allow shells to be loaded. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Loaded | Returns true when a shell is loaded and ready to fire. |

## Battle Cannon Barrel Extension

A battle cannon barrel extension.

Barrel extensions increase weapon accuracy, but also produce more recoil force.

### PROPERTIES

- Mass: 40
- Dimensions (WxDxH): 1x1x3
- Cost: $50
- Tags: weapon,cannon,battle
- File: gun_l_barrel.xml

## Battle Cannon Barrel Extension

A battle cannon barrel extension.

Barrel extensions increase weapon accuracy, but also produce more recoil force.

### PROPERTIES

- Mass: 40
- Dimensions (WxDxH): 3x3x3
- Cost: $50
- Tags: weapon,cannon,battle
- File: gun_l_barrel_1.xml

## Battle Cannon Barrel Extension

A battle cannon barrel extension.

Barrel extensions increase weapon accuracy, but also produce more recoil force.

### PROPERTIES

- Mass: 40
- Dimensions (WxDxH): 1x2x3
- Cost: $50
- Tags: weapon,cannon,battle
- File: gun_l_barrel_2.xml

## Battle Cannon Barrel Extension

A battle cannon barrel extension.

Barrel extensions increase weapon accuracy, but also produce more recoil force.

### PROPERTIES

- Mass: 40
- Dimensions (WxDxH): 3x3x3
- Cost: $50
- Tags: weapon,cannon,battle
- File: gun_l_barrel_3.xml

## Battle Cannon Belt (Connector)

A battle cannon ammo belt.

Cannon ammo belts can store and transfer ammo shells. Connector belts allow ammo transfers between vehicles. Spawned ammo type can be set in component properties window.

### PROPERTIES

- Mass: 3
- Dimensions (WxDxH): 1x3x1
- Cost: $100
- Tags: weapon,cannon,belt,battle
- File: gun_belt_receiver_l.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Contains Ammo | Returns true if the belt contains a shell. |
| on/off | Connected | Returns true when two nearby receivers are aligned, and can transfer ammo between them. |

## Battle Cannon Belt (Corner Inner)

A battle cannon ammo belt.

Cannon ammo belts can store and transfer ammo shells. Spawned ammo type can be set in component properties window.

### PROPERTIES

- Mass: 9
- Dimensions (WxDxH): 1x3x3
- Cost: $100
- Tags: weapon,cannon,belt,battle
- File: gun_belt_corner_flat_l.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Contains Ammo | Returns true if the belt contains a shell. |

## Battle Cannon Belt (Corner Outer)

A battle cannon ammo belt.

Cannon ammo belts can store and transfer ammo shells. Spawned ammo type can be set in component properties window.

### PROPERTIES

- Mass: 9
- Dimensions (WxDxH): 1x3x3
- Cost: $100
- Tags: weapon,cannon,belt,battle
- File: gun_belt_corner_flat_reverse_l.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Contains Ammo | Returns true if the belt contains a shell. |

## Battle Cannon Belt (Corner)

A battle cannon ammo belt.

Cannon ammo belts can store and transfer ammo shells. Spawned ammo type can be set in component properties window.

### PROPERTIES

- Mass: 3
- Dimensions (WxDxH): 1x3x1
- Cost: $100
- Tags: weapon,cannon,belt,battle
- File: gun_belt_corner_l.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Contains Ammo | Returns true if the belt contains a shell. |

## Battle Cannon Belt (Feeder)

A battle cannon ammo belt.

Cannon ammo belts can store and transfer ammo shells. Feeder belts transfer ammo forwards using electric power. Spawned ammo type can be set in component properties window.

### PROPERTIES

- Mass: 4
- Dimensions (WxDxH): 1x4x1
- Cost: $100
- Tags: weapon,cannon,belt,battle
- File: gun_belt_loader_l.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Feed | Transfer shells in the direction of the arrow. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Contains Ammo | Returns true if the belt contains a shell. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Battle Cannon Belt (Flexible)

A battle cannon ammo belt.

Flexible belts can be connected together by rope nodes to transfer ammo. Cannon ammo belts can store and transfer ammo shells. Spawned ammo type can be set in component properties window.

### PROPERTIES

- Mass: 3
- Dimensions (WxDxH): 1x3x2
- Cost: $100
- Tags: weapon,cannon,belt,battle
- File: gun_belt_flex_l.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| rope | Ammo |  |

## Battle Cannon Belt (Junction)

A battle cannon ammo belt.

Cannon ammo belts can store and transfer ammo shells. Junction belts redirect the path of ammo transfer. Spawned ammo type can be set in component properties window.

### PROPERTIES

- Mass: 3
- Dimensions (WxDxH): 1x3x1
- Cost: $100
- Tags: weapon,cannon,belt,battle
- File: gun_belt_junction_l.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Junction Switch | Switches the ammo transfer T-junction between the left and right sides. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Contains Ammo | Returns true if the belt contains a shell. |

## Battle Cannon Belt (Straight)

A battle cannon ammo belt.

Cannon ammo belts can store and transfer ammo shells. Spawned ammo type can be set in component properties window.

### PROPERTIES

- Mass: 3
- Dimensions (WxDxH): 1x3x1
- Cost: $100
- Tags: weapon,cannon,belt,battle
- File: gun_belt_straight_l.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Contains Ammo | Returns true if the belt contains a shell. |

## Battle Cannon Muzzle Brake

A battle cannon muzzle brake.

A muzzle brake will reduce weapon recoil force when added to the end of a weapon barrel.

### PROPERTIES

- Mass: 40
- Dimensions (WxDxH): 1x1x4
- Cost: $50
- Tags: weapon,cannon,battle
- File: gun_l_muzzle.xml

## Battle Cannon Muzzle Brake

A battle cannon muzzle brake.

A muzzle brake will reduce weapon recoil force when added to the end of a weapon barrel.

### PROPERTIES

- Mass: 40
- Dimensions (WxDxH): 3x1x4
- Cost: $50
- Tags: weapon,cannon,battle
- File: gun_l_muzzle_1.xml

## Battle Cannon Muzzle Brake

A battle cannon muzzle brake.

A muzzle brake will reduce weapon recoil force when added to the end of a weapon barrel.

### PROPERTIES

- Mass: 40
- Dimensions (WxDxH): 3x3x4
- Cost: $50
- Tags: weapon,cannon,battle
- File: gun_l_muzzle_2.xml

## Bertha Cannon

A Bertha cannon.

The Bertha cannon fires devastating high explosive mortar shells, with a wide radius of destruction.

### PROPERTIES

- Mass: 500
- Dimensions (WxDxH): 5x5x30
- Cost: $100
- Tags: weapon,cannon,bertha
- File: gun_xxl.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Trigger | When true: fires a loaded shell. |
| on/off | Open Breech | When true: opens the breech to allow shells to be loaded. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Loaded | Returns true when a shell is loaded and ready to fire. |

## Bertha Cannon Barrel Extension

A Bertha cannon barrel extension.

Barrel extensions increase weapon accuracy, but also produce more recoil force.

### PROPERTIES

- Mass: 200
- Dimensions (WxDxH): 3x3x4
- Cost: $50
- Tags: weapon,cannon,bertha
- File: gun_xxl_barrel.xml

## Bertha Cannon Belt (Connector)

A bertha cannon ammo belt.

Cannon ammo belts can store and transfer ammo shells. Connector belts allow ammo transfers between vehicles. Spawned ammo type can be set in component properties window. Bertha shells are too large to be moved by hand.

### PROPERTIES

- Mass: 63
- Dimensions (WxDxH): 3x7x3
- Cost: $100
- Tags: weapon,cannon,belt,bertha
- File: gun_belt_receiver_xxl.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Contains Ammo | Returns true if the belt contains a shell. |
| on/off | Connected | Returns true when two nearby receivers are aligned, and can transfer ammo between them. |

## Bertha Cannon Belt (Corner Inner)

A bertha cannon ammo belt.

Cannon ammo belts can store and transfer ammo shells. Spawned ammo type can be set in component properties window. Bertha shells are too large to be moved by hand.

### PROPERTIES

- Mass: 138
- Dimensions (WxDxH): 3x7x7
- Cost: $100
- Tags: weapon,cannon,belt,bertha
- File: gun_belt_corner_flat_xxl.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Contains Ammo | Returns true if the belt contains a shell. |

## Bertha Cannon Belt (Corner Outer)

A bertha cannon ammo belt.

Cannon ammo belts can store and transfer ammo shells. Spawned ammo type can be set in component properties window. Bertha shells are too large to be moved by hand.

### PROPERTIES

- Mass: 138
- Dimensions (WxDxH): 3x7x7
- Cost: $100
- Tags: weapon,cannon,belt,bertha
- File: gun_belt_corner_flat_reverse_xxl.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Contains Ammo | Returns true if the belt contains a shell. |

## Bertha Cannon Belt (Corner)

A bertha cannon ammo belt.

Cannon ammo belts can store and transfer ammo shells. Spawned ammo type can be set in component properties window. Bertha shells are too large to be moved by hand.

### PROPERTIES

- Mass: 63
- Dimensions (WxDxH): 3x7x3
- Cost: $100
- Tags: weapon,cannon,belt,bertha
- File: gun_belt_corner_xxl.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Contains Ammo | Returns true if the belt contains a shell. |

## Bertha Cannon Belt (Feeder)

A bertha cannon ammo belt.

Cannon ammo belts can store and transfer ammo shells. Feedeer belts transfer ammo forwards using electric power. Spawned ammo type can be set in component properties window. Bertha shells are too large to be moved by hand.

### PROPERTIES

- Mass: 90
- Dimensions (WxDxH): 3x10x3
- Cost: $100
- Tags: weapon,cannon,belt,bertha
- File: gun_belt_loader_xxl.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Feed | Transfer shells in the direction of the arrow. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Contains Ammo | Returns true if the belt contains a shell. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Bertha Cannon Belt (Flexible)

A bertha cannon ammo belt.

Flexible belts can be connected together by rope nodes to transfer ammo. Cannon ammo belts can store and transfer ammo shells. Spawned ammo type can be set in component properties window. Bertha shells are too large to be moved by hand.

### PROPERTIES

- Mass: 63
- Dimensions (WxDxH): 3x7x4
- Cost: $100
- Tags: weapon,cannon,belt,bertha
- File: gun_belt_flex_xxl.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| rope | Ammo |  |

## Bertha Cannon Belt (Junction)

A bertha cannon ammo belt.

Cannon ammo belts can store and transfer ammo shells. Junction belts redirect the path of ammo transfer. Spawned ammo type can be set in component properties window. Bertha shells are too large to be moved by hand.

### PROPERTIES

- Mass: 63
- Dimensions (WxDxH): 3x7x3
- Cost: $100
- Tags: weapon,cannon,belt,bertha
- File: gun_belt_junction_xxl.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Junction Switch | Switches the ammo transfer T-junction between the left and right sides. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Contains Ammo | Returns true if the belt contains a shell. |

## Bertha Cannon Belt (Straight)

A bertha cannon ammo belt.

Cannon ammo belts can store and transfer ammo shells. Spawned ammo type can be set in component properties window. Bertha shells are too large to be moved by hand.

### PROPERTIES

- Mass: 63
- Dimensions (WxDxH): 3x7x3
- Cost: $100
- Tags: weapon,cannon,belt,bertha
- File: gun_belt_straight_xxl.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Contains Ammo | Returns true if the belt contains a shell. |

## Heavy Autocannon

A heavy autocannon.

Heavy autocannons bridge the gap between fast-firing autocannons and high-caliber cannons. Autocannons require electric power to load ammo from connected belts or drums.

### PROPERTIES

- Mass: 50
- Dimensions (WxDxH): 1x1x10
- Cost: $100
- Tags: weapon,autocannon
- File: gun_m.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Trigger | When true: feeds, loads, and fires cartridges from a connected belt or drum. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Loaded | Returns true when a cartridge is loaded and ready to fire. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Heavy Autocannon Barrel Extension

A heavy autocannon barrel extension.

Barrel extensions increase weapon accuracy, but add additional weight.

### PROPERTIES

- Mass: 20
- Dimensions (WxDxH): 1x1x3
- Cost: $50
- Tags: weapon,autocannon
- File: gun_m_barrel.xml

## Heavy Autocannon Barrel Extension

A heavy autocannon barrel extension.

Barrel extensions increase weapon accuracy, but also produce more recoil force.

### PROPERTIES

- Mass: 20
- Dimensions (WxDxH): 1x1x3
- Cost: $50
- Tags: weapon,autocannon
- File: gun_m_barrel_1.xml

## Heavy Autocannon Barrel Extension

A heavy autocannon barrel extension.

Barrel extensions increase weapon accuracy, but also produce more recoil force.

### PROPERTIES

- Mass: 20
- Dimensions (WxDxH): 1x2x3
- Cost: $50
- Tags: weapon,autocannon
- File: gun_m_barrel_2.xml

## Heavy Autocannon Barrel Extension

A heavy autocannon barrel extension.

Barrel extensions increase weapon accuracy, but also produce more recoil force.

### PROPERTIES

- Mass: 20
- Dimensions (WxDxH): 1x2x3
- Cost: $50
- Tags: weapon,autocannon
- File: gun_m_barrel_3.xml

## Heavy Autocannon Muzzle Brake

A heavy autocannon muzzle brake.

A muzzle brake will reduce weapon recoil force when added to the end of a weapon barrel.

### PROPERTIES

- Mass: 20
- Dimensions (WxDxH): 1x1x4
- Cost: $50
- Tags: weapon,autocannon
- File: gun_m_muzzle.xml

## Heavy Autocannon Muzzle Brake

A heavy autocannon muzzle brake.

A muzzle brake will reduce weapon recoil force when added to the end of a weapon barrel.

### PROPERTIES

- Mass: 20
- Dimensions (WxDxH): 1x1x4
- Cost: $50
- Tags: weapon,autocannon
- File: gun_m_muzzle_1.xml

## Heavy Autocannon Muzzle Brake

A heavy autocannon muzzle brake.

A muzzle brake will reduce weapon recoil force when added to the end of a weapon barrel.

### PROPERTIES

- Mass: 20
- Dimensions (WxDxH): 1x1x4
- Cost: $50
- Tags: weapon,autocannon
- File: gun_m_muzzle_2.xml

## Light Autocannon

A light autocannon.

Light autocannons provide rapid fire and high ammo capacity. Autocannons require electric power to load ammo from connected belts or drums.

### PROPERTIES

- Mass: 25
- Dimensions (WxDxH): 2x1x6
- Cost: $100
- Tags: weapon,autocannon
- File: gun_s.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Trigger | When true: feeds, loads, and fires cartridges from a connected belt or drum. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Loaded | Returns true when a cartridge is loaded and ready to fire. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Light Autocannon Barrel Extension

A light autocannon barrel extension.

Barrel extensions increase weapon accuracy, but also produce more recoil force.

### PROPERTIES

- Mass: 10
- Dimensions (WxDxH): 1x1x3
- Cost: $50
- Tags: weapon,autocannon
- File: gun_s_barrel.xml

## Light Autocannon Muzzle Brake

A light autocannon muzzle brake.

A muzzle brake will reduce weapon recoil force when added to the end of a weapon barrel.

### PROPERTIES

- Mass: 3
- Dimensions (WxDxH): 1x1x2
- Cost: $50
- Tags: weapon,autocannon
- File: gun_s_muzzle.xml

## Light Autocannon Muzzle Brake

A light autocannon muzzle brake.

A muzzle brake will reduce weapon recoil force when added to the end of a weapon barrel.

### PROPERTIES

- Mass: 3
- Dimensions (WxDxH): 1x1x2
- Cost: $50
- Tags: weapon,autocannon
- File: gun_s_muzzle_1.xml

## Light Autocannon Muzzle Brake

A light autocannon muzzle brake.

A muzzle brake will reduce weapon recoil force when added to the end of a weapon barrel.

### PROPERTIES

- Mass: 3
- Dimensions (WxDxH): 1x1x2
- Cost: $50
- Tags: weapon,autocannon
- File: gun_s_muzzle_2.xml

## Light Autocannon Muzzle Brake

A light autocannon muzzle brake.

A muzzle brake will reduce weapon recoil force when added to the end of a weapon barrel.

### PROPERTIES

- Mass: 3
- Dimensions (WxDxH): 1x1x2
- Cost: $50
- Tags: weapon,autocannon
- File: gun_s_muzzle_3.xml

## Machine Gun

A machine gun.

Machine guns are lightweight and compact, but require ammo boxes to be reloaded by hand.

### PROPERTIES

- Mass: 10
- Dimensions (WxDxH): 1x1x4
- Cost: $50
- Tags: weapon,machinegun
- File: gun_xs.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Trigger | When true: feeds, loads, and fires cartridges from a connected ammo box. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Loaded | Returns true when a cartridge is loaded and ready to fire. |

## Machine Gun Ammo Box

A machine gun ammo box.

Stores machine gun ammo, but can only be reloaded by hand. Machine guns are restricted to Kinetic, Armor-Piercing, and Incendiary ammo only.

### PROPERTIES

- Mass: 5
- Dimensions (WxDxH): 1x1x1
- Cost: $20
- Tags: weapon,machinegun,belt
- File: gun_drum_xsmall.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Ammo count | Outputs the total ammo count stored in the box. |

## Rocket Launcher

A 4-shot rocket launcher.

Rocket launchers fire powerful high explosive rockets, but cannot be reloaded once empty. Rockets are vulnerable to bullets while in flight.

### PROPERTIES

- Mass: 50
- Dimensions (WxDxH): 1x1x8
- Cost: $100
- Tags: weapon,explosive
- File: gun_rocket_launcher.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Trigger | When true: fires a loaded rocket. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Loaded | Returns true when a rocket is loaded and ready to fire. |
| on/off | Trigger Passthrough | Outputs the trigger value once all rockets have been expended. |

## Rotary Autocannon

A rotary autocannon.

Rotary autocannons have a tremendous rate of fire, but can overheat quickly. Autocannons require electric power to load ammo from connected belts or drums.

### PROPERTIES

- Mass: 400
- Dimensions (WxDxH): 4x2x13
- Cost: $100
- Tags: weapon,autocannon
- File: gun_v.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Trigger | When true: feeds, loads, and fires cartridges from a connected belt or drum. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Loaded | Returns true when a cartridge is loaded and ready to fire. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Rotary Autocannon Barrel Extension

A rotary autocannon barrel extension.

Barrel extensions increase weapon accuracy, but add additional weight.

### PROPERTIES

- Mass: 40
- Dimensions (WxDxH): 1x1x4
- Cost: $50
- Tags: weapon,autocannon
- File: gun_v_barrel.xml

## Warhead (EMP)

A electromagnetic-pulse warhead.

Detonates from an impact, creating an EMP to temporarily shut down nearby electronic systems.

### PROPERTIES

- Mass: 500
- Dimensions (WxDxH): 5x5x13
- Cost: $200
- Tags: weapons,explosive
- File: warhead_emp.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Arm | Arm the EMP charge in the warhead to detonate when the internal impact sensor reaches its threshold. |

## Warhead (Large)

A large explosive warhead.

Detonates from an impact, or when receiving damage. Be careful!

### PROPERTIES

- Mass: 400
- Dimensions (WxDxH): 5x5x9
- Cost: $100
- Tags: weapons,explosive
- File: warhead_large.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Arm | Arm the explosives in the warhead to detonate when the internal impact sensor reaches its threshold. |

## Warhead (Medium)

A medium explosive warhead.

Detonates from an impact, or when receiving damage. Be careful!

### PROPERTIES

- Mass: 80
- Dimensions (WxDxH): 3x3x5
- Cost: $50
- Tags: weapons,explosive
- File: warhead_medium.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Arm | Arm the explosives in the warhead to detonate when the internal impact sensor reaches its threshold. |

## Warhead (Small)

A small explosive warhead.

Detonates from an impact, or when receiving damage. Be careful!

### PROPERTIES

- Mass: 15
- Dimensions (WxDxH): 1x1x2
- Cost: $25
- Tags: weapons,explosive
- File: warhead_small.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Arm | Arm the explosives in the warhead to detonate when the internal impact sensor reaches its threshold. |

## Warhead Body (Large)

A large explosive warhead.

Detonates from an impact, or when receiving damage. Be careful!

### PROPERTIES

- Mass: 400
- Dimensions (WxDxH): 5x5x9
- Cost: $100
- Tags: weapons,explosive
- File: warhead_body_large.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Arm | Arm the explosives in the warhead to detonate when the internal impact sensor reaches its threshold. |

## Warhead Body (Medium)

A medium explosive warhead.

Detonates from an impact, or when receiving damage. Be careful!

### PROPERTIES

- Mass: 80
- Dimensions (WxDxH): 3x3x5
- Cost: $50
- Tags: weapons,explosive
- File: warhead_body_medium.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Arm | Arm the explosives in the warhead to detonate when the internal impact sensor reaches its threshold. |

## Warhead Body (Small)

A small explosive warhead.

Detonates from an impact, or when receiving damage. Be careful!

### PROPERTIES

- Mass: 15
- Dimensions (WxDxH): 1x1x2
- Cost: $25
- Tags: weapons,explosive
- File: warhead_body_small.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Arm | Arm the explosives in the warhead to detonate when the internal impact sensor reaches its threshold. |
