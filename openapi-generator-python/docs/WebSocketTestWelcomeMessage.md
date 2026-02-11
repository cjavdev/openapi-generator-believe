# WebSocketTestWelcomeMessage

Welcome message sent when connecting to the test WebSocket.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** | Welcome message | 
**ted_says** | **str** | Ted&#39;s greeting | 
**type** | **str** | Message type | 

## Example

```python
from openapi_client.models.web_socket_test_welcome_message import WebSocketTestWelcomeMessage

# TODO update the JSON string below
json = "{}"
# create an instance of WebSocketTestWelcomeMessage from a JSON string
web_socket_test_welcome_message_instance = WebSocketTestWelcomeMessage.from_json(json)
# print the JSON string representation of the object
print(WebSocketTestWelcomeMessage.to_json())

# convert the object into a dict
web_socket_test_welcome_message_dict = web_socket_test_welcome_message_instance.to_dict()
# create an instance of WebSocketTestWelcomeMessage from a dict
web_socket_test_welcome_message_from_dict = WebSocketTestWelcomeMessage.from_dict(web_socket_test_welcome_message_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


