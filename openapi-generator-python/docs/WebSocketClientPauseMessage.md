# WebSocketClientPauseMessage

Pause the match simulation.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**action** | **str** | Action to perform | 

## Example

```python
from openapi_client.models.web_socket_client_pause_message import WebSocketClientPauseMessage

# TODO update the JSON string below
json = "{}"
# create an instance of WebSocketClientPauseMessage from a JSON string
web_socket_client_pause_message_instance = WebSocketClientPauseMessage.from_json(json)
# print the JSON string representation of the object
print(WebSocketClientPauseMessage.to_json())

# convert the object into a dict
web_socket_client_pause_message_dict = web_socket_client_pause_message_instance.to_dict()
# create an instance of WebSocketClientPauseMessage from a dict
web_socket_client_pause_message_from_dict = WebSocketClientPauseMessage.from_dict(web_socket_client_pause_message_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


