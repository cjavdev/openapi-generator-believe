# CoachBase

A coach or coaching staff member.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**certifications** | **List[str]** | Coaching certifications and licenses | [optional] 
**character_id** | **str** | ID of the character (references /characters/{id}) | 
**member_type** | **str** | Discriminator field indicating this is a coach | [optional] [default to 'coach']
**specialty** | [**CoachSpecialty**](CoachSpecialty.md) | Coaching specialty/role | 
**team_id** | **str** | ID of the team they belong to | 
**win_rate** | **float** |  | [optional] 
**years_with_team** | **int** | Number of years with the current team | 

## Example

```python
from openapi_client.models.coach_base import CoachBase

# TODO update the JSON string below
json = "{}"
# create an instance of CoachBase from a JSON string
coach_base_instance = CoachBase.from_json(json)
# print the JSON string representation of the object
print(CoachBase.to_json())

# convert the object into a dict
coach_base_dict = coach_base_instance.to_dict()
# create an instance of CoachBase from a dict
coach_base_from_dict = CoachBase.from_dict(coach_base_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


