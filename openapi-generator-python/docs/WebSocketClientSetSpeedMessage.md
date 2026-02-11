# WebSocketClientSetSpeedMessage

Change the simulation playback speed.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**action** | **str** | Action to perform | 
**speed** | **float** | Simulation speed multiplier (0.1 &#x3D; slow motion, 10.0 &#x3D; 10x faster) | 

## Example

```python
from openapi_client.models.web_socket_client_set_speed_message import WebSocketClientSetSpeedMessage

# TODO update the JSON string below
json = "{}"
# create an instance of WebSocketClientSetSpeedMessage from a JSON string
web_socket_client_set_speed_message_instance = WebSocketClientSetSpeedMessage.from_json(json)
# print the JSON string representation of the object
print(WebSocketClientSetSpeedMessage.to_json())

# convert the object into a dict
web_socket_client_set_speed_message_dict = web_socket_client_set_speed_message_instance.to_dict()
# create an instance of WebSocketClientSetSpeedMessage from a dict
web_socket_client_set_speed_message_from_dict = WebSocketClientSetSpeedMessage.from_dict(web_socket_client_set_speed_message_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


