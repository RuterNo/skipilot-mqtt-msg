# [tp-api](../../../../README.md) / [skipilot](../../../README.md) / [v2.0](../../README.md)/[booking-details](README.md) / Booking

MQTT topic                                          | Retain   | QoS| Producer   | Consumer
| :------------------------------------------------ | -------- | -------- | -------- | --------
```ruter/konsentra/av/{vin}/vehicle_schedule/booking```  | ```true``` | ```2``` | ```Konsentra``` | ```Ruter```

* vin = Vehicle ID

# Booking Schema

`object` ([Booking](booking.md)) defined in [booking.json](../../schema/booking-details/booking.json)

## Booking Examples

```json
{
  "id": "booking1233",
  "name": "Ola Hansen",
  "from": "PENDING",
  "to": "2021-05-19T12:45:50Z",
  "status": "Active",
  "traceId": "addf-df123456",
  "datetime": "2021-05-19T12:45:50Z"
}
```

# Mission Properties

| Property                          | Type      | Required | Nullable       | Defined by                                                                                                   |
| :-------------------------------- | --------- | -------- | -------------- | :----------------------------------------------------------------------------------------------------------- |
| [id](#id) | `string`  | Required | cannot be null | [Booking](booking-properties-id.md "\#/properties/id#/properties/id") |
| [name](#name) | `string`  | Required | cannot be null | [Booking](booking-properties-name.md "\#/properties/name#/properties/name") |
| [from](#from) | `string`  | Required | cannot be null | [Booking](booking-properties-from.md "\#/properties/from#/properties/from") |
| [to](#to) | `string`  | Required | cannot be null | [Booking](booking-properties-to.md "\#/properties/to#/properties/to") |
| [status](#status) | `string`  | Required | cannot be null | [Booking](booking-properties-status.md "\#/properties/status#/properties/status") |
| [traceId](#traceId) | `string`  | Required | cannot be null | [Booking](booking-properties-traceId.md "\#/properties/traceId#/properties/traceId") |
| [datetime](#datetime) | `string`  | Required | cannot be null | [Booking](booking-properties-datetime.md "\#/properties/datetime#/properties/datetime") |


## id

`id`

-   is required
-   Type: `string`
-   cannot be null
-   defined in:  [Booking](booking-properties-id.md "\#/properties/id#/properties/id")

## name

`name`

- is required
- Type: `string`
- cannot be null
- defined in:  [Booking](booking-properties-name.md "\#/properties/name#/properties/name")

## from

`from`

- is required
- Type: `string`
- cannot be null
- defined in:  [Booking](booking-properties-from.md "\#/properties/from#/properties/from")

## to

`to`

- is required
- Type: `string`
- cannot be null
- defined in:  [Booking](booking-properties-to.md "\#/properties/to#/properties/to")

## status

`status`

- is required
- Type: `string`
- cannot be null
- defined in:  [Booking](booking-properties-status.md "\#/properties/status#/properties/status")

## traceId

`traceId`

- is required
- Type: `string`
- cannot be null
- defined in:  [Booking](booking-properties-traceId.md "\#/properties/traceId#/properties/traceId")

## datetime

`datetime`

- is required
- Type: `string`
- cannot be null
- defined in:  [Booking](booking-properties-datetime.md "\#/properties/datetime#/properties/datetime")


