# OpenapiClient::WebSocketClientSetSpeedMessage

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **action** | **String** | Action to perform |  |
| **speed** | **Float** | Simulation speed multiplier (0.1 &#x3D; slow motion, 10.0 &#x3D; 10x faster) |  |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::WebSocketClientSetSpeedMessage.new(
  action: null,
  speed: null
)
```

