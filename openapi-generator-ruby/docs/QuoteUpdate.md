# OpenapiClient::QuoteUpdate

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **character_id** | **String** |  | [optional] |
| **context** | **String** |  | [optional] |
| **episode_id** | **String** |  | [optional] |
| **is_funny** | **Boolean** |  | [optional] |
| **is_inspirational** | **Boolean** |  | [optional] |
| **moment_type** | [**QuoteMoment**](QuoteMoment.md) |  | [optional] |
| **popularity_score** | **Float** |  | [optional] |
| **secondary_themes** | [**Array&lt;QuoteTheme&gt;**](QuoteTheme.md) |  | [optional] |
| **text** | **String** |  | [optional] |
| **theme** | [**QuoteTheme**](QuoteTheme.md) |  | [optional] |
| **times_shared** | **Integer** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::QuoteUpdate.new(
  character_id: null,
  context: null,
  episode_id: null,
  is_funny: null,
  is_inspirational: null,
  moment_type: null,
  popularity_score: null,
  secondary_themes: null,
  text: null,
  theme: null,
  times_shared: null
)
```

