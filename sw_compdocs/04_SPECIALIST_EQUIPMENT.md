# Specialist Equipment

## Barometer

Measures the current air pressure.

Returns the pressure in atmospheres of the compartment or current altitude.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x2
- Cost: $20
- Tags: 
- File: barometer.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Pressure |  |

## Bed

A bed.

You can get in and out of the bed by interacting with it using [f]. You can place a rescued survivor in any bed by using [f] while carrying them.

### PROPERTIES

- Mass: 20
- Dimensions (WxDxH): 3x7x4
- Cost: $250
- Tags: basic
- File: seat_bed.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Occupied | Outputs an on signal if this bed is occupied by a character. |

## Camera Gimbal

A gimbal camera with video output feed.

Has an infrared mode as well as pivot controls, a variable field of view.

### PROPERTIES

- Mass: 50
- Dimensions (WxDxH): 3x3x3
- Cost: $5000
- Tags: 
- File: camera_gimbal.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Infrared Mode | Controls whether or not the infrared mode is switched on. |
| number | Field of View | Controls the level of zoom of the camera. |
| number | Pivot Rotation | Controls the rotation of the camera base. |
| number | Pitch Rotation | Controls the rotation of the camera head. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| video | Camera Feed |  |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric |  |

## Camera Medium

A camera with video output feed.

Has infrared mode as well as variable field of view. Can be pivoted up to 0.125 turns using composite input.

### PROPERTIES

- Mass: 10
- Dimensions (WxDxH): 1x1x2
- Cost: $3000
- Tags: 
- File: camera_med.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Infrared Mode | Controls whether or not the infrared mode is switched on. |
| number | Field of View | Controls the level of zoom of the camera. |
| composite | Pivot | Inputs for camera X/Y pivot. (Value 1 : Pivot X) (Value 2 : Pivot Y) |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| video | Camera Feed |  |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric |  |

## Camera Small

A camera with video output feed.

Can be pivoted up to 0.125 turns using composite input.

### PROPERTIES

- Mass: 5
- Dimensions (WxDxH): 1x1x1
- Cost: $1000
- Tags: 
- File: camera_small.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| composite | Pivot | Inputs for camera X/Y pivot. (Value 1 : Pivot X) (Value 2 : Pivot Y) |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| video | Camera Feed |  |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric |  |

## Camera Stabilized

A stabilized gimbal camera with video output feed.

Has an infrared mode, variable field of view, stabilized and tracking modes.

### PROPERTIES

- Mass: 60
- Dimensions (WxDxH): 3x3x3
- Cost: $50000
- Tags: laser,lazer
- File: camera_gimbal_laser.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Infrared Mode | Controls whether or not the infrared mode is switched on. |
| on/off | Enable Laser | Enables the Laser. |
| number | Field of View | Controls the level of zoom of the camera. |
| number | Pivot Rotation | Controls the rotation of the camera base. |
| number | Pitch Rotation | Controls the rotation of the camera head. |
| on/off | Stabilizer Mode | Enable stabilization to keep the camera focused in its current direction. |
| on/off | Tracker Mode | Enable tracking to direct the camera at the current lazed position. |
| number | Laser Wavelength | The specific light wavelength to emit (whole number). |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| video | Camera Feed |  |
| number | Laser Distance | The measured distance in meters. |
| composite | Composite Output | Composite value channels: 1: x position of laser target, 2: y position of laser target, 3: z position of laser target, 4: pitch of component in turns, 5: yaw of component in turns |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric |  |

## Electric Cable Pulley

A pulley that changes attached cable lengths based on forces applied to cables.

Draw a rope logic link between two rope nodes to form a cable. Cables will slide based on difference in force applied to each cable.

### PROPERTIES

- Mass: 25
- Dimensions (WxDxH): 3x3x1
- Cost: $250
- Tags: basic
- File: winch_pulley_cable.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Rope 1 Length | The current length of rope 1 in metres. |
| number | Rope 2 Length | The current length of rope 2 in metres. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| rope | Rope 2 |  |
| rope | Rope 1 |  |

## Electric Cable Pulley (Corner)

A pulley that changes attached cable lengths based on forces applied to cables.

Draw a rope logic link between two rope nodes to form a cable. Cables will slide based on difference in force applied to each cable.

### PROPERTIES

- Mass: 25
- Dimensions (WxDxH): 3x3x1
- Cost: $250
- Tags: basic
- File: winch_pulley_cable_corner.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Rope 1 Length | The current length of rope 1 in metres. |
| number | Rope 2 Length | The current length of rope 2 in metres. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| rope | Rope 2 |  |
| rope | Rope 1 |  |

## Electrical Cable Anchor

An anchor point for a basic data/electric cable.

Draw a rope logic link between two Electrical Cable Anchors to form a cable. Limited to only one link but can transfer Data and Electric across the link.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x2
- Cost: $15
- Tags: basic
- File: rope_hook_composite.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| composite | Composite Input | Composite data to send to the connected anchor. |
| on/off | On/Off Input | On/Off data to send to the connected anchor. |
| video | Video Data Send | Video data to send to the connected anchor. |
| audio | Audio Data Send | Audio data to send to the connected anchor. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| composite | Composite Output | Composite data to receive from the connected anchor. |
| on/off | On/Off Output | On/Off data to receive from the connected anchor. |
| video | Video Data Receive | Video data to receive from the connected anchor. |
| audio | Audio Data Receive | Audio data to receive from the connected anchor. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| rope | Rope Node |  |
| electric | Electric Node |  |

## Equipment inventory (Binoculars)

A small equipment storage unit containing a pair of binoculars.

Hold [lmb] to zoom in on faraway objects.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $50
- Tags: basic
- File: inventory_equipment_binoculars.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Equipment inventory (C4 Detonator)

A small equipment storage unit containing a C-4 remote detonator.

Press [lmb] to detonate armed C-4 explosives.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $50
- Tags: weapon,explosive
- File: inventory_equipment_c4_detonator.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Equipment inventory (C4 Explosive)

A small equipment storage unit containing C-4 plastic explosive.

Press [lmb] to arm and plant the C-4 explosive on a nearby surface.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $50
- Tags: weapon,explosive
- File: inventory_equipment_c4.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Equipment inventory (Cable)

A large equipment storage unit containing 20m of electrical cable.

Press [lmb] to attach the cable to an unoccupied electrical cable anchor. Interacting with [q]/[e] on an occupied electical cable anchor will retrieve the cable if the player has inventory space to hold it.

### PROPERTIES

- Mass: 3
- Dimensions (WxDxH): 1x3x1
- Cost: $200
- Tags: basic
- File: inventory_equipment_cable.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Equipment inventory (Compass)

