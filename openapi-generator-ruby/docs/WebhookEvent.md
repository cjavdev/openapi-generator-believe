# OpenapiClient::WebhookEvent

## Class instance methods

### `openapi_one_of`

Returns the list of classes defined in oneOf.

#### Example

```ruby
require 'openapi_client'

OpenapiClient::WebhookEvent.openapi_one_of
# =>
# [
#   :'MatchCompletedEvent',
#   :'TeamMemberTransferredEvent'
# ]
```

### `openapi_discriminator_name`

Returns the discriminator's property name.

#### Example

```ruby
require 'openapi_client'

OpenapiClient::WebhookEvent.openapi_discriminator_name
# => :'event_type'
```

### `openapi_discriminator_name`

Returns the discriminator's mapping.

#### Example

```ruby
require 'openapi_client'

OpenapiClient::WebhookEvent.openapi_discriminator_mapping
# =>
# {
#   :'match.completed' => :'MatchCompletedEvent',
#   :'team_member.transferred' => :'TeamMemberTransferredEvent'
# }
```

### build

Find the appropriate object from the `openapi_one_of` list and casts the data into it.

#### Example

```ruby
require 'openapi_client'

OpenapiClient::WebhookEvent.build(data)
# => #<MatchCompletedEvent:0x00007fdd4aab02a0>

OpenapiClient::WebhookEvent.build(data_that_doesnt_match)
# => nil
```

#### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| **data** | **Mixed** | data to be matched against the list of oneOf items |

#### Return type

- `MatchCompletedEvent`
- `TeamMemberTransferredEvent`
- `nil` (if no type matches)

