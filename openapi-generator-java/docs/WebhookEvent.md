

# WebhookEvent

Union type for all webhook events. Use the event_type field to determine the specific event type.

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**createdAt** | **OffsetDateTime** | When the event was created |  |
|**data** | [**TeamMemberTransferredData**](TeamMemberTransferredData.md) |  |  |
|**eventId** | **UUID** | Unique identifier for this event |  |
|**eventType** | [**EventTypeEnum**](#EventTypeEnum) | The type of webhook event |  |



## Enum: EventTypeEnum

| Name | Value |
|---- | -----|
| TEAM_MEMBER_TRANSFERRED | &quot;team_member.transferred&quot; |