A small equipment storage unit containing a compass.

When held, the red needle of the compass will point northwards. The compass also displays a bearing on the equipment hotbar UI.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $50
- Tags: basic
- File: inventory_equipment_compass.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Equipment inventory (Defibrillator)

A large equipment storage unit containing a defibrillator.

Press [lmb] on an incapacitated survivor to revive them. Requires electric charge to function, and will recharge when placed into a powered large equipment storage unit.

### PROPERTIES

- Mass: 3
- Dimensions (WxDxH): 1x3x1
- Cost: $200
- Tags: basic
- File: inventory_equipment_defibrillator.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Equipment inventory (Dog Whistle)

A small equipment storage unit containing a dog whistle.

Hold [lmb] to sound the whistle. Nearby dogs will respond to certain whistle patterns. 1 long burst = Wait. 2 short bursts = Follow.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $50
- Tags: 
- File: inventory_equipment_dog_whistle.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Equipment inventory (Fire Extinguisher)

A large equipment storage unit containing a fire extinguisher.

Hold [lmb] to spray a stream of water capable of extinguishing fires. This equipment has a limited water capacity and cannot be refilled.

### PROPERTIES

- Mass: 3
- Dimensions (WxDxH): 1x3x1
- Cost: $200
- Tags: basic,mission
- File: inventory_equipment_fire_extinguisher.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Equipment inventory (First Aid Kit)

A small equipment storage unit containing a first aid kit.

Press [lmb] to heal yourself, or heal a survivor highlighted by your crosshair.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $50
- Tags: basic,mission
- File: inventory_equipment_first_aid.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Equipment inventory (Fishing Rod)

A large equipment storage unit containing a fishing rod.

Hold and release [lmb] to load and cast the fishing line. Hold [lmb] to reel in the fishing line. Press [r] before casting to cycle the sink depth of the hook.

### PROPERTIES

- Mass: 3
- Dimensions (WxDxH): 1x3x1
- Cost: $200
- Tags: basic,fishing
- File: inventory_equipment_fishing_rod.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Equipment inventory (Flare)

A small equipment storage unit containing flares.

Press [lmb] to throw a red smoke flare which burns for a long time.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $50
- Tags: 
- File: inventory_equipment_flare.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Equipment inventory (Flaregun Ammo)

A small equipment storage unit containing a box of flaregun ammo.

Press [lmb] to reload an equipped flaregun.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $50
- Tags: 
- File: inventory_equipment_flaregun_ammo.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Equipment inventory (Flaregun)

A small equipment storage unit containing a flaregun preloaded with 1 flaregun round.

Press [lmb] to fire a red illumination flare that burns for a short time, and [r] to reload.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $50
- Tags: 
- File: inventory_equipment_flaregun.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Equipment inventory (Flashlight)

A small equipment storage unit containing a flashlight.

Press [lmb] to toggle the flashlight on or off. Requires electric charge to function, and will recharge when placed into a powered small equipment storage unit.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $50
- Tags: basic
- File: inventory_equipment_flashlight.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Equipment inventory (Glowstick)

A small equipment storage unit containing glowsticks.

Press [lmb] to throw a glowstick which emits light for an extended time. The editor paint tool can be used to set the glowstick hue.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $50
- Tags: 
- File: inventory_equipment_glowstick.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Equipment Inventory (Hand Grenade)

A small equipment storage unit containing a hand grenade.

Press [lmb] to throw a hand grenade, which will detonate after a short delay.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $50
- Tags: weapon,explosive
- File: inventory_equipment_grenade.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Equipment inventory (Hose)

A large equipment storage unit containing 20m of fluid hosing.

Press [lmb] to attach the hose to an unoccupied fluid hose anchor. Interacting with [q]/[e] on an occupied fluid hose anchor will retrieve the hose if the player has inventory space to hold it. If the hose contains water, press [r] to toggle open the hose valve and allow the water to flow freely.

### PROPERTIES

- Mass: 3
- Dimensions (WxDxH): 1x3x1
- Cost: $200
- Tags: basic
- File: inventory_equipment_hose.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Equipment inventory (Night Vision Binoculars)

A small equipment storage unit containing a pair of night vision binoculars.

Hold [lmb] to zoom in on faraway objects. The night vision effect provides improved visibility in low light conditions, but hinders visibility in daylight. Requires electric charge to function, and will recharge when placed into a powered small equipment storage unit.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $50
- Tags: basic
- File: inventory_equipment_night_vision_binoculars.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Equipment inventory (Oxygen Mask)

A small equipment storage unit containing an oxygen mask.

Press [lmb] to recover your breath while underwater. This equipment has a limited air capacity, and will refill when placed into a powered small equipment storage unit.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $50
- Tags: basic
- File: inventory_equipment_oxygen_mask.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Equipment Inventory (Pistol Ammo)

A small equipment storage unit containing a pistol ammo magazine.

Press [lmb] to reload an equipped pistol.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $50
- Tags: weapon,firearm,gun
- File: inventory_equipment_pistol_ammo.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Equipment inventory (Pistol)

A small equipment storage unit containing a pistol.

Press [lmb] to fire, and [r] to reload. The pistol is compact enough for a belt holster, and can be accurate when recoil is carefully managed.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $200
- Tags: weapon,firearm,gun
- File: inventory_equipment_pistol.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Equipment inventory (Radiation Detector)

A small equipment storage unit containing a radiation detector.

Press [lmb] to toggle radiation detection on or off. Requires electric charge to function, and will recharge when placed into a powered small equipment storage unit.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $50
- Tags: geiger,radiation
- File: inventory_equipment_geiger_counter.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Equipment inventory (Radio Signal Locator)

A large equipment storage unit containing a handheld transponder locator.

Press [lmb] to toggle the locator on or off. When active, the locator produces audible beeps that increase in frequency as the player nears an active transponder. The handheld locator has a shorter detection range than the vehicle mounted locator, but can narrow down the target location to a smaller area. Requires electric charge to function, and will recharge when placed into a powered large equipment storage unit.

### PROPERTIES

- Mass: 3
- Dimensions (WxDxH): 1x3x1
- Cost: $200
- Tags: mission
- File: inventory_equipment_radio_signal_locator.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Equipment inventory (Radio)

A small equipment storage unit containing a handheld radio.

Hold [lmb] transmit voice audio. Press [r] to cycle between frequencies 0~8, or turn the radio off. When a frequency is selected, the radio will transmit and receive voice audio on that frequency only. Requires electric charge to function, and will recharge when placed into a powered small equipment storage unit. (Max Effective Range : 500m)

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $50
- Tags: basic
- File: inventory_equipment_radio.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Equipment inventory (Remote Control Unit)

