# [mqtt-msg](../../../README.md)/[v2.0](../../README.md)/[Vehicle details](../vehicle-details/README.md)/Vehicle Status

MQTT topic                                          | Retain      | QoS
| :------------------------------------------------ |-------------| -------- |
```ruter/holo/av/{vin}/vehicle_status```  | ```false``` | ```2```
```konsentra/ruter/av/{vin}/vehicle_status```  | ```false``` | ```2```

# VehicleStatus Schema

`object` ([VehicleStatus](vehicle-status.md)) defined in [vehicle-status.json](../../schema/vehicle-details/vehicle-status.json)



## VehicleStatus Examples

```json
{
  "status": "READY",
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
"OFFLINE"
```
```json
"READY"
```
```json
"NOT_READY"
```
```json
"ON_MISSION"
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