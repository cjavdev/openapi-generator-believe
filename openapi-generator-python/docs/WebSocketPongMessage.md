# WebSocketPongMessage

Pong response to client ping.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** | Message type | 

## Example

```python
from openapi_client.models.web_socket_pong_message import WebSocketPongMessage

# TODO update the JSON string below
json = "{}"
# create an instance of WebSocketPongMessage from a JSON string
web_socket_pong_message_instance = WebSocketPongMessage.from_json(json)
# print the JSON string representation of the object
print(WebSocketPongMessage.to_json())

# convert the object into a dict
web_socket_pong_message_dict = web_socket_pong_message_instance.to_dict()
# create an instance of WebSocketPongMessage from a dict
web_socket_pong_message_from_dict = WebSocketPongMessage.from_dict(web_socket_pong_message_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


