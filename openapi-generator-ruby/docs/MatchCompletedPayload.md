# OpenapiClient::MatchCompletedPayload

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **data** | [**MatchCompletedData**](MatchCompletedData.md) | Event data |  |
| **event_type** | **String** | The type of webhook event | [optional][default to &#39;match.completed&#39;] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::MatchCompletedPayload.new(
  data: null,
  event_type: null
)
```

