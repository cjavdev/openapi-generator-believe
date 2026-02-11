# OpenapiClient::DataInner1

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **character_id** | **String** | ID of the character (references /characters/{id}) |  |
| **id** | **String** | Unique identifier for this team membership |  |
| **license_number** | **String** |  | [optional] |
| **member_type** | **String** | Discriminator field indicating this is an equipment manager | [optional][default to &#39;equipment_manager&#39;] |
| **qualifications** | **Array&lt;String&gt;** | Medical qualifications and degrees | [optional] |
| **specialty** | [**MedicalSpecialty**](MedicalSpecialty.md) | Medical specialty |  |
| **team_id** | **String** | ID of the team they belong to |  |
| **years_with_team** | **Integer** | Number of years with the current team |  |
| **is_head_kitman** | **Boolean** | Whether this is the head equipment manager | [optional][default to false] |
| **responsibilities** | **Array&lt;String&gt;** | List of responsibilities | [optional] |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::DataInner1.new(
  character_id: jamie-tartt,
  id: nate-kitman-richmond,
  license_number: null,
  member_type: null,
  qualifications: [PhD Clinical Psychology, Sports Psychology Certification],
  specialty: null,
  team_id: afc-richmond,
  years_with_team: 3,
  is_head_kitman: true,
  responsibilities: [Kit preparation, Equipment maintenance]
)
```

