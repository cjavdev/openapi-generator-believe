
# MatchCompletedEvent

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | When the event was created |  |
| **&#x60;data&#x60;** | [**MatchCompletedData**](MatchCompletedData.md) |  |  |
| **eventId** | [**java.util.UUID**](java.util.UUID.md) | Unique identifier for this event |  |
| **eventType** | [**inline**](#EventType) | The type of webhook event |  |


<a id="EventType"></a>
## Enum: event_type
| Name | Value |
| ---- | ----- |
| eventType | match.completed |



