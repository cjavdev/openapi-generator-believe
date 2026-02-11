

# WebhookRegistrationRequest

Request to register a new webhook endpoint.

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**description** | **String** |  |  [optional] |
|**eventTypes** | [**List&lt;EventTypesEnum&gt;**](#List&lt;EventTypesEnum&gt;) |  |  [optional] |
|**url** | **URI** | The URL to send webhook events to |  |



## Enum: List&lt;EventTypesEnum&gt;

| Name | Value |
|---- | -----|
| MATCH_COMPLETED | &quot;match.completed&quot; |
| TEAM_MEMBER_TRANSFERRED | &quot;team_member.transferred&quot; |



