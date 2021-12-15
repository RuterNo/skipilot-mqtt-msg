# [mqtt-msg](../../../README.md)/[v2.0](../../README.md)/[Vehicle schedule](../vehicle-schedule/README.md) / Vehicle Schedule

MQTT topic                                          | Retain      | QoS| Producer   | Consumer   
| :------------------------------------------------ |-------------| -------- | -------- | --------
```ruter/udrive/av/{vin}/vehicle_schedule```  | ```false``` | ```2``` | ```Udrive``` | ```Ruter```
```holo/ruter/av/{vin}/vehicle_schedule```  | ```false``` | ```2``` | ```Ruter``` | ```Holo```
```konsentra/ruter/av/{vin}/vehicle_schedule```  | ```false``` | ```2``` | ```Ruter``` | ```Konsentra```


# Vehicle Schedule Schema

`object` ([VehicleSchedule](vehicle-schedule.md)) defined in [vehicle-schedule.json](../../schema/vehicle-schedule/vehicle-schedule.json)


## VehicleSchedule Examples

```json
 {
  "id": 6139,
  "runId": 1,
  "datetime": "2021-05-19T12:45:50Z",
  "traceId": "addf-df123456",
  "events": [{
    "id":  1,
    "name":  "ACT_PULLOUT",
    "bookingId": null,
    "lat":  null,
    "lon":  null,
    "estTime": null,
    "scheduledTime":  "11:16",
    "status":  1,
    "activity":  4,
    "addressName":  "",
    "onStreet":  "",
    "streetNo":  "",
    "unit":  "",
    "zipCode":  "",
    "city":  "",
    "fullAddress":  "",
    "bookingComments": null,
    "bookingLegComments":  null,
    "bookingMobilityAids":  null,
    "bookingLegMobilityAids":  null,
    "fareToCollect":  null,
    "spaceType": null
  },{
    "id":  6,
    "name":  "ACT_DROPOFF",
    "bookingId": 43,
    "lat":  null,
    "lon":  null,
    "estTime": null,
    "scheduledTime":  "12:00",
    "status":  1,
    "activity":  1,
    "addressName":  "MOTORSENTERET",
    "onStreet":  "LØXAVEIEN",
    "streetNo":  "2",
    "unit":  "",
    "zipCode":  "1352",
    "city":  "RUD, BÆRUM",
    "fullAddress":  "MOTORSENTERET LØXAVEIEN 2, 1351 RUD, BÆRUM",
    "bookingComments": null,
    "bookingLegComments":  null,
    "bookingMobilityAids":  null,
    "bookingLegMobilityAids":  null,
    "fareToCollect":  null,
    "spaceType": null
  }
  ]
}
```

# VehicleSchedule Properties

| Property                          | Type      | Required | Nullable       | Defined by                                                                                                   |
| :-------------------------------- | --------- | -------- | -------------- | :----------------------------------------------------------------------------------------------------------- |
| [id](#id) | `number`  | Required | cannot be null | [VehicleSchedule](vehicle-schedule-properties-id.md "\#/properties/id#/properties/id") |
| [runId](#runId) | `number`  | Required | cannot be null | [VehicleSchedule](vehicle-schedule-properties-runId.md "\#/properties/runId#/properties/runId") |
| [datetime](#datetime) | `string`  | Required | cannot be null | [VehicleSchedule](vehicle-schedule-properties-datetime.md "\#/properties/datetime#/properties/datetime") |
| [traceId](#traceId) | `string`  | Required | cannot be null | [VehicleSchedule](vehicle-schedule-properties-traceId.md "\#/properties/traceId#/properties/traceId") |
| [events](#events) | `array`  | Required | cannot be null | [VehicleSchedule](vehicle-schedule-properties-event.md "\#/properties/events#/properties/events") |

## id

`id`

-   is required
-   Type: `number`
-   cannot be null
-   defined in:  [VehicleSchedule](vehicle-schedule-properties-id.md "\#/properties/id#/properties/id")

## runId

`runId`

-   is required
-   Type: `number`
-   cannot be null
-   defined in:  [VehicleSchedule](vehicle-schedule-properties-runId.md "\#/properties/runId#/properties/runId")


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

## events

`events`

-   is required
-   Type: `arrayLIst of: ` [Event](../../schema/vehicle-schedule/event.json)
-   cannot be null
-   defined in:  [VehicleSchedule](vehicle-schedule-properties-event.md "\#/properties/events#/properties/events")