A small equipment storage unit containing a remote control unit.

Press [lmb] to toggle the remote control on or off. Press [r] to cycle between frequencies 0~8. When active, the remote control uses the basic vehicle pilot seat input bindings and transmits them as composite radio data on the selected frequency. Requires electric charge to function, and will recharge when placed into a powered small equipment storage unit. (Max Effective Range : 500m)

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $50
- Tags: 
- File: inventory_equipment_remote_control.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Equipment inventory (Rifle Ammo)

A small equipment storage unit containing a rifle ammo magazine.

Press [lmb] to reload an equipped rifle.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $50
- Tags: weapon,firearm,gun
- File: inventory_equipment_rifle_ammo.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Equipment inventory (Rifle)

A large equipment storage unit containing a rifle.

Press [lmb] to fire, and [r] to reload. The rifle fires accurate and powerful shots for long-range engagements.

### PROPERTIES

- Mass: 3
- Dimensions (WxDxH): 1x3x1
- Cost: $200
- Tags: weapon,firearm,gun
- File: inventory_equipment_rifle.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Equipment inventory (Rope)

A large equipment storage unit containing 20m of rope.

Press [lmb] to attach the rope to any rope anchor. Interacting with [q]/[e] on an occupied rope anchor will retrieve the rope if the player has inventory space to hold it.

### PROPERTIES

- Mass: 3
- Dimensions (WxDxH): 1x3x1
- Cost: $200
- Tags: basic
- File: inventory_equipment_rope.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Equipment inventory (SMG Ammo)

A small equipment storage unit containing a submachine gun ammo magazine.

Press [lmb] to reload an equipped submachine gun.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $50
- Tags: weapon,firearm,gun
- File: inventory_equipment_smg_ammo.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Equipment inventory (SMG)

A large equipment storage unit containing a submachine gun.

Press [lmb] to fire, and [r] to reload. The SMG has a high rate of fire and magazine capacity.

### PROPERTIES

- Mass: 3
- Dimensions (WxDxH): 1x3x1
- Cost: $200
- Tags: weapon,firearm,gun
- File: inventory_equipment_smg.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Equipment inventory (Speargun Ammo)

A small equipment storage unit containing a box of speargun ammo.

Press [lmb] to reload an equipped speargun.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $50
- Tags: weapon,firearm,gun
- File: inventory_equipment_speargun_ammo.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Equipment inventory (Speargun)

A large equipment storage unit containing a speargun.

Press [lmb] to fire, and [r] to reload. The speargun can be fired underwater and spears travel through the water more effectively than bullets.

### PROPERTIES

- Mass: 3
- Dimensions (WxDxH): 1x3x1
- Cost: $200
- Tags: weapon,firearm,gun
- File: inventory_equipment_speargun.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Equipment inventory (Strobe Light)

A small equipment storage unit containing a strobe light.

Press [lmb] to toggle the strobe light on or off. Press [r] to toggle MOB (man overboard) mode, which will automatically turn the strobe light on if the player is submerged in water. The strobe light will continue to function when unequipped or discarded. Requires electric charge to function, and will recharge when placed into a powered small equipment storage unit.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $50
- Tags: 
- File: inventory_equipment_strobe_light.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Equipment inventory (Strobe Light, Infrared)

A small equipment storage unit containing an infrared strobe light.

Press [lmb] to toggle the strobe light on or off. Press [r] to toggle MOB (man overboard) mode, which will automatically turn the strobe light on if the player is submerged in water. The strobe light will continue to function when unequipped or discarded. The infrared strobe light flashes are only visible to infrared cameras. Requires electric charge to function, and will recharge when placed into a powered small equipment storage unit.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $50
- Tags: 
- File: inventory_equipment_strobe_light_infrared.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Equipment inventory (Transponder)

A small equipment storage unit containing a handheld transponder.

Press [lmb] to toggle the transponder on or off. Press [r] to toggle MOB (man overboard) mode, which will automatically turn the transponder on if the player is submerged in water. The transponder will continue to function when unequipped or discarded. Requires electric charge to function, and will recharge when placed into a powered small equipment storage unit.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $50
- Tags: mission
- File: inventory_equipment_transponder.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Equipment inventory (Underwater Welding Torch)

A large equipment storage unit containing an underwater welding torch.

Hold [lmb] to repair damaged vehicle components highlighted by the players crosshair. The underwater welding torch holds less fuel than the standard welding torch, but can be operated while submerged in water. This equipment has a limited fuel capacity and cannot be refilled.

### PROPERTIES

- Mass: 3
- Dimensions (WxDxH): 1x3x1
- Cost: $200
- Tags: basic
- File: inventory_equipment_underwater_welding_torch.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Equipment inventory (Welding Torch)

A large equipment storage unit containing a welding torch.

Hold [lmb] to repair damaged vehicle components highlighted by the players crosshair. This equipment has a limited fuel capacity and cannot be refilled.

### PROPERTIES

- Mass: 3
- Dimensions (WxDxH): 1x3x1
- Cost: $200
- Tags: basic
- File: inventory_equipment_welding_torch.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Flare Launcher

Single-use flare launcher for signalling and illumination.

Set the flare canister type and launch velocity in the component properties.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x2
- Cost: $10
- Tags: 
- File: flare_launcher.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Launch |  |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Launch Passthrough |  |

## Fluid Cannon

A fluid cannon that fires pressurized water for putting out fires.

The cannon is a turret and can rotate on 2 axis.

### PROPERTIES

- Mass: 11
- Dimensions (WxDxH): 3x3x3
- Cost: $100
- Tags: 
- File: watercannon.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| number | Turret Swivel | Yaw axis servo control for the cannon head. |
| number | Nozzle Pitch | Pitch axis servo control for the cannon head. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Fluid Supply | The fluid input to output from the nozzle. Filters to water only. |
| electric | Electric | Electrical power connection. |

## Fluid Hose Anchor

An anchor point for a basic fluid hose.

Draw a rope logic link between two Fluid Hose Anchors to form a hose. Limited to only one link but can transfer fluid across the link.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x2
- Cost: $15
- Tags: basic
- File: rope_hook_fluid.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| rope | Rope Node |  |
| fluid | Fluid Node |  |

## Fluid Hose Pulley

A pulley that changes attached hose lengths based on forces applied to hoses.

Draw a rope logic link between two rope nodes to form a hose. Hoses will slide based on difference in force applied to each hose.

### PROPERTIES

