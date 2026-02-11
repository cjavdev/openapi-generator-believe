

# TriggerEventResponse

Response after triggering webhook events.

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**deliveries** | [**List&lt;WebhookDeliveryResult&gt;**](WebhookDeliveryResult.md) | Results of webhook deliveries |  |
|**eventId** | **String** | Unique event identifier |  |
|**eventType** | [**EventTypeEnum**](#EventTypeEnum) | The type of event triggered |  |
|**successfulDeliveries** | **Integer** | Number of successful deliveries |  |
|**tedSays** | **String** | Ted&#39;s reaction |  |
|**totalWebhooks** | **Integer** | Total number of webhooks that received this event |  |



## Enum: EventTypeEnum

| Name | Value |
|---- | -----|
| MATCH_COMPLETED | &quot;match.completed&quot; |
| TEAM_MEMBER_TRANSFERRED | &quot;team_member.transferred&quot; |



