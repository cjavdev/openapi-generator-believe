# OpenapiClient::WebhookRegistrationRequest

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **description** | **String** |  | [optional] |
| **event_types** | **Array&lt;String&gt;** |  | [optional] |
| **url** | **String** | The URL to send webhook events to |  |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::WebhookRegistrationRequest.new(
  description: null,
  event_types: null,
  url: null
)
```

