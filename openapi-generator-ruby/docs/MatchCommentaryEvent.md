# OpenapiClient::MatchCommentaryEvent

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **commentary** | **String** | Commentator&#39;s call |  |
| **crowd_reaction** | **String** | How the crowd reacted | [optional] |
| **description** | **String** | What happened |  |
| **event_id** | **Integer** | Event sequence number |  |
| **event_type** | **String** | Type of event |  |
| **is_final** | **Boolean** | Is this the final event | [default to false] |
| **minute** | **Integer** | Match minute |  |
| **ted_sideline_reaction** | **String** | Ted&#39;s reaction on the sideline | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::MatchCommentaryEvent.new(
  commentary: null,
  crowd_reaction: null,
  description: null,
  event_id: null,
  event_type: null,
  is_final: null,
  minute: null,
  ted_sideline_reaction: null
)
```

