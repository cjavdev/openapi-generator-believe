# OpenapiClient::PepTalkChunk

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **chunk_id** | **Integer** | Chunk sequence number |  |
| **emotional_beat** | **String** | The emotional purpose of this chunk (e.g., greeting, acknowledgment, wisdom, affirmation, encouragement) | [optional] |
| **is_final** | **Boolean** | Is this the final chunk | [default to false] |
| **text** | **String** | The text of this chunk |  |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::PepTalkChunk.new(
  chunk_id: null,
  emotional_beat: null,
  is_final: null,
  text: null
)
```

