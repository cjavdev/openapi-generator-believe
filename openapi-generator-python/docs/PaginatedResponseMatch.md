# PaginatedResponseMatch


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[Match]**](Match.md) |  | 
**has_more** | **bool** | Whether there are more items after this page. | [readonly] 
**limit** | **int** |  | 
**page** | **int** | Current page number (1-indexed, for display purposes). | [readonly] 
**pages** | **int** | Total number of pages. | [readonly] 
**skip** | **int** |  | 
**total** | **int** |  | 

## Example

```python
from openapi_client.models.paginated_response_match import PaginatedResponseMatch

# TODO update the JSON string below
json = "{}"
# create an instance of PaginatedResponseMatch from a JSON string
paginated_response_match_instance = PaginatedResponseMatch.from_json(json)
# print the JSON string representation of the object
print(PaginatedResponseMatch.to_json())

# convert the object into a dict
paginated_response_match_dict = paginated_response_match_instance.to_dict()
# create an instance of PaginatedResponseMatch from a dict
paginated_response_match_from_dict = PaginatedResponseMatch.from_dict(paginated_response_match_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


