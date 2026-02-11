# PaginatedResponseEpisode


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[Episode]**](Episode.md) |  | 
**has_more** | **bool** | Whether there are more items after this page. | [readonly] 
**limit** | **int** |  | 
**page** | **int** | Current page number (1-indexed, for display purposes). | [readonly] 
**pages** | **int** | Total number of pages. | [readonly] 
**skip** | **int** |  | 
**total** | **int** |  | 

## Example

```python
from openapi_client.models.paginated_response_episode import PaginatedResponseEpisode

# TODO update the JSON string below
json = "{}"
# create an instance of PaginatedResponseEpisode from a JSON string
paginated_response_episode_instance = PaginatedResponseEpisode.from_json(json)
# print the JSON string representation of the object
print(PaginatedResponseEpisode.to_json())

# convert the object into a dict
paginated_response_episode_dict = paginated_response_episode_instance.to_dict()
# create an instance of PaginatedResponseEpisode from a dict
paginated_response_episode_from_dict = PaginatedResponseEpisode.from_dict(paginated_response_episode_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


