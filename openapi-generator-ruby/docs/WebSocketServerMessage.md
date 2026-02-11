# OpenapiClient::WebSocketServerMessage

## Class instance methods

### `openapi_one_of`

Returns the list of classes defined in oneOf.

#### Example

```ruby
require 'openapi_client'

OpenapiClient::WebSocketServerMessage.openapi_one_of
# =>
# [
#   :'WebSocketErrorMessage',
#   :'WebSocketMatchEndMessage',
#   :'WebSocketMatchEventMessage',
#   :'WebSocketMatchStartMessage',
#   :'WebSocketPongMessage'
# ]
```

### `openapi_discriminator_name`

Returns the discriminator's property name.

#### Example

```ruby
require 'openapi_client'

OpenapiClient::WebSocketServerMessage.openapi_discriminator_name
# => :'type'
```
```

### build

Find the appropriate object from the `openapi_one_of` list and casts the data into it.

#### Example

```ruby
require 'openapi_client'

OpenapiClient::WebSocketServerMessage.build(data)
# => #<WebSocketErrorMessage:0x00007fdd4aab02a0>

OpenapiClient::WebSocketServerMessage.build(data_that_doesnt_match)
# => nil
```

#### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| **data** | **Mixed** | data to be matched against the list of oneOf items |

#### Return type

- `WebSocketErrorMessage`
- `WebSocketMatchEndMessage`
- `WebSocketMatchEventMessage`
- `WebSocketMatchStartMessage`
- `WebSocketPongMessage`
- `nil` (if no type matches)

