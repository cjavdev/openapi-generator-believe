# OpenapiClient::Updates

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
| **certifications** | **Array&lt;String&gt;** |  | [optional] |
| **specialty** | [**MedicalSpecialty**](MedicalSpecialty.md) |  | [optional] |
| **win_rate** | **Float** |  | [optional] |
| **license_number** | **String** |  | [optional] |
| **qualifications** | **Array&lt;String&gt;** |  | [optional] |
| **is_head_kitman** | **Boolean** |  | [optional] |
| **responsibilities** | **Array&lt;String&gt;** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::Updates.new(
  assists: null,
  goals_scored: null,
  is_captain: null,
  jersey_number: null,
  position: null,
  team_id: null,
  years_with_team: null,
  certifications: null,
  specialty: null,
  win_rate: null,
  license_number: null,
  qualifications: null,
  is_head_kitman: null,
  responsibilities: null
)
```

