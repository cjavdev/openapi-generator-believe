# OpenapiClient::QuoteCreate

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **character_id** | **String** | ID of the character who said it |  |
| **context** | **String** | Context in which the quote was said |  |
| **episode_id** | **String** |  | [optional] |
| **is_funny** | **Boolean** | Whether this quote is humorous | [optional][default to false] |
| **is_inspirational** | **Boolean** | Whether this quote is inspirational | [optional][default to true] |
| **moment_type** | [**QuoteMoment**](QuoteMoment.md) | Type of moment when the quote was said |  |
| **popularity_score** | **Float** |  | [optional] |
| **secondary_themes** | [**Array&lt;QuoteTheme&gt;**](QuoteTheme.md) | Additional themes | [optional] |
| **text** | **String** | The quote text |  |
| **theme** | [**QuoteTheme**](QuoteTheme.md) | Primary theme of the quote |  |
| **times_shared** | **Integer** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::QuoteCreate.new(
  character_id: ted-lasso,
  context: Ted playing darts against Rupert in the pub, explaining his philosophy,
  episode_id: null,
  is_funny: null,
  is_inspirational: null,
  moment_type: null,
  popularity_score: null,
  secondary_themes: [wisdom, kindness],
  text: Be curious, not judgmental.,
  theme: null,
  times_shared: null
)
```

