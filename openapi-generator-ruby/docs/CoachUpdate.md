# OpenapiClient::CoachUpdate

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **certifications** | **Array&lt;String&gt;** |  | [optional] |
| **specialty** | [**CoachSpecialty**](CoachSpecialty.md) |  | [optional] |
| **team_id** | **String** |  | [optional] |
| **win_rate** | **Float** |  | [optional] |
| **years_with_team** | **Integer** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::CoachUpdate.new(
  certifications: null,
  specialty: null,
  team_id: null,
  win_rate: null,
  years_with_team: null
)
```

