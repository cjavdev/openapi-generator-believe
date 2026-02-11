# OpenapiClient::PlayerUpdate

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **assists** | **Integer** |  | [optional] |
| **goals_scored** | **Integer** |  | [optional] |
| **is_captain** | **Boolean** |  | [optional] |
| **jersey_number** | **Integer** |  | [optional] |
| **position** | [**Position**](Position.md) |  | [optional] |
| **team_id** | **String** |  | [optional] |
| **years_with_team** | **Integer** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::PlayerUpdate.new(
  assists: null,
  goals_scored: null,
  is_captain: null,
  jersey_number: null,
  position: null,
  team_id: null,
  years_with_team: null
)
```

