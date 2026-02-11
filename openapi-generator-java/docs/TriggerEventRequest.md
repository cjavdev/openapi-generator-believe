

# TriggerEventRequest

Request to trigger a webhook event.

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**eventType** | [**EventTypeEnum**](#EventTypeEnum) | The type of event to trigger |  |
|**payload** | [**TriggerEventRequestPayload**](TriggerEventRequestPayload.md) |  |  [optional] |



## Enum: EventTypeEnum

| Name | Value |
|---- | -----|
| MATCH_COMPLETED | &quot;match.completed&quot; |
| TEAM_MEMBER_TRANSFERRED | &quot;team_member.transferred&quot; |



