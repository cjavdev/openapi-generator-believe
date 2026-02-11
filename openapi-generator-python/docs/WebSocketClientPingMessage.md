# WebSocketClientPingMessage

Ping message for keep-alive.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**action** | **str** | Action to perform | 

## Example

```python
from openapi_client.models.web_socket_client_ping_message import WebSocketClientPingMessage

# TODO update the JSON string below
json = "{}"
# create an instance of WebSocketClientPingMessage from a JSON string
web_socket_client_ping_message_instance = WebSocketClientPingMessage.from_json(json)
# print the JSON string representation of the object
print(WebSocketClientPingMessage.to_json())

# convert the object into a dict
web_socket_client_ping_message_dict = web_socket_client_ping_message_instance.to_dict()
# create an instance of WebSocketClientPingMessage from a dict
web_socket_client_ping_message_from_dict = WebSocketClientPingMessage.from_dict(web_socket_client_ping_message_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


