# WebSocketTestServerMessage

Messages sent by the test WebSocket endpoint.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** | The echoed message | 
**ted_says** | **str** | Ted&#39;s response | 
**type** | **str** | Message type | 

## Example

```python
from openapi_client.models.web_socket_test_server_message import WebSocketTestServerMessage

# TODO update the JSON string below
json = "{}"
# create an instance of WebSocketTestServerMessage from a JSON string
web_socket_test_server_message_instance = WebSocketTestServerMessage.from_json(json)
# print the JSON string representation of the object
print(WebSocketTestServerMessage.to_json())

# convert the object into a dict
web_socket_test_server_message_dict = web_socket_test_server_message_instance.to_dict()
# create an instance of WebSocketTestServerMessage from a dict
web_socket_test_server_message_from_dict = WebSocketTestServerMessage.from_dict(web_socket_test_server_message_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


