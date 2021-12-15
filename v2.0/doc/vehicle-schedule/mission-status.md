# [mqtt-msg](../../../README.md)/[v2.0](../../README.md)/[Vehicle schedule](../vehicle-schedule/README.md)/Mission Status

MQTT topic                                          | Retain      | QoS
| :------------------------------------------------ |-------------| -------- |
```ruter/holo/av/{vin}/vehicle_schedule/{vaid}/mission_status```  | ```false``` | ```2```

# MissionStatus Schema

`object` ([MissionStatus](mission-status.md)) defined in [mission-status.json](../../schema/vehicle-schedule/mission-status.json)



## MissionStatus Examples

```json
{
  "status": "COMPLETED",
  "traceId": "addf-df123456",
  "datetime": "2021-05-19T12:45:50Z"
}
```

# MissionStatus Properties

| Property                          | Type      | Required | Nullable       | Defined by                                                                                                   |
| :-------------------------------- | --------- | -------- | -------------- | :----------------------------------------------------------------------------------------------------------- |
| [status](#status) | `string`  | Required | cannot be null | [MissionStatus](mission-status-properties-status.md "\#/properties/status#/properties/status") |
| [traceId](#traceId) | `string`  | Required | cannot be null | [MissionStatus](mission-status-traceId-properties-traceId.md "\#/properties/traceId#/properties/traceId") |
| [datetime](#datetime) | `string`  | Required | cannot be null | [MissionStatus](mission-status-datetime-properties-datetime.md "\#/properties/datetime#/properties/datetime") |

## status

`status`

-   is required
-   Type: `string`
-   cannot be null
-   defined in:   [MissionStatus](mission-status-properties-status.md "\#/properties/status#/properties/status")

### status Examples

```json
"PENDING"
```
```json
"ACCEPTED"
```
```json
"REJECTED"
```
```json
"IN_PROGRESS"
```
```json
"INTERRUPTED"
```
```json
"COMPLETED"
```

## traceId

`traceId`

-   is required
-   Type: `string`
-   cannot be null
-   defined in:  [MissionStatus](mission-status-properties-traceId.md "\#/properties/traceId#/properties/traceId")

## datetime

ISO 8601, UTC


`datetime`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [MissionStatus](mission-status-properties-datetime.md "\#/properties/datetime#/properties/datetime")