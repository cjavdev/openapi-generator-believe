# OpenapiClient::WebSocketMatchStartMessage

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **away_team** | **String** | Away team name |  |
| **home_team** | **String** | Home team name |  |
| **match_id** | **String** | Unique match identifier |  |
| **message** | **String** | Welcome message |  |
| **type** | **String** | Message type |  |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::WebSocketMatchStartMessage.new(
  away_team: null,
  home_team: null,
  match_id: null,
  message: null,
  type: null
)
```

