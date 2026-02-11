# OpenapiClient::Member

## Class instance methods

### `openapi_one_of`

Returns the list of classes defined in oneOf.

#### Example

```ruby
require 'openapi_client'

OpenapiClient::Member.openapi_one_of
# =>
# [
#   :'CoachBase',
#   :'EquipmentManagerBase',
#   :'MedicalStaffBase',
#   :'PlayerBase'
# ]
```

### `openapi_discriminator_name`

Returns the discriminator's property name.

#### Example

```ruby
require 'openapi_client'

OpenapiClient::Member.openapi_discriminator_name
# => :'member_type'
```

### `openapi_discriminator_name`

Returns the discriminator's mapping.

#### Example

```ruby
require 'openapi_client'

OpenapiClient::Member.openapi_discriminator_mapping
# =>
# {
#   :'coach' => :'CoachBase',
#   :'equipment_manager' => :'EquipmentManagerBase',
#   :'medical_staff' => :'MedicalStaffBase',
#   :'player' => :'PlayerBase'
# }
```

### build

Find the appropriate object from the `openapi_one_of` list and casts the data into it.

#### Example

```ruby
require 'openapi_client'

OpenapiClient::Member.build(data)
# => #<CoachBase:0x00007fdd4aab02a0>

OpenapiClient::Member.build(data_that_doesnt_match)
# => nil
```

#### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| **data** | **Mixed** | data to be matched against the list of oneOf items |

#### Return type

- `CoachBase`
- `EquipmentManagerBase`
- `MedicalStaffBase`
- `PlayerBase`
- `nil` (if no type matches)

