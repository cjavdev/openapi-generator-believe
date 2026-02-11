# OpenapiClient::TriggerEventRequestPayload

## Class instance methods

### `openapi_one_of`

Returns the list of classes defined in oneOf.

#### Example

```ruby
require 'openapi_client'

OpenapiClient::TriggerEventRequestPayload.openapi_one_of
# =>
# [
#   :'MatchCompletedPayload',
#   :'TeamMemberTransferredPayload'
# ]
```

### `openapi_discriminator_name`

Returns the discriminator's property name.

#### Example

```ruby
require 'openapi_client'

OpenapiClient::TriggerEventRequestPayload.openapi_discriminator_name
# => :'event_type'
```

### `openapi_discriminator_name`

Returns the discriminator's mapping.

#### Example

```ruby
require 'openapi_client'

OpenapiClient::TriggerEventRequestPayload.openapi_discriminator_mapping
# =>
# {
#   :'match.completed' => :'MatchCompletedPayload',
#   :'team_member.transferred' => :'TeamMemberTransferredPayload'
# }
```

### build

Find the appropriate object from the `openapi_one_of` list and casts the data into it.

#### Example

```ruby
require 'openapi_client'

OpenapiClient::TriggerEventRequestPayload.build(data)
# => #<MatchCompletedPayload:0x00007fdd4aab02a0>

OpenapiClient::TriggerEventRequestPayload.build(data_that_doesnt_match)
# => nil
```

#### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| **data** | **Mixed** | data to be matched against the list of oneOf items |

#### Return type

- `MatchCompletedPayload`
- `TeamMemberTransferredPayload`
- `nil` (if no type matches)

