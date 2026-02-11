# OpenapiClient::WebSocketMatchEndMessage

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **final_score** | [**WebSocketMatchScore**](WebSocketMatchScore.md) |  |  |
| **final_stats** | [**WebSocketMatchStats**](WebSocketMatchStats.md) |  |  |
| **man_of_the_match** | **String** | Man of the match |  |
| **match_id** | **String** | Match identifier |  |
| **ted_post_match** | **String** | Ted&#39;s post-match thoughts |  |
| **type** | **String** | Message type |  |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::WebSocketMatchEndMessage.new(
  final_score: null,
  final_stats: null,
  man_of_the_match: null,
  match_id: null,
  ted_post_match: null,
  type: null
)
```

