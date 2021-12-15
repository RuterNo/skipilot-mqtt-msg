# [mqtt-msg](../../../README.md) / [v2.0](../../README.md)/[Common](README.md) / Error

MQTT topic                                          | Retain   | QoS   | Producer | Consumer   
| :------------------------------------------------ | -------- |-------|----------| --------
[Error](error.md) | ``konsentra/ruter/av/{vin}/vehicle_schedule/vehicle_activity/error`` | false | 2        | Ruter | Konsentra
[Error](error.md) | ``holo/ruter/av/{vin}/vehicle_schedule/vehicle_activity/error``| false | 2     | Ruter    | Holo
[Error](error.md) | ``konsentra/ruter/av/{vin}/vehicle_schedule/booking/error``  | false | 2      | Ruter    | Konsentra
--- 

* vin = Vehicle ID

# Common Schema

`object` ([Error](../common/error.md)) defined in [error.json](../../schema/common/error.json)


## Error Examples

```json
 {
  "id": "error1",
  "code": "409",
  "message": "Illegal status transition, status can not be set to IN_PROGRESS from PENDING",
  "datetime": "2021-05-19T12:45:50Z",
  "traceId": "addf-df123456",
  "refEventTraceId": "afdf-df12333"
}
```

# VehicleSchedule Properties

| Property                          | Type      | Required | Nullable       | Defined by                                                                                                   |
| :-------------------------------- | --------- | -------- | -------------- | :----------------------------------------------------------------------------------------------------------- |
| [id](#id) | `string`  | Required | cannot be null | [Error](errorproperties-id.md "\#/properties/id#/properties/id") |
| [code](#code) | `string`  | Required | cannot be null | [Error](errorproperties-code.md "\#/properties/code#/properties/code") |
| [message](#message) | `string`  | Required | cannot be null | [Error](errorproperties-message.md "\#/properties/message#/properties/message") |
| [datetime](#datetime) | `string`  | Required | cannot be null | [Error](errorproperties-datetime.md "\#/properties/datetime#/properties/datetime") |
| [traceId](#traceId) | `string`  | Required | cannot be null | [Error](errorproperties-traceId.md "\#/properties/traceId#/properties/traceId") |
| [refEventTraceId](#refEventTraceId) | `string`  | Required | cannot be null | [Error](errorproperties-refEventTraceId.md "\#/properties/refEventTraceId#/properties/refEventTraceId") |

## id

`id`

-   is required
-   Type: `string`
-   cannot be null
-   defined in:  [Error](error-properties-id.md "\#/properties/id#/properties/id")

## code

`code`

-   is required
-   Type: `number`
-   cannot be null
-   defined in:  [Error](error-properties-code.md "\#/properties/code#/properties/code")

## message

`message`

-   is required
-   Type: `number`
-   cannot be null
-   defined in:  [Error](error-properties-message.md "\#/properties/message#/properties/message")


## datetime

ISO 8601, UTC


`datetime`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [Error](error-properties-datetime.md "\#/properties/datetime#/properties/datetime")


## traceId

`traceId`

-   is required
-   Type: `string`
-   cannot be null
-   defined in:  [Error](error-properties-traceId.md "\#/properties/traceId#/properties/traceId")

## refEventTraceId

`refEventTraceId`

-   is required
-   Type: `string`
-   cannot be null
-   defined in:  [Error](error-properties-refEventTraceId.md "\#/properties/refEventTraceId#/properties/refEventTraceId")
