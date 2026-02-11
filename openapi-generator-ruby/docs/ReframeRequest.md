# OpenapiClient::ReframeRequest

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **negative_thought** | **String** | The negative thought to reframe |  |
| **recurring** | **Boolean** | Is this a recurring thought? | [optional][default to false] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::ReframeRequest.new(
  negative_thought: I&#39;m not good enough for this job.,
  recurring: null
)
```

