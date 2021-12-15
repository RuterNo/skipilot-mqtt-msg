# [tp-api](../../../../README.md) / [skipilot](../../../README.md) / [v1.0](../../README.md)/[Vehicle schedule](../vehicle-schedule/README.md) / Dropoff Status


MQTT topic                                          | Retain   | QoS
| :------------------------------------------------ | -------- | -------- |
```ruter/udrive/{vehicleId}/{dropoffId}/dropoff_status```  | ```true``` | ```1```


# DropoffStatus Schema

`object` ([DroppoffStatus](dropoff-status.md)) defined in [dropoff-status.json](../../schema/vehicle-schedule/dropoff-status.json)



## DropoffStatus Examples

```json
{
  "status": "PENDING",
  "traceId": "addf-df123456",
  "datetime": "2021-05-19T12:45:50Z"
}
```

# DropoffStatus Properties

| Property                          | Type      | Required | Nullable       | Defined by                                                                                                   |
| :-------------------------------- | --------- | -------- | -------------- | :----------------------------------------------------------------------------------------------------------- |
| [status](#status) | `string`  | Required | cannot be null | [DropoffStatus](dropoff-status-properties-status.md "\#/properties/status#/properties/status") |
| [traceId](#traceId) | `string`  | Required | cannot be null | [DropoffStatus](dropoff-status-traceId-properties-traceId.md "\#/properties/traceId#/properties/traceId") |
| [datetime](#datetime) | `string`  | Required | cannot be null | [DropoffStatus](dropoff-status-datetime-properties-datetime.md "\#/properties/datetime#/properties/datetime") |

## status

`status`

-   is required
-   Type: `string`
-   cannot be null
-   defined in:   [DropoffStatus](dropoff-status-properties-status.md "\#/properties/status#/properties/status")

### status Examples

```json
"PLANNED"
```
```json
"RESCHEDULED"
```
```json
"COMPLETED"
```

## traceId

`traceId`

-   is required
-   Type: `string`
-   cannot be null
-   defined in:  [DropoffStatus](dropoff-status-properties-traceId.md "\#/properties/traceId#/properties/traceId")

## datetime

ISO 8601, UTC


`datetime`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [DropoffStatus](dropoff-status-properties-datetime.md "\#/properties/datetime#/properties/datetime")