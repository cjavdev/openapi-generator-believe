# OpenapiClient::EquipmentManager

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **character_id** | **String** | ID of the character (references /characters/{id}) |  |
| **id** | **String** | Unique identifier for this team membership |  |
| **is_head_kitman** | **Boolean** | Whether this is the head equipment manager | [optional][default to false] |
| **member_type** | **String** | Discriminator field indicating this is an equipment manager | [optional][default to &#39;equipment_manager&#39;] |
| **responsibilities** | **Array&lt;String&gt;** | List of responsibilities | [optional] |
| **team_id** | **String** | ID of the team they belong to |  |
| **years_with_team** | **Integer** | Number of years with the current team |  |

## Example

```ruby
require 'openapi_client'

instance = OpenapiClient::EquipmentManager.new(
  character_id: jamie-tartt,
  id: nate-kitman-richmond,
  is_head_kitman: true,
  member_type: null,
  responsibilities: [Kit preparation, Equipment maintenance],
  team_id: afc-richmond,
  years_with_team: 3
)
```

