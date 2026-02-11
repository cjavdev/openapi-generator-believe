# WebSocketClientMessage

Messages sent by the client to control the match simulation.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**action** | **str** | Action to perform | 
**speed** | **float** | Simulation speed multiplier (0.1 &#x3D; slow motion, 10.0 &#x3D; 10x faster) | 

## Example

```python
from openapi_client.models.web_socket_client_message import WebSocketClientMessage

# TODO update the JSON string below
json = "{}"
# create an instance of WebSocketClientMessage from a JSON string
web_socket_client_message_instance = WebSocketClientMessage.from_json(json)
# print the JSON string representation of the object
print(WebSocketClientMessage.to_json())

# convert the object into a dict
web_socket_client_message_dict = web_socket_client_message_instance.to_dict()
# create an instance of WebSocketClientMessage from a dict
web_socket_client_message_from_dict = WebSocketClientMessage.from_dict(web_socket_client_message_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


