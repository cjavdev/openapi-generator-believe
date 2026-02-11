# WebSocketMatchStartMessage

Message sent when a match simulation starts.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**away_team** | **str** | Away team name | 
**home_team** | **str** | Home team name | 
**match_id** | **str** | Unique match identifier | 
**message** | **str** | Welcome message | 
**type** | **str** | Message type | 

## Example

```python
from openapi_client.models.web_socket_match_start_message import WebSocketMatchStartMessage

# TODO update the JSON string below
json = "{}"
# create an instance of WebSocketMatchStartMessage from a JSON string
web_socket_match_start_message_instance = WebSocketMatchStartMessage.from_json(json)
# print the JSON string representation of the object
print(WebSocketMatchStartMessage.to_json())

# convert the object into a dict
web_socket_match_start_message_dict = web_socket_match_start_message_instance.to_dict()
# create an instance of WebSocketMatchStartMessage from a dict
web_socket_match_start_message_from_dict = WebSocketMatchStartMessage.from_dict(web_socket_match_start_message_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