- Mass: 25
- Dimensions (WxDxH): 3x3x1
- Cost: $250
- Tags: basic
- File: winch_pulley_hose.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Rope 1 Length | The current length of rope 1 in metres. |
| number | Rope 2 Length | The current length of rope 2 in metres. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| rope | Rope 2 |  |
| rope | Rope 1 |  |
| fluid | Fluid Node 1 |  |
| fluid | Fluid Node 2 |  |

## Fluid Hose Pulley (Corner)

A pulley that changes attached hose lengths based on forces applied to hoses.

Draw a rope logic link between two rope nodes to form a hose. Hoses will slide based on difference in force applied to each hose.

### PROPERTIES

- Mass: 25
- Dimensions (WxDxH): 3x3x1
- Cost: $250
- Tags: basic
- File: winch_pulley_hose_corner.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Rope 1 Length | The current length of rope 1 in metres. |
| number | Rope 2 Length | The current length of rope 2 in metres. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| rope | Rope 2 |  |
| rope | Rope 1 |  |
| fluid | Fluid Node 1 |  |
| fluid | Fluid Node 2 |  |

## Fluid Nozzle

A fluid nozzle that fires pressurized water for putting out fires.

The angle of spray can be adjusted.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x2
- Cost: $100
- Tags: cannon,basic
- File: water_nozzle.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| number | Spray Angle | Adjustable spray angle from 0 (focused) to 1 (spread). |

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Fluid Supply | The fluid input to output from the nozzle. |
| electric | Electric | Electrical power connection. |

## Foghorn

A ship's foghorn that will sound when receiving an on signal.

It has an audible range of 1500m.

### PROPERTIES

- Mass: 5
- Dimensions (WxDxH): 4x3x3
- Cost: $200
- Tags: boat,sound,audio
- File: foghorn.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Horn | Sounds the horn when recieving an on signal. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Harness

A rescue harness.

You can get in and out of the harness by interacting with it using [f]. You can place a rescued survivor in any harness by using [f] while carrying them.

### PROPERTIES

- Mass: 20
- Dimensions (WxDxH): 3x3x6
- Cost: $150
- Tags: basic,seat
- File: seat_harness.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Occupied | Outputs an on signal if this harness is occupied by a character. |
| on/off | Trigger [space] | Outputs an on signal when [space] is held, and off when it is not. |
| on/off | Hotkey 1 [1] | Outputs an on signal when [1] is held, and off when it is not. |
| on/off | Hotkey 2 [2] | Outputs an on signal when [2] is held, and off when it is not. |
| on/off | Hotkey 3 [3] | Outputs an on signal when [3] is held, and off when it is not. |
| on/off | Hotkey 4 [4] | Outputs an on signal when [4] is held, and off when it is not. |
| on/off | Hotkey 5 [5] | Outputs an on signal when [5] is held, and off when it is not. |
| on/off | Hotkey 6 [6] | Outputs an on signal when [6] is held, and off when it is not. |
| composite | Seat Data | Outputs the axis, hotkey and occupied data from the seat. (On/Off 1+ : Hotkeys) (On/Off 31 : Trigger) (On/Off 32 : Occupied) (Value 1 : [a]/[d]) (Value 2 : [w]/[s]) (Value 3 : [left]/[right]) (Value 4 : [up]/[down]) |

## Heater

A small heater that will provide warmth in a radius.

When enabled, the heater will warm either the compartment it is within or any players within a 10m radius, allowing them to survive cold temperatures.

### PROPERTIES

- Mass: 3
- Dimensions (WxDxH): 1x3x1
- Cost: $50
- Tags: basic
- File: heater.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Heating Element | Enables the heating element when receiving an on signal. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Huge Winch

A mechanical winch that can transfer data/electric/fluid through an attached cable, with an extension length of 600m.

Draw a rope logic link between two Rope Nodes to form a cable. Can be extended and retracted.

### PROPERTIES

- Mass: 400
- Dimensions (WxDxH): 9x7x7
- Cost: $5000
- Tags: basic
- File: rope_hook_winch_huge.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Down | Lowers the winch cable down when receiving an on signal. |
| on/off | Up | Raises the winch cable up when receiving an on signal. |
| composite | Composite Input | Composite data to send to the connected anchor. |
| on/off | On/Off Input | On/Off data to send to the connected anchor. |
| video | Video Data Send | Video data to send to the connected anchor. |
| audio | Audio Data Send | Audio data to send to the connected anchor. |
| number | Speed | The speed of the winch clamped to a relative range of -1 to 1. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| composite | Composite Output | Composite data to receive from the connected anchor. |
| on/off | On/Off Output | On/Off data to receive from the connected anchor. |
| video | Video Data Receive | Video data to receive from the connected anchor. |
| audio | Audio Data Receive | Audio data to receive from the connected anchor. |
| number | Length | The current length of the winch cable in metres. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| rope | Rope Node |  |
| electric | Electric Node |  |
| fluid | Fluid | Fluid connection for the hose coil. |

## Landing Float

A buoyant float.

Ideal for attaching to helicopters to allow them to land on the ocean.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 3x9x3
- Cost: $50
- Tags: basic
- File: landing_float.xml

## Large equipment inventory (Empty)

An empty large equipment storage unit.

Only large handheld equipment can be stored in this unit. When connected to an electric power source, any rechargable equipment stored in the unit will drain a small amount of electricity until recharged to 100% capacity.

### PROPERTIES

- Mass: 3
- Dimensions (WxDxH): 1x3x1
- Cost: $50
- Tags: basic
- File: inventory_medium.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Large Winch

A mechanical winch that can transfer data/electric/fluid through an attached cable, with an extension length of 150m.

Draw a rope logic link between two Rope Nodes to form a cable. Can be extended and retracted.

### PROPERTIES

- Mass: 100
- Dimensions (WxDxH): 3x3x4
- Cost: $800
- Tags: basic
- File: rope_hook_winch_large.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Down | Lowers the winch cable down when receiving an on signal. |
| on/off | Up | Raises the winch cable up when receiving an on signal. |
| composite | Composite Input | Composite data to send to the connected anchor. |
| on/off | On/Off Input | On/Off data to send to the connected anchor. |
| video | Video Data Send | Video data to send to the connected anchor. |
| audio | Audio Data Send | Audio data to send to the connected anchor. |
| number | Speed | The speed of the winch clamped to a relative range of -1 to 1. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| composite | Composite Output | Composite data to receive from the connected anchor. |
| on/off | On/Off Output | On/Off data to receive from the connected anchor. |
| video | Video Data Receive | Video data to receive from the connected anchor. |
| audio | Audio Data Receive | Audio data to receive from the connected anchor. |
| number | Length | The current length of the winch cable in metres. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| rope | Rope Node |  |
| electric | Electric Node |  |
| fluid | Fluid | Fluid connection for the hose coil. |

