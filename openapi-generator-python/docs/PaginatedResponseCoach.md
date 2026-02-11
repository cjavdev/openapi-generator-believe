# PaginatedResponseCoach


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[Coach]**](Coach.md) |  | 
**has_more** | **bool** | Whether there are more items after this page. | [readonly] 
**limit** | **int** |  | 
**page** | **int** | Current page number (1-indexed, for display purposes). | [readonly] 
**pages** | **int** | Total number of pages. | [readonly] 
**skip** | **int** |  | 
**total** | **int** |  | 

## Example

```python
from openapi_client.models.paginated_response_coach import PaginatedResponseCoach

# TODO update the JSON string below
json = "{}"
# create an instance of PaginatedResponseCoach from a JSON string
paginated_response_coach_instance = PaginatedResponseCoach.from_json(json)
# print the JSON string representation of the object
print(PaginatedResponseCoach.to_json())

# convert the object into a dict
paginated_response_coach_dict = paginated_response_coach_instance.to_dict()
# create an instance of PaginatedResponseCoach from a dict
paginated_response_coach_from_dict = PaginatedResponseCoach.from_dict(paginated_response_coach_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


