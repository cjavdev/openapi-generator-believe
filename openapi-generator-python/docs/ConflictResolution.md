# ConflictResolution

Conflict resolution response.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**barbecue_sauce_wisdom** | **str** | A folksy metaphor to remember | 
**diagnosis** | **str** | Understanding the root cause | 
**diamond_dogs_advice** | **str** | Advice from the Diamond Dogs support group | 
**potential_outcome** | **str** | What resolution could look like | 
**steps_to_resolution** | **List[str]** | Concrete steps to resolve the conflict | 
**ted_approach** | **str** | How Ted would handle this | 

## Example

```python
from openapi_client.models.conflict_resolution import ConflictResolution

# TODO update the JSON string below
json = "{}"
# create an instance of ConflictResolution from a JSON string
conflict_resolution_instance = ConflictResolution.from_json(json)
# print the JSON string representation of the object
print(ConflictResolution.to_json())

# convert the object into a dict
conflict_resolution_dict = conflict_resolution_instance.to_dict()
# create an instance of ConflictResolution from a dict
conflict_resolution_from_dict = ConflictResolution.from_dict(conflict_resolution_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