## Light

A basic light that can be controlled using an on/off signal.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x2
- Cost: $20
- Tags: 
- File: small_light.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Light Switch | Controls whether or not the light is switched on. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Light (RGB)

An advanced light that can be controlled using a microcontroller.

Three channels of the composite input can be used to set the red, green and blue components of the light's color using numbers between 0 and 1. The light can also operate in HSV mode, where the 3 inputs correspond to the hue, saturation and value (brightness) of the color between 0 and 1. The color mode and input channels can be customised by selecting this component with the select tool.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x2
- Cost: $50
- Tags: 
- File: small_light_rgb.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| composite | Color Data | Composite link containing the light's color data. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Medical Bed

A bed equiped with medical monitoring equipment, slowly heals injured characters.

You can get in and out of the medical bed by interacting with it using [f]. You can place a rescued survivor in any medical bed by using [f] while carrying them.

### PROPERTIES

- Mass: 40
- Dimensions (WxDxH): 3x7x4
- Cost: $2500
- Tags: basic
- File: seat_medical.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Occupied | Outputs an on signal if this bed is occupied by a character. |

## Medium Winch

A mechanical winch that can transfer data/electric/fluid through an attached cable, with an extension length of 40m.

Draw a rope logic link between two Rope Nodes to form a cable. Can be extended and retracted.

### PROPERTIES

- Mass: 20
- Dimensions (WxDxH): 3x1x2
- Cost: $250
- Tags: basic
- File: rope_hook_winch.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Down | Lowers the winch cable down when receiving an on signal. |
| on/off | Up | Raises the winch cable up when receiving an on signal. |
| composite | Composite Input | Composite data to send to the connected anchor. |
| on/off | On/Off Input | On/Off data to send to the connected anchor. |
| video | Video Data Send | Video data to send to the connected anchor. |
| audio | Audio Data Send | Audio data to send to the connected anchor. |
| number | Speed | The speed of the winch clamped to a relative range of -1 to 1. |

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| composite | Composite Output | Composite data to receive from the connected anchor. |
| on/off | On/Off Output | On/Off data to receive from the connected anchor. |
| video | Video Data Receive | Video data to receive from the connected anchor. |
| audio | Audio Data Receive | Audio data to receive from the connected anchor. |
| number | Length | The current length of the winch cable in metres. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| rope | Rope Node |  |
| electric | Electric Node |  |
| fluid | Fluid | Fluid connection for the hose coil. |

## Megaphone Speaker (Large)

A speaker capable of playing audio data to players within its range.

A large megaphone capable of playing audio data to players within its range. (Range : 1000)

### PROPERTIES

- Mass: 10
- Dimensions (WxDxH): 3x5x3
- Cost: $1000
- Tags: 
- File: speaker_large.xml

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

## Megaphone Speaker (Small)

A speaker capable of playing audio data to players within its range.

A small megaphone capable of playing audio data to players within its range. (Range : 300)

### PROPERTIES

- Mass: 3
- Dimensions (WxDxH): 1x2x1
- Cost: $500
- Tags: 
- File: speaker_medium.xml

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

## Mineral Drill

A vehicle mounted drill for mining ore deposits.

The mineral drill can be driven by torque to mine ore deposits in the world. Extracted minerals can be transferred to an attached hopper.

### PROPERTIES

- Mass: 110
- Dimensions (WxDxH): 3x3x6
- Cost: $20000
- Tags: mining,ore,coal
- File: mineral_drill.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| power | Drill Shaft |  |

## Mounted End-Effector

A vehicle mounted end-effector.

The end-effector can interact with button components.

### PROPERTIES

- Mass: 10
- Dimensions (WxDxH): 1x1x2
- Cost: $1000
- Tags: 
- File: vehicle_tool_interact.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Activate | Enable end-effector. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Mounted Welder

A vehicle mounted welding torch.

The welding torch can repair components. This welder is electrically powered and works underwater.

### PROPERTIES

- Mass: 10
- Dimensions (WxDxH): 1x1x2
- Cost: $1000
- Tags: 
- File: vehicle_tool_welder.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Activate | Enable welding torch. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Outfit Inventory (Arctic)

An outfit inventory unit containing specialist thermal clothing for surviving Arctic temperatures.

When equipped, it will increase your temperature enough to survive in colder weather conditions. Its thermal effectiveness is reduced when wet.

### PROPERTIES

- Mass: 9
- Dimensions (WxDxH): 3x1x3
- Cost: $500
- Tags: basic
- File: inventory_outfit_arctic.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Outfit Inventory (Armor Vest)

An outfit inventory unit containing specialist millitary clothing for projectile protection.

When equipped, damage from projectiles to the body and head is greatly reduced.  Wearing the outfit significantly limits movement speed.

### PROPERTIES

- Mass: 9
- Dimensions (WxDxH): 3x1x3
- Cost: $1500
- Tags: basic
- File: inventory_outfit_wep_armor_vest.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Outfit Inventory (Black Hawk Vest)

An outfit inventory unit containing specialist millitary clothing for projectile protection.

When equipped, damage from projectiles to the body is reduced slightly.

### PROPERTIES

- Mass: 9
- Dimensions (WxDxH): 3x1x3
- Cost: $500
- Tags: basic
- File: inventory_outfit_wep_black_hawk_vest.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Outfit Inventory (Bomb Disposal)

An outfit inventory unit containing specialist millitary clothing for explosive protection.

When equipped, damage from explosives is drastically reduced. Damage from projectiles to the body and head is slightly reduced. Wearing the outfit greatly limits movement speed.

### PROPERTIES

- Mass: 9
- Dimensions (WxDxH): 3x1x3
- Cost: $1500
- Tags: basic
- File: inventory_outfit_wep_bomb_disposal.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Outfit Inventory (Chest Rig)

An outfit inventory unit containing specialist millitary clothing for projectile protection.

When equipped, damage from projectiles to the body is reduced slightly and damage to the head is significantly reduced.

### PROPERTIES

- Mass: 9
- Dimensions (WxDxH): 3x1x3
- Cost: $500
- Tags: basic
- File: inventory_outfit_wep_chest_rig.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Outfit Inventory (Diving)

An outfit inventory unit containing specialist diving equipment.

When equipped, it will allow deep sea diving to a depth of 230m, and provides air for 10 minutes. The air tank can be refilled by storing the gear in an outfit inventory unit with an attached air input or via space seat.

### PROPERTIES

