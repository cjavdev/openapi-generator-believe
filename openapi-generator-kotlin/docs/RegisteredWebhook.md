
# RegisteredWebhook

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | When the webhook was registered |  |
| **eventTypes** | [**inline**](#kotlin.collections.List&lt;EventTypes&gt;) | List of event types this webhook is subscribed to |  |
| **id** | **kotlin.String** | Unique webhook identifier |  |
| **secret** | **kotlin.String** | The secret key for verifying webhook signatures (base64 encoded) |  |
| **url** | [**java.net.URI**](java.net.URI.md) | The URL to send webhook events to |  |
| **description** | **kotlin.String** |  |  [optional] |


<a id="kotlin.collections.List<EventTypes>"></a>
## Enum: event_types
| Name | Value |
| ---- | ----- |
| eventTypes | match.completed, team_member.transferred |



