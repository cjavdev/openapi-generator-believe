# OpenapiClient::RegisteredWebhook

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **created_at** | **Time** | When the webhook was registered |  |
| **description** | **String** |  | [optional] |
| **event_types** | **Array&lt;String&gt;** | List of event types this webhook is subscribed to |  |
| **id** | **String** | Unique webhook identifier |  |
| **secret** | **String** | The secret key for verifying webhook signatures (base64 encoded) |  |
| **url** | **String** | The URL to send webhook events to |  |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::RegisteredWebhook.new(
  created_at: null,
  description: null,
  event_types: null,
  id: null,
  secret: null,
  url: null
)
```

