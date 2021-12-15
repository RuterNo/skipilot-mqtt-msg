# [mqtt-msg](../../../README.md)/[v1.0](../../README.md)/[Vehicle schedule](../vehicle-schedule/README.md)/Dropoff
MQTT topic                                          | Retain      | QoS
| :------------------------------------------------ |-------------| -------- |
```holo/ruter/{vehicleId}/dropoff```  | ```false``` | ```2```




# Dropoff Schema

`VehicleActivity` ([Dropoff](dropoff.md)) defined in [dropoff.json](../../schema/vehicle-schedule/dropoff.json)

## Dropoff Examples

```json
{
  "id": "dropoff12334343",
  "type": "dropoff",
  "status": "PENDING",
  "datetime": "2021-05-19T12:45:50Z",
  "traceId": "addf-df123456",
  "bookingRef": "booking-1233"
}
```

# Dropoff Properties

| Property                          | Type      | Required | Nullable       | Defined by                                                                                                   |
| :-------------------------------- | --------- | -------- | -------------- | :----------------------------------------------------------------------------------------------------------- |
| [bookingRef](#bookingRef) | `string`  | Required | cannot be null | [Dropoff](dropoff-properties-bookingRef.md "\#/properties/bookingRef#/properties/bookingRef") |

## bookingRef

`bookingRef`

-   is required
-   Type: `string`
-   cannot be null
-   defined in:   [Dropoff](dropoff-properties-bookingRef.md "\#/properties/bookingRef#/properties/bookingRef")
