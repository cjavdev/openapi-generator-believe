# OpenapiClient::TurningPoint

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **character_involved** | **String** |  | [optional] |
| **description** | **String** | What happened |  |
| **emotional_impact** | **String** | How this affected the team emotionally |  |
| **minute** | **Integer** | Minute of the match |  |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::TurningPoint.new(
  character_involved: null,
  description: null,
  emotional_impact: Galvanized the team&#39;s fighting spirit,
  minute: null
)
```

