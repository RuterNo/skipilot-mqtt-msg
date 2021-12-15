# [tp-api](../../../../README.md) / [skipilot](../../../README.md) / [v2.0](../../README.md)/[booking-details](README.md) / Booking Status

MQTT topic                                          | Retain   | QoS| Producer   | Consumer
| :------------------------------------------------ | -------- | -------- | -------- | --------
```ruter/konsentra/av/{vin}/vehicle_schedule/{bid}/booking_status```  | ```true``` | ```2``` | ```Konsentra``` | ```Ruter```

* vin = Vehicle ID
* bid = Booking ID

# BookingStatus Schema

`object` ([BookingStatus](booking-status.md)) defined in [booking-status.json](../../schema/booking-details/booking-status.json)

## BookingStatus Examples

```json
{
  "status": "Active",
  "traceId": "addf-df123456",
  "datetime": "2021-05-19T12:45:50Z"
}
```

# Booking Status Properties

| Property                          | Type      | Required | Nullable       | Defined by                                                                                                   |
| :-------------------------------- | --------- | -------- | -------------- | :----------------------------------------------------------------------------------------------------------- |
| [status](#status) | `string`  | Required | cannot be null | [Booking Status](booking-status-properties-status.md "\#/properties/status#/properties/status") |
| [traceId](#traceId) | `string`  | Required | cannot be null | [Booking Status](booking-status-properties-traceId.md "\#/properties/traceId#/properties/traceId") |
| [datetime](#datetime) | `string`  | Required | cannot be null | [Booking Status](booking-status-properties-datetime.md "\#/properties/datetime#/properties/datetime") |

## status

`status`

- is required
- Type: `string`
- cannot be null
- defined in:  [BookingStatus](booking-status-properties-status.md "\#/properties/status#/properties/status")

## traceId

`traceId`

- is required
- Type: `string`
- cannot be null
- defined in:  [BookingStatus](booking-status-properties-traceId.md "\#/properties/traceId#/properties/traceId")

## datetime

`datetime`

- is required
- Type: `string`
- cannot be null
- defined in:  [BookingStatus](booking-status-properties-datetime.md "\#/properties/datetime#/properties/datetime")

