# WebSocketLiveMatchEvent

A live match event with full details.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**added_time** | **int** | Added/injury time minutes | [optional] 
**commentary** | **str** | Match commentary for this event | 
**crowd_reaction** | **str** | Crowd reaction to the event | [optional] 
**description** | **str** | Human-readable event description | 
**event_id** | **int** | Unique event sequence number | 
**event_type** | **str** | Type of match event | 
**minute** | **int** | Match minute | 
**player** | [**WebSocketPlayerInfo**](WebSocketPlayerInfo.md) |  | [optional] 
**score** | [**WebSocketMatchScore**](WebSocketMatchScore.md) |  | 
**secondary_player** | [**WebSocketPlayerInfo**](WebSocketPlayerInfo.md) | Second player involved (e.g., assist, replaced player) | [optional] 
**stats** | [**WebSocketMatchStats**](WebSocketMatchStats.md) |  | 
**team** | **str** | Which team the event relates to | [optional] 
**ted_reaction** | **str** | Ted Lasso&#39;s sideline reaction | [optional] 

## Example

```python
from openapi_client.models.web_socket_live_match_event import WebSocketLiveMatchEvent

# TODO update the JSON string below
json = "{}"
# create an instance of WebSocketLiveMatchEvent from a JSON string
web_socket_live_match_event_instance = WebSocketLiveMatchEvent.from_json(json)
# print the JSON string representation of the object
print(WebSocketLiveMatchEvent.to_json())

# convert the object into a dict
web_socket_live_match_event_dict = web_socket_live_match_event_instance.to_dict()
# create an instance of WebSocketLiveMatchEvent from a dict
web_socket_live_match_event_from_dict = WebSocketLiveMatchEvent.from_dict(web_socket_live_match_event_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


