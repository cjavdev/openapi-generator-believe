# OpenapiClient::MedicalStaffUpdate

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **license_number** | **String** |  | [optional] |
| **qualifications** | **Array&lt;String&gt;** |  | [optional] |
| **specialty** | [**MedicalSpecialty**](MedicalSpecialty.md) |  | [optional] |
| **team_id** | **String** |  | [optional] |
| **years_with_team** | **Integer** |  | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::MedicalStaffUpdate.new(
  license_number: null,
  qualifications: null,
  specialty: null,
  team_id: null,
  years_with_team: null
)
```

