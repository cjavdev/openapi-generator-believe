# WebSocketMatchEndMessage

Message sent when a match simulation ends.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**final_score** | [**WebSocketMatchScore**](WebSocketMatchScore.md) |  | 
**final_stats** | [**WebSocketMatchStats**](WebSocketMatchStats.md) |  | 
**man_of_the_match** | **str** | Man of the match | 
**match_id** | **str** | Match identifier | 
**ted_post_match** | **str** | Ted&#39;s post-match thoughts | 
**type** | **str** | Message type | 

## Example

```python
from openapi_client.models.web_socket_match_end_message import WebSocketMatchEndMessage

# TODO update the JSON string below
json = "{}"
# create an instance of WebSocketMatchEndMessage from a JSON string
web_socket_match_end_message_instance = WebSocketMatchEndMessage.from_json(json)
# print the JSON string representation of the object
print(WebSocketMatchEndMessage.to_json())

# convert the object into a dict
web_socket_match_end_message_dict = web_socket_match_end_message_instance.to_dict()
# create an instance of WebSocketMatchEndMessage from a dict
web_socket_match_end_message_from_dict = WebSocketMatchEndMessage.from_dict(web_socket_match_end_message_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