- Mass: 9
- Dimensions (WxDxH): 3x1x3
- Cost: $2000
- Tags: basic
- File: inventory_outfit_diving.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |
| fluid | Fluid In |  |

## Outfit Inventory (Empty)

An empty outfit storage unit.

Interacting with [q]/[e] will equip/store the selected outfit. Only specialist outfits can be stored in this unit. When connected to an electric power source, any rechargable outfits stored in the unit will drain a small amount of electricity until recharged to 100% capacity.

### PROPERTIES

- Mass: 9
- Dimensions (WxDxH): 3x1x3
- Cost: $50
- Tags: basic
- File: inventory_outfit.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Outfit Inventory (Firefighter SCBA)

An outfit inventory unit containing specialist firefighting gear.

When equipped, it will absorb 95% of damage dealt by fires, and provides breathable air for the user. The air tank can be refilled by storing the gear in an outfit inventory unit.

### PROPERTIES

- Mass: 9
- Dimensions (WxDxH): 3x1x3
- Cost: $1000
- Tags: basic
- File: inventory_outfit_firefighter_scba.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |
| fluid | Fluid In |  |

## Outfit Inventory (Firefighter)

An outfit inventory unit containing specialist firefighting gear.

When equipped, it will absorb 95% of damage dealt by fires.

### PROPERTIES

- Mass: 9
- Dimensions (WxDxH): 3x1x3
- Cost: $500
- Tags: basic
- File: inventory_outfit_firefighter.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Outfit Inventory (Hazmat)

An outfit inventory unit containing specialist hazmat gear.

When equipped, it will absorb 95% of incoming radiation.

### PROPERTIES

- Mass: 9
- Dimensions (WxDxH): 3x1x3
- Cost: $500
- Tags: basic,radiation
- File: inventory_outfit_hazmat.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Outfit Inventory (Parachute)

An outfit inventory unit containing a single-use parachute.

When selected, press [lmb] while falling to deploy the parachute. It will then open when you are falling fast enough. Press [r] to close the parachute. This parachute is single-use once equipped but can be refolded by storing it in an outfit inventory unit.

### PROPERTIES

- Mass: 9
- Dimensions (WxDxH): 3x1x3
- Cost: $500
- Tags: basic
- File: inventory_outfit_parachute.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Outfit Inventory (Plate Vest)

An outfit inventory unit containing specialist millitary clothing for projectile protection.

When equipped, damage from projectiles to the body is reduced significantly and damage to the head is greatly reduced.  Wearing the outfit significantly limits movement speed.

### PROPERTIES

- Mass: 9
- Dimensions (WxDxH): 3x1x3
- Cost: $800
- Tags: basic
- File: inventory_outfit_wep_plate_vest.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Outfit Inventory (Scuba)

An outfit inventory unit containing specialist scuba gear.

When equipped, it will allow diving to a depth of 40m, and provides air for 2 minutes. The air tank can be refilled by storing the gear in an outfit inventory unit with an attached air input or via space seat.

### PROPERTIES

- Mass: 9
- Dimensions (WxDxH): 3x1x3
- Cost: $500
- Tags: basic
- File: inventory_outfit_scuba.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |
| fluid | Fluid In |  |

## Outfit Inventory (Space Exploration)

An outfit inventory unit containing specialist Space Exploration gear required for surviving in space. The air tank can be refilled by storing the gear in an outfit inventory unit with an attached air input or via space seat.

When equipped, it will protect against low temperatures, low pressures and provide oxygen.

### PROPERTIES

- Mass: 9
- Dimensions (WxDxH): 3x1x3
- Cost: $10000
- Tags: space
- File: inventory_outfit_space_suit_exploration.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |
| fluid | Fluid In |  |

## Outfit Inventory (Space)

An outfit inventory unit containing specialist Space Exploration gear required for surviving in space. The air tank can be refilled by storing the gear in an outfit inventory unit with an attached air input or via space seat.

When equipped, it will protect against low temperatures, low pressures and provide oxygen.

### PROPERTIES

- Mass: 9
- Dimensions (WxDxH): 3x1x3
- Cost: $5000
- Tags: space
- File: inventory_outfit_space_suit.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |
| fluid | Fluid In |  |

## Padded Seat

A small padded passenger seat.

You can get in and out of the seat by interacting with it using [f]. You can place a rescued survivor in any seat by using [f] while carrying them.

### PROPERTIES

- Mass: 2
- Dimensions (WxDxH): 2x2x4
- Cost: $25
- Tags: basic,seat
- File: seat_padded.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Occupied | Outputs an on signal if this seat is occupied by a character. |

## Passenger Seat

A basic passenger seat.

You can get in and out of the seat by interacting with it using [f]. You can place a rescued survivor in any seat by using [f] while carrying them.

### PROPERTIES

- Mass: 6
- Dimensions (WxDxH): 3x3x5
- Cost: $50
- Tags: basic,seat
- File: seat_passenger.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Occupied | Outputs an on signal if this seat is occupied by a character. |

## RCS Thruster

A fluid jet that fires pressurized air for altitude control and translation.

The reaction control system can fire in 4 non-cardinal directions resulting in 5 directions of motion. RCS thrusters also have body relative activation modes where thrusters will collaborate from different orientations to achieve the desired translation or rotation. The RCS thruster also has positional and rotational stabilization toggles.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $140
- Tags: 
- File: rcs_thruster.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| composite | Composite Input | Composite bool channels: 1:Component X+, 2:Component X-, 3:Component Z+, 4:Component Z-, 5:Enable position stabilization, 6:Enable rotation stabilization, 7:Body X+, 8:Body X-, 9:Body Y+, 10:Body Y-, 11:Body Z+, 12:Body Z-, 13:Body Rotate X+, 14:Body Rotate X-, 15:Body Rotate Y+, 16:Body Rotate Y-, 17:Body Rotate Z+, 18:Body Rotate Z- |

### connections

| Type | Label | Description |
| --- | --- | --- |
| fluid | Fluid Supply | The fluid input to output from the thruster. |
| electric | Electric | Electrical power connection. |

## Rope Anchor

An anchor point for a basic rope.

Draw a rope logic link between two Rope Anchors to form a rope.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x2
- Cost: $15
- Tags: basic
- File: rope_hook.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Detach Rope |  |

### connections

| Type | Label | Description |
| --- | --- | --- |
| rope | Rope Node |  |

## Rope Pulley

A pulley that changes attached rope lengths based on forces applied to ropes.

Draw a rope logic link between two rope nodes to form a rope. Ropes will slide based on difference in force applied to each rope.

### PROPERTIES

