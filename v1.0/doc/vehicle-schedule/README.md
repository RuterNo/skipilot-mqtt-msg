# [mqtt-msg](../../../README.md)/[v1.0](../../README.md)/Vehicle schedule

# Vehicle Schedule
## [Vehicle schedule Schema](README.md)

Schema                                | MQTT topic                                                               | Produced by | Consumed by
| :---------------------------------- | :----------------------------------------------------------------------- | ----------- | -------- |
[Vehicle schedule](vehicle-schedule.md) | ```ruter/konsentra/{vehicleId}/vehicle_schedule```  | Konsentra | Ruter
[Vehicle schedule](vehicle-schedule.md) | ```holo/ruter/{vehicleId}/vehicle_schedule```  | Ruter | Holo
[Vehicle activity](vehicle-activity.md) | ```ruter/konsentra/{vehicleId}/vehicle_activity```  | Konsentra | Ruter
[Mission](mission.md) | ```holo/ruter/{vehicleId}/mission```  | Ruter | Holo
[Mission](mission.md) | ```ruter/holo/{vehicleId}/mission```  | Holo | Ruter
[Mission](mission.md) | ```konsentra/ruter/{vehicleId}/mission```  | Ruter | Konsentra
[Pickup](pickup.md) | ```holo/ruter/{vehicleId}/pickup```  | Ruter | Holo
[Dropoff](dropoff.md) | ```holo/ruter/{vehicleId}/dropoff```  | Ruter | Holo
[Mission status](mission-status.md) | ```ruter/holo/{vehicleId}/{missionId}/mission_status```  | Holo | Ruter
[Pickup status](pickup-status.md) | ```ruter/udrive/{vehicleId}/{pickupId}/pickup_status```  | Udrive | Ruter
[Dropoff status](dropoff-status.md) | ```ruter/udrive/{vehicleId}/{dropoffId}/dropoff_status```  | Udrive | Ruter
 --- 