# [mqtt-msg](../../../README.md)/[v2.0](../../README.md)/Vehicle schedule

# Vehicle Schedule
## [Vehicle schedule Schema](README.md)

Schema                                | MQTT topic                                                               | Produced by | Consumed by
| :---------------------------------- | :----------------------------------------------------------------------- | ----------- | -------- |
[Vehicle Schedule](vehicle-schedule.md) | ```ruter/udrive/av/{vin}/vehicle_schedule```  | Udrive | Ruter
[Vehicle Schedule](vehicle-schedule.md) | ```holo/ruter/av/{vin}/vehicle_schedule```  | Ruter | Holo
[Vehicle Schedule](vehicle-schedule.md) | ```konsentra/ruter/av/{vin}/vehicle_schedule```  | Ruter | Konsentra
[Mission](mission.md) | ```ruter/konsentra/av/{vin}/vehicle_schedule/vehicle_activity```  | Konsentra | Ruter
[Mission](mission.md) | ```holo/ruter/av/{vin}/vehicle_schedule/mission```  | Ruter | Holo
[Mission](mission.md) | ```konsentra/ruter/av/{vin}/vehicle_schedule/mission```  | Ruter | Konsentra
[Mission Status](mission-status.md) | ```ruter/holo/av/{vin}/vehicle_schedule/{vaid}/mission_status```  | Holo | Ruter
 --- 