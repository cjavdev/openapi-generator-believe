# OpenapiClient::PressConferenceRequest

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **hostile** | **Boolean** | Is this a hostile question from Trent Crimm? | [optional][default to false] |
| **question** | **String** | The press question to answer |  |
| **topic** | **String** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::PressConferenceRequest.new(
  hostile: null,
  question: Ted, your team just lost 5-0. How do you explain this embarrassing defeat?,
  topic: null
)
```

