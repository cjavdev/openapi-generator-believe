# WebSocketMatchScore

Current match score.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**away** | **int** | Away team score | 
**home** | **int** | Home team score | 

## Example

```python
from openapi_client.models.web_socket_match_score import WebSocketMatchScore

# TODO update the JSON string below
json = "{}"
# create an instance of WebSocketMatchScore from a JSON string
web_socket_match_score_instance = WebSocketMatchScore.from_json(json)
# print the JSON string representation of the object
print(WebSocketMatchScore.to_json())

# convert the object into a dict
web_socket_match_score_dict = web_socket_match_score_instance.to_dict()
# create an instance of WebSocketMatchScore from a dict
web_socket_match_score_from_dict = WebSocketMatchScore.from_dict(web_socket_match_score_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


