# OpenapiClient::WebSocketClientMessage

## Class instance methods

### `openapi_one_of`

Returns the list of classes defined in oneOf.

#### Example

```ruby
require 'openapi_client'

OpenapiClient::WebSocketClientMessage.openapi_one_of
# =>
# [
#   :'WebSocketClientGetStatusMessage',
#   :'WebSocketClientPauseMessage',
#   :'WebSocketClientPingMessage',
#   :'WebSocketClientResumeMessage',
#   :'WebSocketClientSetSpeedMessage'
# ]
```

### `openapi_discriminator_name`

Returns the discriminator's property name.

#### Example

```ruby
require 'openapi_client'

OpenapiClient::WebSocketClientMessage.openapi_discriminator_name
# => :'action'
```

### `openapi_discriminator_name`

Returns the discriminator's mapping.

#### Example

```ruby
require 'openapi_client'

OpenapiClient::WebSocketClientMessage.openapi_discriminator_mapping
# =>
# {
#   :'get_status' => :'WebSocketClientGetStatusMessage',
#   :'pause' => :'WebSocketClientPauseMessage',
#   :'ping' => :'WebSocketClientPingMessage',
#   :'resume' => :'WebSocketClientResumeMessage',
#   :'set_speed' => :'WebSocketClientSetSpeedMessage'
# }
```

### build

Find the appropriate object from the `openapi_one_of` list and casts the data into it.

#### Example

```ruby
require 'openapi_client'

OpenapiClient::WebSocketClientMessage.build(data)
# => #<WebSocketClientGetStatusMessage:0x00007fdd4aab02a0>

OpenapiClient::WebSocketClientMessage.build(data_that_doesnt_match)
# => nil
```

#### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| **data** | **Mixed** | data to be matched against the list of oneOf items |

#### Return type

- `WebSocketClientGetStatusMessage`
- `WebSocketClientPauseMessage`
- `WebSocketClientPingMessage`
- `WebSocketClientResumeMessage`
- `WebSocketClientSetSpeedMessage`
- `nil` (if no type matches)

