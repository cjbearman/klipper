# Klipper configuration for ender 3 v2

The configuration is broken up into a variety of files:

* printer.cfg - The main configuration file
* leveling.cfg - BL Touch and bed leveling settings
* filament_sensor.cfg - BTT Smart Filament Sensor
* macros.cfg - Misc macros
* start.cfg - Start script
* end.cfg - End script

# CURA configuration
Set start gcode to:
```
START_PRINT BED_TEMP={material_bed_temperature_layer_0} EXTRUDER_TEMP={material_print_temperature_layer_0}
```

Set end gcode to:
```
END_PRINT
```