- Mass: 25
- Dimensions (WxDxH): 3x3x1
- Cost: $250
- Tags: basic
- File: winch_pulley.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Rope 1 Length | The current length of rope 1 in metres. |
| number | Rope 2 Length | The current length of rope 2 in metres. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| rope | Rope 2 |  |
| rope | Rope 1 |  |

## Rope Pulley (Corner)

A pulley that changes attached rope lengths based on forces applied to ropes.

Draw a rope logic link between two rope nodes to form a rope. Ropes will slide based on difference in force applied to each rope.

### PROPERTIES

- Mass: 25
- Dimensions (WxDxH): 3x3x1
- Cost: $250
- Tags: basic
- File: winch_pulley_corner.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| number | Rope 1 Length | The current length of rope 1 in metres. |
| number | Rope 2 Length | The current length of rope 2 in metres. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| rope | Rope 2 |  |
| rope | Rope 1 |  |

## Rotating Light

A rotating light that can be controlled using an on/off signal.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $50
- Tags: beacon,warning
- File: rotating_light.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Light Switch | Controls whether or not the light is switched on. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Saddle Passenger Seat

A small padded passenger seat.

You can get in and out of the seat by interacting with it using [f]. You can place a rescued survivor in any seat by using [f] while carrying them.

### PROPERTIES

- Mass: 3
- Dimensions (WxDxH): 3x2x4
- Cost: $25
- Tags: basic,seat
- File: seat_saddle_passenger.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Occupied | Outputs an on signal if the seat is occupied by a character. |

## Sail Anchor

An anchor point for a sail.

Draw a rope logic link between four Sail Anchors in a loop to form a sail. A sail will convert force from the wind to the direction of the sail facing. The sail force is strongest when fully facing the wind to act as a parachute, but also has a strong force when facing slightly off a right-angle from the wind to act as a wing. A keel is recommended for sailboats to apply sail forces in a useful direction.

### PROPERTIES

- Mass: 3
- Dimensions (WxDxH): 1x1x2
- Cost: $50
- Tags: basic
- File: rope_hook_sail.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Take In/Out Sails | While active, allows the ropes forming the sail to spool freely. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| rope | Sail Node |  |

## Search Light

A spotlight that can be rotated up and down.

The light has a standard value input that sets the target orientation within the its range of motion. It can rotate a quarter turn in both directions. An on/off signal is used to switch the light on and off. It has a range of 120m.

### PROPERTIES

- Mass: 20
- Dimensions (WxDxH): 3x3x3
- Cost: $30
- Tags: spotlight,basic
- File: searchlight.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Light Switch | Controls whether or not the light is switched on. |
| number | Rotation | Standard value between -1 and 1 representing the target orientation of the light. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Siren

A warning siren with a large audible range.

It has an audible range of 3000m.

### PROPERTIES

- Mass: 5
- Dimensions (WxDxH): 3x5x3
- Cost: $200
- Tags: sound,audio
- File: siren.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Horn | Sounds the horn when recieving an on signal. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Small equipment inventory (Empty)

An empty small equipment storage unit.

Only small handheld equipment can be stored in this unit. When connected to an electric power source, any rechargable equipment stored in the unit will drain a small amount of electricity until recharged to 100% capacity.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $50
- Tags: basic
- File: inventory_small.xml

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Small Spotlight (Block)

A small spotlight that can be controlled using an on/off signal.

It has a range of 60m. Can be pivoted up to 0.125 turns using composite input.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x2
- Cost: $20
- Tags: 
- File: searchlight_small.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Light Switch | Controls whether or not the light is switched on. |
| composite | Pivot | Inputs for spotlight X/Y pivot. (Value 1 : Pivot X) (Value 2 : Pivot Y) |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Small Spotlight (Mounted)

A small spotlight that can be controlled using an on/off signal.

It has a range of 60m. Can be pivoted up to 0.125 turns using composite input.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $20
- Tags: 
- File: searchlight_small_2.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Light Switch | Controls whether or not the light is switched on. |
| composite | Pivot | Inputs for spotlight X/Y pivot. (Value 1 : Pivot X) (Value 2 : Pivot Y) |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Small Winch

A mechanical winch that can transfer electric/fluid through an attached cable, with an extension length of 10m.

Draw a rope logic link between two Rope Nodes to form a cable. Can be extended and retracted.

### PROPERTIES

- Mass: 10
- Dimensions (WxDxH): 1x1x2
- Cost: $100
- Tags: 
- File: rope_hook_winch_small.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Down | Lowers the winch cable down when receiving an on signal. |
| on/off | Up | Raises the winch cable up when receiving an on signal. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| rope | Rope Node |  |
| electric | Electric Node |  |
| fluid | Fluid | Fluid connection for the hose coil. |

## Sonar Noisemaker

A distracting device for sonar.

Emits a very loud noise at an inaudible frequency when activated, as a decoy or distraction for sonar components that are listening passively.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x3x1
- Cost: $250
- Tags: 
- File: sonar_jammer.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Enable | Enable the noisemaker. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical connection. |

## Stretcher

A strecher that connects below an attachment point.

You can get in and out of the stretcher by interacting with it using [f]. You can place a rescued survivor in any stretcher by using [f] while carrying them.

### PROPERTIES

- Mass: 80
- Dimensions (WxDxH): 3x7x3
- Cost: $250
- Tags: basic
- File: seat_stretcher.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Occupied | Outputs an on signal if this bed is occupied by a character. |

## Transponder

An emergency search and rescue transponder.

When activated, emits a continuous transponder signal that can be detected over great distances by any transponder locator.

### PROPERTIES

- Mass: 1
- Dimensions (WxDxH): 1x1x1
- Cost: $20
- Tags: basic,mission
- File: transponder.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Active | Emit a continuous transponder signal when active. |

### connections

| Type | Label | Description |
| --- | --- | --- |
| electric | Electric | Electrical power connection. |

## Vehicle Parachute

A single-use parachute that can be deployed to reduce a vehicle's velocity.

The parachute will deploy when receiving an on signal, and will close when not. Once deployed, it will open at a speed of 20m/s and stall when it drops below 5m/s. Once opened, the single use will be consumed and it must be returned to a workbench to be refolded. The size of the parachute can be customised by selecting this component with the select tool.

### PROPERTIES

- Mass: 5
- Dimensions (WxDxH): 3x3x1
- Cost: $500
- Tags: 
- File: parachute.xml

### logic inputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Deploy | Deploy the parachute. The parachute will close when it stalls or stops receiving an on signal. |

## Hose (Deprecated)

> [!WARNING]
> This component is deprecated.

A building block attached to the end of a mechanical hose that can be raised and lowered.

