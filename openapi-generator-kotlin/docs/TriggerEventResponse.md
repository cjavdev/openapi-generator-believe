
# TriggerEventResponse

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **deliveries** | [**kotlin.collections.List&lt;WebhookDeliveryResult&gt;**](WebhookDeliveryResult.md) | Results of webhook deliveries |  |
| **eventId** | **kotlin.String** | Unique event identifier |  |
| **eventType** | [**inline**](#EventType) | The type of event triggered |  |
| **successfulDeliveries** | **kotlin.Int** | Number of successful deliveries |  |
| **tedSays** | **kotlin.String** | Ted&#39;s reaction |  |
| **totalWebhooks** | **kotlin.Int** | Total number of webhooks that received this event |  |


<a id="EventType"></a>
## Enum: event_type
| Name | Value |
| ---- | ----- |
| eventType | match.completed, team_member.transferred |



