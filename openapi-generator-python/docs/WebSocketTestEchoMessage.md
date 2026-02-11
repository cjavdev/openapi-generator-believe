# WebSocketTestEchoMessage

Echo response from the test WebSocket.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** | The echoed message | 
**ted_says** | **str** | Ted&#39;s response | 
**type** | **str** | Message type | 

## Example

```python
from openapi_client.models.web_socket_test_echo_message import WebSocketTestEchoMessage

# TODO update the JSON string below
json = "{}"
# create an instance of WebSocketTestEchoMessage from a JSON string
web_socket_test_echo_message_instance = WebSocketTestEchoMessage.from_json(json)
# print the JSON string representation of the object
print(WebSocketTestEchoMessage.to_json())

# convert the object into a dict
web_socket_test_echo_message_dict = web_socket_test_echo_message_instance.to_dict()
# create an instance of WebSocketTestEchoMessage from a dict
web_socket_test_echo_message_from_dict = WebSocketTestEchoMessage.from_dict(web_socket_test_echo_message_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


