# OpenapiClient::TeamMemberTransferredEvent

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **created_at** | **Time** | When the event was created |  |
| **data** | [**TeamMemberTransferredData**](TeamMemberTransferredData.md) |  |  |
| **event_id** | **String** | Unique identifier for this event |  |
| **event_type** | **String** | The type of webhook event |  |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::TeamMemberTransferredEvent.new(
  created_at: null,
  data: null,
  event_id: null,
  event_type: null
)
```

