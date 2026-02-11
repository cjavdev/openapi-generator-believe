# OpenapiClient::Biscuit

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **String** | Biscuit identifier |  |
| **message** | **String** | Message that comes with the biscuit |  |
| **pairs_well_with** | **String** | What this biscuit pairs well with |  |
| **ted_note** | **String** | A handwritten note from Ted |  |
| **type** | [**BiscuitType**](BiscuitType.md) | Type of biscuit |  |
| **warmth_level** | **Integer** | How warm and fresh (1-10) |  |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::Biscuit.new(
  id: null,
  message: null,
  pairs_well_with: null,
  ted_note: null,
  type: null,
  warmth_level: null
)
```

