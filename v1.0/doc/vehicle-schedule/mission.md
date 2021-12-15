# [mqtt-msg](../../../README.md)/[v1.0](../../README.md)/[Vehicle schedule](../vehicle-schedule/README.md)/Mission

MQTT topic                                          | Retain      | QoS
| :------------------------------------------------ |-------------| -------- |
```holo/ruter/{vehicleId}/mission```  | ```false``` | ```2```


# Mission Schema

`VehicleActivity` ([Mission](mission.md)) defined in [mission.json](../../schema/vehicle-schedule/mission.json)



## Mission Examples

```json
{
  "id": "mission12334343",
  "type": "mission",
  "status": "PENDING",
  "datetime": "2021-05-19T12:45:50Z",
  "traceId": "addf-df123456",
  "usageType": "stopCompletely",
  "stops": [{"usageType":"stopCompletely", "stopId":"Stop1"}, {"usageType":"driveThrough", "stopId":"Stop2"}],
  "reason": ""
}
```

# Mission Properties

| Property                          | Type      | Required | Nullable       | Defined by                                                                                                   |
| :-------------------------------- | --------- | -------- | -------------- | :----------------------------------------------------------------------------------------------------------- |
| [stops](#stops) | `array`  | Required | cannot be null | [Mission](mission-properties-stops.md "\#/properties/usageType#/properties/stops") |
| [usageType](#usageType) | `string`  | Required | cannot be null | [Mission](mission-properties-usageType.md "\#/properties/usageType#/properties/usageType") |
| [stopId](#stopId) | `string`  | Required | cannot be null | [Mission](mission-properties-stopId.md "\#/properties/stopId#/properties/stopId") |
| [reason](#reason) | `string`  | Required | can be empty | [Mission](mission-properties-reason.md "\#/properties/reason#/properties/reason") |

## stops
`stops`

-   is required
-   Type: `array`
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
-   cannot be empty
-   defined in:   [Mission](mission-properties-reason.md "\#/properties/reason#/properties/reason")