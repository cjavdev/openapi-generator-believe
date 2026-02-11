# OpenapiClient::WebSocketLiveMatchEvent

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **added_time** | **Integer** | Added/injury time minutes | [optional] |
| **commentary** | **String** | Match commentary for this event |  |
| **crowd_reaction** | **String** | Crowd reaction to the event | [optional] |
| **description** | **String** | Human-readable event description |  |
| **event_id** | **Integer** | Unique event sequence number |  |
| **event_type** | **String** | Type of match event |  |
| **minute** | **Integer** | Match minute |  |
| **player** | [**WebSocketPlayerInfo**](WebSocketPlayerInfo.md) |  | [optional] |
| **score** | [**WebSocketMatchScore**](WebSocketMatchScore.md) |  |  |
| **secondary_player** | [**WebSocketPlayerInfo**](WebSocketPlayerInfo.md) | Second player involved (e.g., assist, replaced player) | [optional] |
| **stats** | [**WebSocketMatchStats**](WebSocketMatchStats.md) |  |  |
| **team** | **String** | Which team the event relates to | [optional] |
| **ted_reaction** | **String** | Ted Lasso&#39;s sideline reaction | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::WebSocketLiveMatchEvent.new(
  added_time: null,
  commentary: null,
  crowd_reaction: null,
  description: null,
  event_id: null,
  event_type: null,
  minute: null,
  player: null,
  score: null,
  secondary_player: null,
  stats: null,
  team: null,
  ted_reaction: null
)
```

