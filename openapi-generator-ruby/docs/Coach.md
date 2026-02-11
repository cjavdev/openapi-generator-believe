# OpenapiClient::Coach

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **certifications** | **Array&lt;String&gt;** | Coaching certifications and licenses | [optional] |
| **character_id** | **String** | ID of the character (references /characters/{id}) |  |
| **id** | **String** | Unique identifier for this team membership |  |
| **member_type** | **String** | Discriminator field indicating this is a coach | [optional][default to &#39;coach&#39;] |
| **specialty** | [**CoachSpecialty**](CoachSpecialty.md) | Coaching specialty/role |  |
| **team_id** | **String** | ID of the team they belong to |  |
| **win_rate** | **Float** |  | [optional] |
| **years_with_team** | **Integer** | Number of years with the current team |  |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::Coach.new(
  certifications: [UEFA Pro License, FA Level 4],
  character_id: jamie-tartt,
  id: ted-lasso-richmond,
  member_type: null,
  specialty: null,
  team_id: afc-richmond,
  win_rate: null,
  years_with_team: 3
)
```

