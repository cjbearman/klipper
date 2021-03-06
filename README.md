# Klipper configuration for ender 3 v2

This is the configuration that I use for Klipper on my customized Ender 3 V2 (SKR Mini E3 V3.0 mainboard)

Specific machine upgrades:
* Ender 3 V2
* BTT SKR PRO E2 V3.0 Mainboard
* Microswiss Direct Drive extruder
* Microswiss All Metal hot end
* Dual Z axis
* Gulfcoast Robotics HEX EPCOS Thermistor (300c capable)
* Big Tree Tech Smart Filament Sensor

Note that my last configuration that used my old creality-4.2.2 board
can be found in the creality-4.2.2 branch.


The configuration is broken up into a variety of files:

* printer.cfg - The main configuration file
* leveling.cfg - BL Touch and bed leveling settings
* filament_sensor.cfg - BTT Smart Filament Sensor
* macros.cfg - Misc macros
* start.cfg - Start script
* end.cfg - End script
* loading.cfg - Load and unload filament macros
* park.cfg - Parking, used by load/unload


# CURA configuration
Set start gcode to:
```
START_PRINT BED_TEMP={material_bed_temperature_layer_0} EXTRUDER_TEMP={material_print_temperature_layer_0}
```

Set end gcode to:
```
END_PRINT
```

# SuperSlicer configuration
Set start gcode to:
```
START_PRINT BED_TEMP=[first_layer_bed_temperature] EXTRUDER_TEMP=[first_layer_temperature_0]
```

Set end gcode to:
```
END_PRINT
```

