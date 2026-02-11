# WebSocketMatchStats

Current match statistics.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**corners_away** | **int** | Away team corners | 
**corners_home** | **int** | Home team corners | 
**fouls_away** | **int** | Away team fouls | 
**fouls_home** | **int** | Home team fouls | 
**possession_away** | **float** | Away team possession % | 
**possession_home** | **float** | Home team possession % | 
**red_cards_away** | **int** | Away team red cards | 
**red_cards_home** | **int** | Home team red cards | 
**shots_away** | **int** | Away team total shots | 
**shots_home** | **int** | Home team total shots | 
**shots_on_target_away** | **int** | Away team shots on target | 
**shots_on_target_home** | **int** | Home team shots on target | 
**yellow_cards_away** | **int** | Away team yellow cards | 
**yellow_cards_home** | **int** | Home team yellow cards | 

## Example

```python
from openapi_client.models.web_socket_match_stats import WebSocketMatchStats

# TODO update the JSON string below
json = "{}"
# create an instance of WebSocketMatchStats from a JSON string
web_socket_match_stats_instance = WebSocketMatchStats.from_json(json)
# print the JSON string representation of the object
print(WebSocketMatchStats.to_json())

# convert the object into a dict
web_socket_match_stats_dict = web_socket_match_stats_instance.to_dict()
# create an instance of WebSocketMatchStats from a dict
web_socket_match_stats_from_dict = WebSocketMatchStats.from_dict(web_socket_match_stats_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


