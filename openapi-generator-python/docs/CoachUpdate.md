# CoachUpdate

Update model for coaches.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**certifications** | **List[str]** |  | [optional] 
**specialty** | [**CoachSpecialty**](CoachSpecialty.md) |  | [optional] 
**team_id** | **str** |  | [optional] 
**win_rate** | **float** |  | [optional] 
**years_with_team** | **int** |  | [optional] 

## Example

```python
from openapi_client.models.coach_update import CoachUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of CoachUpdate from a JSON string
coach_update_instance = CoachUpdate.from_json(json)
# print the JSON string representation of the object
print(CoachUpdate.to_json())

# convert the object into a dict
coach_update_dict = coach_update_instance.to_dict()
# create an instance of CoachUpdate from a dict
coach_update_from_dict = CoachUpdate.from_dict(coach_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


