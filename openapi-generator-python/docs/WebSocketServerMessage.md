# WebSocketServerMessage

Messages sent by the server during live match simulation.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**away_team** | **str** | Away team name | 
**home_team** | **str** | Home team name | 
**match_id** | **str** | Match identifier | 
**message** | **str** | Error description | 
**type** | **str** | Message type | 
**event** | [**WebSocketLiveMatchEvent**](WebSocketLiveMatchEvent.md) |  | 
**final_score** | [**WebSocketMatchScore**](WebSocketMatchScore.md) |  | 
**final_stats** | [**WebSocketMatchStats**](WebSocketMatchStats.md) |  | 
**man_of_the_match** | **str** | Man of the match | 
**ted_post_match** | **str** | Ted&#39;s post-match thoughts | 
**code** | **str** | Error code | 

## Example

```python
from openapi_client.models.web_socket_server_message import WebSocketServerMessage

# TODO update the JSON string below
json = "{}"
# create an instance of WebSocketServerMessage from a JSON string
web_socket_server_message_instance = WebSocketServerMessage.from_json(json)
# print the JSON string representation of the object
print(WebSocketServerMessage.to_json())

# convert the object into a dict
web_socket_server_message_dict = web_socket_server_message_instance.to_dict()
# create an instance of WebSocketServerMessage from a dict
web_socket_server_message_from_dict = WebSocketServerMessage.from_dict(web_socket_server_message_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


