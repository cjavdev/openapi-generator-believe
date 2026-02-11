# OpenapiClient::MatchCompletedEvent

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **created_at** | **Time** | When the event was created |  |
| **data** | [**MatchCompletedData**](MatchCompletedData.md) |  |  |
| **event_id** | **String** | Unique identifier for this event |  |
| **event_type** | **String** | The type of webhook event |  |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::MatchCompletedEvent.new(
  created_at: null,
  data: null,
  event_id: null,
  event_type: null
)
```

