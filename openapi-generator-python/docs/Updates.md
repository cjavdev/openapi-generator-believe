# Updates


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**assists** | **int** |  | [optional] 
**goals_scored** | **int** |  | [optional] 
**is_captain** | **bool** |  | [optional] 
**jersey_number** | **int** |  | [optional] 
**position** | [**Position**](Position.md) |  | [optional] 
**team_id** | **str** |  | [optional] 
**years_with_team** | **int** |  | [optional] 
**certifications** | **List[str]** |  | [optional] 
**specialty** | [**MedicalSpecialty**](MedicalSpecialty.md) |  | [optional] 
**win_rate** | **float** |  | [optional] 
**license_number** | **str** |  | [optional] 
**qualifications** | **List[str]** |  | [optional] 
**is_head_kitman** | **bool** |  | [optional] 
**responsibilities** | **List[str]** |  | [optional] 

## Example

```python
from openapi_client.models.updates import Updates

# TODO update the JSON string below
json = "{}"
# create an instance of Updates from a JSON string
updates_instance = Updates.from_json(json)
# print the JSON string representation of the object
print(Updates.to_json())

# convert the object into a dict
updates_dict = updates_instance.to_dict()
# create an instance of Updates from a dict
updates_from_dict = Updates.from_dict(updates_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


