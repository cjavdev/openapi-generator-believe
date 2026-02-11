

# MatchCompletedEvent

Webhook event sent when a match completes.

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**createdAt** | **OffsetDateTime** | When the event was created |  |
|**data** | [**MatchCompletedData**](MatchCompletedData.md) |  |  |
|**eventId** | **UUID** | Unique identifier for this event |  |
|**eventType** | [**EventTypeEnum**](#EventTypeEnum) | The type of webhook event |  |



## Enum: EventTypeEnum

| Name | Value |
|---- | -----|
| MATCH_COMPLETED | &quot;match.completed&quot; |



