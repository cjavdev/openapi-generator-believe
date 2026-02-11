# OpenapiClient::MedicalStaff

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **character_id** | **String** | ID of the character (references /characters/{id}) |  |
| **id** | **String** | Unique identifier for this team membership |  |
| **license_number** | **String** |  | [optional] |
| **member_type** | **String** | Discriminator field indicating this is medical staff | [optional][default to &#39;medical_staff&#39;] |
| **qualifications** | **Array&lt;String&gt;** | Medical qualifications and degrees | [optional] |
| **specialty** | [**MedicalSpecialty**](MedicalSpecialty.md) | Medical specialty |  |
| **team_id** | **String** | ID of the team they belong to |  |
| **years_with_team** | **Integer** | Number of years with the current team |  |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::MedicalStaff.new(
  character_id: jamie-tartt,
  id: sharon-fieldstone-richmond,
  license_number: null,
  member_type: null,
  qualifications: [PhD Clinical Psychology, Sports Psychology Certification],
  specialty: null,
  team_id: afc-richmond,
  years_with_team: 3
)
```

