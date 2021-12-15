# [mqtt-msg](../../../README.md)/[v1.0](../../README.md)/[Vehicle schedule](../vehicle-schedule/README.md)/Vehicle Schedule

MQTT topic                                          | Retain      | QoS
| :------------------------------------------------ |-------------| -------- |
```ruter/konsentra/{vehicleId}/vehicle_schedule```  | ```false``` | ```2```
```holo/rute/{vehicleId}/vehicle_schedule```  | ```false``` | ```2```

# Vehicle Schedule Schema

`object` ([VehicleSchedule](vehicle-schedule.md)) defined in [vehicle-schedule.json](../../schema/vehicle-schedule/vehicle-schedule.json)


## VehicleSchedule Examples

```json
{
  "id": "schedule12334343",
  "status": "PENDING",
  "datetime": "2021-05-19T12:45:50Z",
  "traceId": "addf-df123456",
  "activities": [{
    "id": "mission12334343",
    "type": "mission",
    "status": "PENDING",
    "datetime": "2021-05-19T12:45:50Z",
    "traceId": "addf-df123456",
    "usageType": "stopCompletely",
    "stops": [{"usageType":"stopCompletely", "stopId":"Stop1"}, {"usageType":"driveThrough", "stopId":"Stop2"}]
  },{
    "id": "pickup12334343",
    "type": "pickup",
    "status": "PENDING",
    "datetime": "2021-05-19T12:45:50Z",
    "traceId": "addf-df123456",
    "bookingRef": "booking-1233"
  }
  ]
}
```

# VehicleSchedule Properties

| Property                          | Type      | Required | Nullable       | Defined by                                                                                                   |
| :-------------------------------- | --------- | -------- | -------------- | :----------------------------------------------------------------------------------------------------------- |
| [id](#id) | `string`  | Required | cannot be null | [VehicleSchedule](vehicle-schedule-properties-id.md "\#/properties/id#/properties/id") |
| [status](#status) | `string`  | Required | cannot be null | [VehicleSchedule](vehicle-schedule-properties-status.md "\#/properties/status#/properties/status") |
| [datetime](#datetime) | `string`  | Required | cannot be null | [VehicleSchedule](vehicle-schedule-properties-datetime.md "\#/properties/datetime#/properties/datetime") |
| [traceId](#traceId) | `string`  | Required | cannot be null | [VehicleSchedule](vehicle-schedule-properties-traceId.md "\#/properties/traceId#/properties/traceId") |
| [activities](#activities) | `string`  | Required | cannot be null | [VehicleSchedule](vehicle-schedule-properties-activities.md "\#/properties/activities#/properties/activities") |

## id

`id`

-   is required
-   Type: `string`
-   cannot be null
-   defined in:  [VehicleSchedule](vehicle-schedule-properties-id.md "\#/properties/id#/properties/id")

## status

`status`

-   is required
-   Type: `string`
-   cannot be null
-   defined in:  [VehicleSchedule](vehicle-schedule-properties-status.md "\#/properties/status#/properties/status")


## datetime

ISO 8601, UTC


`datetime`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [VehicleSchedule](vehicle-schedule-properties-datetime.md "\#/properties/datetime#/properties/datetime")


## traceId

`traceId`

-   is required
-   Type: `string`
-   cannot be null
-   defined in:  [VehicleSchedule](vehicle-schedule-properties-traceId.md "\#/properties/traceId#/properties/traceId")

## activities

`activities`

-   is required
-   Type: `array`
-   cannot be null
-   defined in:  [VehicleSchedule](vehicle-schedule-properties-activities.md "\#/properties/activities#/properties/activities")
