# [mqtt-msg](../../../README.md)/[v2.0](../../README.md)/[Vehicle schedule](../vehicle-schedule/README.md) / Mission

MQTT topic                                          | Retain      | QoS| Producer   | Consumer
| :------------------------------------------------ |-------------| -------- | -------- | --------
```ruter/konsentra/av/{vin}/vehicle_schedule/vehicle_activity```  | ```false``` | ```2``` | ```Konsentra``` | ```Ruter```
```holo/ruter/av/{vin}/vehicle_schedule/mission```  | ```false``` | ```2``` | ```Ruter``` | ```Holo```
```konsentra/ruter/av/{vin}/vehicle_schedule/mission```  | ```false``` | ```2``` | ```Ruter``` | ```Konsentra```

# Mission Schema

`object` ([Mission](mission.md)) defined in [mission.json](../../schema/vehicle-schedule/mission.json)

inherits following fields from [VehicleActivity](vehicle-activity.md)
- id
- type
- status
- datetime
- traceId


## Mission Examples

```json
{
  "id": "mission12323",
  "type": "mission",
  "status": "PENDING",
  "datetime": "2021-05-19T12:45:50Z",
  "traceId": "addf-df123456",
  "stops": [{"usageType":"stopCompletely", "stopId":"Stop1"}, {"usageType":"driveThrough", "stopId":"Stop2"}],
  "reason": ""
}
```

# Mission Properties

| Property                          | Type      | Required | Nullable       | Defined by                                                                                                   |
| :-------------------------------- | --------- | -------- | -------------- | :----------------------------------------------------------------------------------------------------------- |
| [stops](#stopId) | `arrayList`  | Required | cannot be null | [Mission](mission-properties-stopId.md "\#/properties/stopId#/properties/stopId") |
| [reason](#reason) | `string`  | Required | can be empty | [Mission](mission-properties-reason.md "\#/properties/reason#/properties/reason") |

## stops
`stops`

-   is required
-   Type: `arrayList of usageType and stopId`
-   cannot be null
-   defined in:   [Mission](mission-properties-stops.md "\#/properties/usageType#/properties/stops")

## usageType

`usageType`

-   is required
-   Type: `string`
-   cannot be null
-   defined in:   [Mission](mission-properties-usageType.md "\#/properties/usageType#/properties/usageType") 

### usageType Examples

```json
"stopCompletely"
```
```json
"driveThrough"
```

## stopId

`stopId`

-   is required
-   Type: `string`
-   cannot be null
-   defined in:   [Mission](mission-properties-stopId.md "\#/properties/stopId#/properties/stopId")


## reason

`reason`

-   is required
-   Type: `string`
-   can be empty
-   defined in:   [Mission](mission-properties-reason.md "\#/properties/reason#/properties/reason")