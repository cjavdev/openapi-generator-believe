# Coach

Full coach model with ID.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**certifications** | **List[str]** | Coaching certifications and licenses | [optional] 
**character_id** | **str** | ID of the character (references /characters/{id}) | 
**id** | **str** | Unique identifier for this team membership | 
**member_type** | **str** | Discriminator field indicating this is a coach | [optional] [default to 'coach']
**specialty** | [**CoachSpecialty**](CoachSpecialty.md) | Coaching specialty/role | 
**team_id** | **str** | ID of the team they belong to | 
**win_rate** | **float** |  | [optional] 
**years_with_team** | **int** | Number of years with the current team | 

## Example

```python
from openapi_client.models.coach import Coach

# TODO update the JSON string below
json = "{}"
# create an instance of Coach from a JSON string
coach_instance = Coach.from_json(json)
# print the JSON string representation of the object
print(Coach.to_json())

# convert the object into a dict
coach_dict = coach_instance.to_dict()
# create an instance of Coach from a dict
coach_from_dict = Coach.from_dict(coach_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


