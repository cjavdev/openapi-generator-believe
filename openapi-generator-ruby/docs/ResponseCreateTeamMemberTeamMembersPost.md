# OpenapiClient::ResponseCreateTeamMemberTeamMembersPost

## Class instance methods

### `openapi_one_of`

Returns the list of classes defined in oneOf.

#### Example

```ruby
require 'openapi_client'

OpenapiClient::ResponseCreateTeamMemberTeamMembersPost.openapi_one_of
# =>
# [
#   :'Coach',
#   :'EquipmentManager',
#   :'MedicalStaff',
#   :'Player'
# ]
```

### `openapi_discriminator_name`

Returns the discriminator's property name.

#### Example

```ruby
require 'openapi_client'

OpenapiClient::ResponseCreateTeamMemberTeamMembersPost.openapi_discriminator_name
# => :'member_type'
```

### `openapi_discriminator_name`

Returns the discriminator's mapping.

#### Example

```ruby
require 'openapi_client'

OpenapiClient::ResponseCreateTeamMemberTeamMembersPost.openapi_discriminator_mapping
# =>
# {
#   :'coach' => :'Coach',
#   :'equipment_manager' => :'EquipmentManager',
#   :'medical_staff' => :'MedicalStaff',
#   :'player' => :'Player'
# }
```

### build

Find the appropriate object from the `openapi_one_of` list and casts the data into it.

#### Example

```ruby
require 'openapi_client'

OpenapiClient::ResponseCreateTeamMemberTeamMembersPost.build(data)
# => #<Coach:0x00007fdd4aab02a0>

OpenapiClient::ResponseCreateTeamMemberTeamMembersPost.build(data_that_doesnt_match)
# => nil
```

#### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| **data** | **Mixed** | data to be matched against the list of oneOf items |

#### Return type

- `Coach`
- `EquipmentManager`
- `MedicalStaff`
- `Player`
- `nil` (if no type matches)

