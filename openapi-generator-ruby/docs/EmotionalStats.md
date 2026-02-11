# OpenapiClient::EmotionalStats

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **curiosity** | **Integer** | Level of curiosity over judgment (0-100) |  |
| **empathy** | **Integer** | Capacity for empathy (0-100) |  |
| **optimism** | **Integer** | Level of optimism (0-100) |  |
| **resilience** | **Integer** | Bounce-back ability (0-100) |  |
| **vulnerability** | **Integer** | Willingness to be vulnerable (0-100) |  |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::EmotionalStats.new(
  curiosity: 99,
  empathy: 100,
  optimism: 95,
  resilience: 90,
  vulnerability: 80
)
```

