# CoachingPrinciple

A Ted Lasso coaching principle.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**application** | **str** | How to apply this principle | 
**example_from_show** | **str** | Example from the show | 
**explanation** | **str** | What this principle means | 
**id** | **str** | Principle identifier | 
**principle** | **str** | The coaching principle | 
**ted_quote** | **str** | Related Ted quote | 

## Example

```python
from openapi_client.models.coaching_principle import CoachingPrinciple

# TODO update the JSON string below
json = "{}"
# create an instance of CoachingPrinciple from a JSON string
coaching_principle_instance = CoachingPrinciple.from_json(json)
# print the JSON string representation of the object
print(CoachingPrinciple.to_json())

# convert the object into a dict
coaching_principle_dict = coaching_principle_instance.to_dict()
# create an instance of CoachingPrinciple from a dict
coaching_principle_from_dict = CoachingPrinciple.from_dict(coaching_principle_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


