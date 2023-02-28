# Valetudo-NodeRed-Extensions
This repo includes my extensions to the official Valetudo API.

## Flows available:
### GetRobotInfo.json 
Will calculate & return a summary info related to the robot. most importantly, calculating the current position (segment) of the robot from the map data, but also other information about the sensors maintenance.
<br>**Please change the IP address in the GetRobotState Node to your robot's IP.**

Example of returned info:
```
{
   "battery_level":100,
   "state":"docked",
   "main_brush_remaining":{"value":9900,"unit":"minutes"},
   "side_right_brush_remaining":{"value":3120,"unit":"minutes"},
   "main_filter_remaining":{"value":120,"unit":"minutes"},
   "sensor_cleanup_remaining":{"value":300,"unit":"minutes"},
   "currentLocation":{"segmentId":"14","name":"Living Area"},
   "_linkSource":[]
}
```
