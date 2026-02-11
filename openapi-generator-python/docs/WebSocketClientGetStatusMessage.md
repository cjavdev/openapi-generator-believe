# WebSocketClientGetStatusMessage

Request current match status.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**action** | **str** | Action to perform | 

## Example

```python
from openapi_client.models.web_socket_client_get_status_message import WebSocketClientGetStatusMessage

# TODO update the JSON string below
json = "{}"
# create an instance of WebSocketClientGetStatusMessage from a JSON string
web_socket_client_get_status_message_instance = WebSocketClientGetStatusMessage.from_json(json)
# print the JSON string representation of the object
print(WebSocketClientGetStatusMessage.to_json())

# convert the object into a dict
web_socket_client_get_status_message_dict = web_socket_client_get_status_message_instance.to_dict()
# create an instance of WebSocketClientGetStatusMessage from a dict
web_socket_client_get_status_message_from_dict = WebSocketClientGetStatusMessage.from_dict(web_socket_client_get_status_message_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


