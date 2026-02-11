# WebSocketMatchEventMessage

Message containing a live match event.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**event** | [**WebSocketLiveMatchEvent**](WebSocketLiveMatchEvent.md) |  | 
**type** | **str** | Message type | 

## Example

```python
from openapi_client.models.web_socket_match_event_message import WebSocketMatchEventMessage

# TODO update the JSON string below
json = "{}"
# create an instance of WebSocketMatchEventMessage from a JSON string
web_socket_match_event_message_instance = WebSocketMatchEventMessage.from_json(json)
# print the JSON string representation of the object
print(WebSocketMatchEventMessage.to_json())

# convert the object into a dict
web_socket_match_event_message_dict = web_socket_match_event_message_instance.to_dict()
# create an instance of WebSocketMatchEventMessage from a dict
web_socket_match_event_message_from_dict = WebSocketMatchEventMessage.from_dict(web_socket_match_event_message_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


