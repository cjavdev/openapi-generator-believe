# OpenapiClient::WebSocketTestServerMessage

## Class instance methods

### `openapi_one_of`

Returns the list of classes defined in oneOf.

#### Example

```ruby
require 'openapi_client'

OpenapiClient::WebSocketTestServerMessage.openapi_one_of
# =>
# [
#   :'WebSocketTestEchoMessage',
#   :'WebSocketTestWelcomeMessage'
# ]
```

### `openapi_discriminator_name`

Returns the discriminator's property name.

#### Example

```ruby
require 'openapi_client'

OpenapiClient::WebSocketTestServerMessage.openapi_discriminator_name
# => :'type'
```
```

### build

Find the appropriate object from the `openapi_one_of` list and casts the data into it.

#### Example

```ruby
require 'openapi_client'

OpenapiClient::WebSocketTestServerMessage.build(data)
# => #<WebSocketTestEchoMessage:0x00007fdd4aab02a0>

OpenapiClient::WebSocketTestServerMessage.build(data_that_doesnt_match)
# => nil
```

#### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| **data** | **Mixed** | data to be matched against the list of oneOf items |

#### Return type

- `WebSocketTestEchoMessage`
- `WebSocketTestWelcomeMessage`
- `nil` (if no type matches)