This can be used to transport water between Two bodies. Two on/off signals are used to control whether the hose is moving up (towards the base) or down (away from the base). A number output allows you to measure the hose's current length if necessary. The maximum length of the hose is 16 metres (64 blocks). The speed of the hose mechanism can be configured by selecting this component with the select tool.

### PROPERTIES

- Mass: 45
  - Parent Mass: 25
  - Child Mass: 20
- Dimensions (WxDxH): 3x5x4
  - Parent Dimensions (WxDxH): 3x3x4
  - Child Dimensions (WxDxH): 1x1x1
- Cost: $100
- Tags: 
- Parent File: water_hose.xml
- Child File: water_hose_b.xml

### logic inputs

| Body | Type | Label | Description |
| --- | --- | --- | --- |
| Parent | on/off | Hose Up | Raises the hose up when receiving an on signal. |
| Parent | on/off | Hose Down | Lowers the hose down when receiving an on signal. |

### logic outputs

| Body | Type | Label | Description |
| --- | --- | --- | --- |
| Parent | number | Hose Length | The current length of the hose in metres. |

### connections

| Body | Type | Label | Description |
| --- | --- | --- | --- |
| Parent | fluid | Fluid | Fluid connection for the hose coil. |
| Parent | electric | Electric | Electrical power connection. |
| Child | fluid | Fluid | Fluid connection for the end of the hose. |

## Huge Winch (Deprecated)

> [!WARNING]
> This component is deprecated.

A building block attached to the end of a 500m mechanical winch that can be raised and lowered.

The winch is operated electrically, and outputs its current length.

### PROPERTIES

- Mass: 420
  - Parent Mass: 400
  - Child Mass: 20
- Dimensions (WxDxH): 9x9x7
  - Parent Dimensions (WxDxH): 9x7x7
  - Child Dimensions (WxDxH): 1x1x1
- Cost: $5000
- Tags: 
- Parent File: winch_huge_a.xml
- Child File: winch_b.xml

### logic inputs

| Body | Type | Label | Description |
| --- | --- | --- | --- |
| Parent | on/off | Up | Raises the winch cable up when receiving an on signal. |
| Parent | on/off | Down | Lowers the winch cable down when receiving an on signal. |

### logic outputs

| Body | Type | Label | Description |
| --- | --- | --- | --- |
| Parent | number | Length | The current length of the winch cable in metres. |

### connections

| Body | Type | Label | Description |
| --- | --- | --- | --- |
| Parent | electric | Electric | Electrical power connection. |
| Parent | fluid | Fluid | Fluid connection for the hose coil. |
| Child | fluid | Fluid | Fluid connection for the end of the hose. |

## Large Winch (Deprecated)

> [!WARNING]
> This component is deprecated.

A building block attached to the end of a 100m mechanical winch that can be raised and lowered.

The winch is operated electrically, and outputs its current length.

### PROPERTIES

- Mass: 120
  - Parent Mass: 100
  - Child Mass: 20
- Dimensions (WxDxH): 3x4x4
  - Parent Dimensions (WxDxH): 3x3x4
  - Child Dimensions (WxDxH): 1x1x1
- Cost: $800
- Tags: 
- Parent File: winch_large_a.xml
- Child File: winch_b.xml

### logic inputs

| Body | Type | Label | Description |
| --- | --- | --- | --- |
| Parent | on/off | Up | Raises the winch cable up when receiving an on signal. |
| Parent | on/off | Down | Lowers the winch cable down when receiving an on signal. |

### logic outputs

| Body | Type | Label | Description |
| --- | --- | --- | --- |
| Parent | number | Length | The current length of the winch cable in metres. |

### connections

| Body | Type | Label | Description |
| --- | --- | --- | --- |
| Parent | electric | Electric | Electrical power connection. |
| Parent | fluid | Fluid | Fluid connection for the hose coil. |
| Child | fluid | Fluid | Fluid connection for the end of the hose. |

## Medium Winch (Deprecated)

> [!WARNING]
> This component is deprecated.

A building block attached to the end of a 20m mechanical winch that can be raised and lowered.

The winch is operated electrically, and outputs its current length.

### PROPERTIES

- Mass: 40
  - Parent Mass: 20
  - Child Mass: 20
- Dimensions (WxDxH): 3x3x2
  - Parent Dimensions (WxDxH): 3x1x2
  - Child Dimensions (WxDxH): 1x1x1
- Cost: $250
- Tags: 
- Parent File: winch_a.xml
- Child File: winch_b.xml

### logic inputs

| Body | Type | Label | Description |
| --- | --- | --- | --- |
| Parent | on/off | Up | Raises the winch cable up when receiving an on signal. |
| Parent | on/off | Down | Lowers the winch cable down when receiving an on signal. |

### logic outputs

| Body | Type | Label | Description |
| --- | --- | --- | --- |
| Parent | number | Length | The current length of the winch cable in metres. |

### connections

| Body | Type | Label | Description |
| --- | --- | --- | --- |
| Parent | electric | Electric | Electrical power connection. |
| Parent | fluid | Fluid | Fluid connection for the hose coil. |
| Child | fluid | Fluid | Fluid connection for the end of the hose. |

## Passenger Seat (Deprecated)

> [!WARNING]
> This component is deprecated.

A basic passenger seat.

You can get in and out of the seat by interacting with it using [f]. You can place a rescued survivor in any seat by using [f] while carrying them.

### PROPERTIES

- Mass: 20
- Dimensions (WxDxH): 3x3x5
- Cost: $50
- Tags: 
- File: passenger_seat.xml

### logic outputs

| Type | Label | Description |
| --- | --- | --- |
| on/off | Occupied | Outputs an on signal if this seat is occupied by a character. |

## Small Winch (Deprecated)

> [!WARNING]
> This component is deprecated.

A building block attached to the end of a 10m mechanical winch that can be raised and lowered.

The winch is operated electrically, and outputs its current length.

### PROPERTIES

- Mass: 30
  - Parent Mass: 10
  - Child Mass: 20
- Dimensions (WxDxH): 1x3x2
  - Parent Dimensions (WxDxH): 1x1x2
  - Child Dimensions (WxDxH): 1x1x1
- Cost: $100
- Tags: 
- Parent File: winch_electric.xml
- Child File: winch_electric_b.xml

### logic inputs

| Body | Type | Label | Description |
| --- | --- | --- | --- |
| Parent | on/off | Up |  |
| Parent | on/off | Down |  |

### connections

| Body | Type | Label | Description |
| --- | --- | --- | --- |
| Parent | electric | Electric | Electrical power connection. |
| Parent | fluid | Fluid | Fluid connection for the hose coil. |
| Child | fluid | Fluid | Fluid connection for the end of the hose. |
