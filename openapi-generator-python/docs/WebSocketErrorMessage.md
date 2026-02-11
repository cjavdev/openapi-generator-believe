# WebSocketErrorMessage

Error message for WebSocket communication.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **str** | Error code | 
**message** | **str** | Error description | 
**type** | **str** | Message type | 

## Example

```python
from openapi_client.models.web_socket_error_message import WebSocketErrorMessage

# TODO update the JSON string below
json = "{}"
# create an instance of WebSocketErrorMessage from a JSON string
web_socket_error_message_instance = WebSocketErrorMessage.from_json(json)
# print the JSON string representation of the object
print(WebSocketErrorMessage.to_json())

# convert the object into a dict
web_socket_error_message_dict = web_socket_error_message_instance.to_dict()
# create an instance of WebSocketErrorMessage from a dict
web_socket_error_message_from_dict = WebSocketErrorMessage.from_dict(web_socket_error_message_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


