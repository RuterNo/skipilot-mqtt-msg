# [mqtt-msg](../../../README.md)/[v1.0](../../README.md)/[Vehicle schedule](../vehicle-schedule/README.md)/Pickup

MQTT topic                                          | Retain      | QoS
| :------------------------------------------------ |-------------| -------- |
```holo/ruter/{vehicleId}/pickup```  | ```false``` | ```2```



# Pickup Schema

`VehicleActivity` ([Pickup](pickup.md)) defined in [pickup.json](../../schema/vehicle-schedule/pickup.json)



## Pickup Examples

```json
{
  "id": "pickup12334343",
  "type": "pickup",
  "status": "PENDING",
  "datetime": "2021-05-19T12:45:50Z",
  "traceId": "addf-df123456",
  "bookingRef": "booking-1233"
}
```

# Pickup Properties

| Property                          | Type      | Required | Nullable       | Defined by                                                                                                   |
| :-------------------------------- | --------- | -------- | -------------- | :----------------------------------------------------------------------------------------------------------- |
| [bookingRef](#bookingRef) | `string`  | Required | cannot be null | [Pickup](pickup-properties-bookingRef.md "\#/properties/bookingRef#/properties/bookingRef") |

## bookingRef

`bookingRef`

-   is required
-   Type: `string`
-   cannot be null
-   defined in:   [Pickup](pickup-properties-bookingRef.md "\#/properties/bookingRef#/properties/bookingRef")