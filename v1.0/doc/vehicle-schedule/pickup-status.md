# [tp-api](../../../../README.md) / [skipilot](../../../README.md) / [v1.0](../../README.md)/[Vehicle schedule](../vehicle-schedule/README.md) / Pickup Status

MQTT topic                                          | Retain   | QoS
| :------------------------------------------------ | -------- | -------- |
```ruter/udrive/{vehicleId}/{pickupId}/pickup_status```  | ```true``` | ```1```


# PickupStatus Schema

`object` ([PickupStatus](pickup-status.md)) defined in [pickup-status.json](../../schema/vehicle-schedule/pickup-status.json)



## PickupStatus Examples

```json
{
  "status": "PENDING",
  "traceId": "addf-df123456",
  "datetime": "2021-05-19T12:45:50Z"
}
```

# PickupStatus Properties

| Property                          | Type      | Required | Nullable       | Defined by                                                                                                   |
| :-------------------------------- | --------- | -------- | -------------- | :----------------------------------------------------------------------------------------------------------- |
| [status](#status) | `string`  | Required | cannot be null | [PickupStatus](pickup-status-properties-status.md "\#/properties/status#/properties/status") |
| [traceId](#traceId) | `string`  | Required | cannot be null | [PickupStatus](pickup-status-traceId-properties-traceId.md "\#/properties/traceId#/properties/traceId") |
| [datetime](#datetime) | `string`  | Required | cannot be null | [PickupStatus](pickup-status-datetime-properties-datetime.md "\#/properties/datetime#/properties/datetime") |

## status

`status`

-   is required
-   Type: `string`
-   cannot be null
-   defined in:   [PickupStatus](pickup-status-properties-status.md "\#/properties/status#/properties/status")

### status Examples

```json
"PLANNED"
```
```json
"NOSHOW"
```
```json
"COMPLETED"
```

## traceId

`traceId`

-   is required
-   Type: `string`
-   cannot be null
-   defined in:  [PickupStatus](pickup-status-properties-traceId.md "\#/properties/traceId#/properties/traceId")


## datetime

ISO 8601, UTC


`datetime`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [PickupStatus](pickup-status-properties-datetime.md "\#/properties/datetime#/properties/datetime")
