# [tp-api](../../../../README.md) / [skipilot](../../../README.md) / [v1.0](../../README.md)/[Vehicle details](../vehicle-details/README.md) / Vehicle Status

MQTT topic                                          | Retain   | QoS
| :------------------------------------------------ | -------- | -------- |
```ruter/holo/{vehicleId}/vehicle-status```  | ```true``` | ```1```
```konsentra/ruter/{vehicleId}/vehicle-status```  | ```true``` | ```1```

# VehicleStatus Schema

`object` ([VehicleStatus](vehicle-status.md)) defined in [vehicle-status.json](../../schema/vehicle-details/vehicle-status.json)



## VehicleStatus Examples

```json
{
  "status": "IDLE",
  "traceId": "holo-df123456",
  "datetime": "2021-05-19T12:45:50Z"
}
```

# MissionStatus Properties

| Property                          | Type      | Required | Nullable       | Defined by                                                                                                   |
| :-------------------------------- | --------- | -------- | -------------- | :----------------------------------------------------------------------------------------------------------- |
| [status](#status) | `string`  | Required | cannot be null | [VehicleStatus](vehicle-status-properties-status.md "\#/properties/status#/properties/status") |
| [traceId](#traceId) | `string`  | Required | cannot be null | [VehicleStatus](vehicle-status--traceId-properties-traceId.md "\#/properties/traceId#/properties/traceId") |
| [datetime](#datetime) | `string`  | Required | cannot be null | [VehicleStatus](vehicle-status-datetime-properties-datetime.md "\#/properties/datetime#/properties/datetime") |
| Additional Properties             | Any       | Optional | can be null    |                                                                                                              |

## usageType

`usageType`

-   is required
-   Type: `string`
-   cannot be null
-   defined in:   [VehicleStatus](vehicle-status-properties-usageType.md "\#/properties/usageType#/properties/usageType")

### usageType Type

`string`
### usageType Examples

```json
"stopCompletely"
```
```json
"driveThrough"
```

## status

`status`

-   is required
-   Type: `string`
-   cannot be null
-   defined in:   [VehicleStatus](vehicle-status-properties-status.md "\#/properties/status#/properties/status")

### status Type

`string`
### status Examples

```json
"IDLE"
```
```json
"BUSY"
```
```json
"OUT_OF_ORDER"
```

## traceId

`traceId`

-   is required
-   Type: `string`
-   cannot be null
-   defined in:  [VehicleStatus](vehicle-status-properties-traceId.md "\#/properties/traceId#/properties/traceId")

### id Type

`string`

## datetime

ISO 8601, UTC


`datetime`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [VehicleStatus](vehicle-status-properties-datetime.md "\#/properties/datetime#/properties/datetime")

### datetime Type

`string`