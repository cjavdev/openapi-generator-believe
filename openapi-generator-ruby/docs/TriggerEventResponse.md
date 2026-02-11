# OpenapiClient::TriggerEventResponse

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **deliveries** | [**Array&lt;WebhookDeliveryResult&gt;**](WebhookDeliveryResult.md) | Results of webhook deliveries |  |
| **event_id** | **String** | Unique event identifier |  |
| **event_type** | **String** | The type of event triggered |  |
| **successful_deliveries** | **Integer** | Number of successful deliveries |  |
| **ted_says** | **String** | Ted&#39;s reaction |  |
| **total_webhooks** | **Integer** | Total number of webhooks that received this event |  |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::TriggerEventResponse.new(
  deliveries: null,
  event_id: null,
  event_type: null,
  successful_deliveries: null,
  ted_says: null,
  total_webhooks: null
)
```

