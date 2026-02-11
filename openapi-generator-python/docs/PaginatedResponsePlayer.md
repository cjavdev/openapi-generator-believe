# PaginatedResponsePlayer


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[Player]**](Player.md) |  | 
**has_more** | **bool** | Whether there are more items after this page. | [readonly] 
**limit** | **int** |  | 
**page** | **int** | Current page number (1-indexed, for display purposes). | [readonly] 
**pages** | **int** | Total number of pages. | [readonly] 
**skip** | **int** |  | 
**total** | **int** |  | 

## Example

```python
from openapi_client.models.paginated_response_player import PaginatedResponsePlayer

# TODO update the JSON string below
json = "{}"
# create an instance of PaginatedResponsePlayer from a JSON string
paginated_response_player_instance = PaginatedResponsePlayer.from_json(json)
# print the JSON string representation of the object
print(PaginatedResponsePlayer.to_json())

# convert the object into a dict
paginated_response_player_dict = paginated_response_player_instance.to_dict()
# create an instance of PaginatedResponsePlayer from a dict
paginated_response_player_from_dict = PaginatedResponsePlayer.from_dict(paginated_response_player_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


