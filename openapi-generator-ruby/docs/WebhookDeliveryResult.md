# OpenapiClient::WebhookDeliveryResult

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **error** | **String** |  | [optional] |
| **status_code** | **Integer** |  | [optional] |
| **success** | **Boolean** | Whether delivery was successful |  |
| **url** | **String** | URL the webhook was sent to |  |
| **webhook_id** | **String** | ID of the webhook |  |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::WebhookDeliveryResult.new(
  error: null,
  status_code: null,
  success: null,
  url: null,
  webhook_id: null
)
```

