

# RegisteredWebhook

A registered webhook endpoint.

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**createdAt** | **OffsetDateTime** | When the webhook was registered |  |
|**description** | **String** |  |  [optional] |
|**eventTypes** | [**List&lt;EventTypesEnum&gt;**](#List&lt;EventTypesEnum&gt;) | List of event types this webhook is subscribed to |  |
|**id** | **String** | Unique webhook identifier |  |
|**secret** | **String** | The secret key for verifying webhook signatures (base64 encoded) |  |
|**url** | **URI** | The URL to send webhook events to |  |



## Enum: List&lt;EventTypesEnum&gt;

| Name | Value |
|---- | -----|
| MATCH_COMPLETED | &quot;match.completed&quot; |
| TEAM_MEMBER_TRANSFERRED | &quot;team_member.transferred&quot; |



