# OpenapiClient::TriggerEventRequest

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **event_type** | **String** | The type of event to trigger |  |
| **payload** | [**TriggerEventRequestPayload**](TriggerEventRequestPayload.md) |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::TriggerEventRequest.new(
  event_type: null,
  payload: null
)
```

