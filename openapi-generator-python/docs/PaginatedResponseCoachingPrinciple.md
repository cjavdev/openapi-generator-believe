# PaginatedResponseCoachingPrinciple


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[CoachingPrinciple]**](CoachingPrinciple.md) |  | 
**has_more** | **bool** | Whether there are more items after this page. | [readonly] 
**limit** | **int** |  | 
**page** | **int** | Current page number (1-indexed, for display purposes). | [readonly] 
**pages** | **int** | Total number of pages. | [readonly] 
**skip** | **int** |  | 
**total** | **int** |  | 

## Example

```python
from openapi_client.models.paginated_response_coaching_principle import PaginatedResponseCoachingPrinciple

# TODO update the JSON string below
json = "{}"
# create an instance of PaginatedResponseCoachingPrinciple from a JSON string
paginated_response_coaching_principle_instance = PaginatedResponseCoachingPrinciple.from_json(json)
# print the JSON string representation of the object
print(PaginatedResponseCoachingPrinciple.to_json())

# convert the object into a dict
paginated_response_coaching_principle_dict = paginated_response_coaching_principle_instance.to_dict()
# create an instance of PaginatedResponseCoachingPrinciple from a dict
paginated_response_coaching_principle_from_dict = PaginatedResponseCoachingPrinciple.from_dict(paginated_response_coaching_principle_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


