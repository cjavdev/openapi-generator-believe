# OpenapiClient::WebhookRegistrationResponse

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **message** | **String** | Status message | [optional][default to &#39;Webhook registered successfully&#39;] |
| **ted_says** | **String** | Ted&#39;s reaction | [optional][default to &#39;You know what? Staying connected is what it&#39;s all about. Welcome to the team!&#39;] |
| **webhook** | [**RegisteredWebhook**](RegisteredWebhook.md) | The registered webhook details |  |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::WebhookRegistrationResponse.new(
  message: null,
  ted_says: null,
  webhook: null
)
```

