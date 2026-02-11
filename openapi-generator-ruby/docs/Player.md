# OpenapiClient::Player

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **assists** | **Integer** | Total assists for the team | [optional][default to 0] |
| **character_id** | **String** | ID of the character (references /characters/{id}) |  |
| **goals_scored** | **Integer** | Total goals scored for the team | [optional][default to 0] |
| **id** | **String** | Unique identifier for this team membership |  |
| **is_captain** | **Boolean** | Whether this player is team captain | [optional][default to false] |
| **jersey_number** | **Integer** | Jersey/shirt number |  |
| **member_type** | **String** | Discriminator field indicating this is a player | [optional][default to &#39;player&#39;] |
| **position** | [**Position**](Position.md) | Playing position on the field |  |
| **team_id** | **String** | ID of the team they belong to |  |
| **years_with_team** | **Integer** | Number of years with the current team |  |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::Player.new(
  assists: 23,
  character_id: jamie-tartt,
  goals_scored: 47,
  id: jamie-tartt-richmond,
  is_captain: false,
  jersey_number: 9,
  member_type: null,
  position: null,
  team_id: afc-richmond,
  years_with_team: 3
)
```

