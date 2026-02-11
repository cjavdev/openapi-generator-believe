# GrowthArc

Character development arc.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**breakthrough** | **str** | Key breakthrough moment | 
**challenge** | **str** | Main challenge faced | 
**ending_point** | **str** | Where the character ends up | 
**season** | **int** | Season number | 
**starting_point** | **str** | Where the character starts emotionally | 

## Example

```python
from openapi_client.models.growth_arc import GrowthArc

# TODO update the JSON string below
json = "{}"
# create an instance of GrowthArc from a JSON string
growth_arc_instance = GrowthArc.from_json(json)
# print the JSON string representation of the object
print(GrowthArc.to_json())

# convert the object into a dict
growth_arc_dict = growth_arc_instance.to_dict()
# create an instance of GrowthArc from a dict
growth_arc_from_dict = GrowthArc.from_dict(growth_arc_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


