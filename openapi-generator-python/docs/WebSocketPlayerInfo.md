# WebSocketPlayerInfo

Information about a player involved in an event.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** | Player name | 
**number** | **int** | Jersey number | 
**position** | **str** | Player position | 

## Example

```python
from openapi_client.models.web_socket_player_info import WebSocketPlayerInfo

# TODO update the JSON string below
json = "{}"
# create an instance of WebSocketPlayerInfo from a JSON string
web_socket_player_info_instance = WebSocketPlayerInfo.from_json(json)
# print the JSON string representation of the object
print(WebSocketPlayerInfo.to_json())

# convert the object into a dict
web_socket_player_info_dict = web_socket_player_info_instance.to_dict()
# create an instance of WebSocketPlayerInfo from a dict
web_socket_player_info_from_dict = WebSocketPlayerInfo.from_dict(web_socket_player_info_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


