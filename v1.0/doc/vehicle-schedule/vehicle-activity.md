# [mqtt-msg](../../../README.md)/[v1.0](../../README.md)/[Vehicle schedule](../vehicle-schedule/README.md)/Vehicle Activity
MQTT topic                                          | Retain      | QoS
| :------------------------------------------------ |-------------| -------- |
```ruter/konsentra/{vehicleId}/vehicle_activity```  | ```false``` | ```2```

# VehicleActivity Schema

`object` ([VehicleActivity](vehicle-activity.md)) defined in [vehicle-activity.json](../../schema/vehicle-schedule/vehicle-activity.json)



## VehicleActivity Examples

```json
{
  "id": "mission12334343",
  "type": "mission",
  "status": "PENDING",
  "datetime": "2021-05-19T12:45:50Z",
  "traceId": "addf-df123456",
  "usageType": "stopCompletely",
  "stops": [{"usageType":"stopCompletely", "stopId":"Stop1"}, {"usageType":"driveThrough", "stopId":"Stop2"}]
}
```

# VehicleActivity Properties

| Property                          | Type      | Required | Nullable       | Defined by                                                                                                   |
| :-------------------------------- | --------- | -------- | -------------- | :----------------------------------------------------------------------------------------------------------- |
| [id](#id) | `string`  | Required | cannot be null | [VehicleActivity](vehicle-activity-properties-id.md "\#/properties/id#/properties/id") |
| [type](#type) | `string`  | Required | cannot be null | [VehicleActivity](vehicle-activity-properties-type.md "\#/properties/type#/properties/type") |
| [status](#status) | `string`  | Required | cannot be null | [VehicleActivity](vehicle-activity-properties-status.md "\#/properties/status#/properties/status") |
| [datetime](#datetime) | `string`  | Required | cannot be null | [VehicleActivity](vehicle-activity-properties-datetime.md "\#/properties/datetime#/properties/datetime") |
| [traceId](#traceId) | `string`  | Required | cannot be null | [VehicleActivity](vehicle-activity-properties-traceId.md "\#/properties/traceId#/properties/traceId") |

## id

`id`

-   is required
-   Type: `string`
-   cannot be null
-   defined in:  [VehicleActivity](vehicle-activity-properties-id.md "\#/properties/id#/properties/id")

## type

`type`

-   is required
-   Type: `string`
-   cannot be null
-   defined in:  [VehicleActivity](vehicle-activity-properties-type.md "\#/properties/type#/properties/type")

### type Examples

```json
"mission"
```
```json
"pickup"
```
```json
"dropoff"
```
```json
"pullin"
```
```json
"pullout"
```
```json
"pause"
```
## status

`status`

-   is required
-   Type: `string`
-   cannot be null
-   defined in:  [VehicleActivity](vehicle-activity-properties-status.md "\#/properties/status#/properties/status")

### status Examples

| VehicleActivity| Status      | 
| :-------------------------------- | --------- | 
| Mission | ``` {'PENDING', 'ACCEPTED', 'REJECTED', 'IN_PROGRESS', 'INTERRUPTED', 'COMPLETED'} ```|
| Pickup | ``` {'PLANNED', 'NOSHOW','COMPLETED'} ```|
| Dropoff | ``` {'PLANNED', 'RESCHEDULED','COMPLETED'} ```|

## datetime

ISO 8601, UTC


`datetime`

-   is required
-   Type: `string`
-   cannot be null
-   defined in: [VehicleActivity](vehicle-activity-properties-datetime.md "\#/properties/datetime#/properties/datetime")


## traceId

`traceId`

-   is required
-   Type: `string`
-   cannot be null
-   defined in:  [VehicleActivity](vehicle-activity-properties-traceId.md "\#/properties/traceId#/properties/traceId")
