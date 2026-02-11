# Member


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**assists** | **int** | Total assists for the team | [optional] [default to 0]
**character_id** | **str** | ID of the character (references /characters/{id}) | 
**goals_scored** | **int** | Total goals scored for the team | [optional] [default to 0]
**is_captain** | **bool** | Whether this player is team captain | [optional] [default to False]
**jersey_number** | **int** | Jersey/shirt number | 
**member_type** | **str** | Discriminator field indicating this is an equipment manager | [optional] [default to 'equipment_manager']
**position** | [**Position**](Position.md) | Playing position on the field | 
**team_id** | **str** | ID of the team they belong to | 
**years_with_team** | **int** | Number of years with the current team | 
**certifications** | **List[str]** | Coaching certifications and licenses | [optional] 
**specialty** | [**MedicalSpecialty**](MedicalSpecialty.md) | Medical specialty | 
**win_rate** | **float** |  | [optional] 
**license_number** | **str** |  | [optional] 
**qualifications** | **List[str]** | Medical qualifications and degrees | [optional] 
**is_head_kitman** | **bool** | Whether this is the head equipment manager | [optional] [default to False]
**responsibilities** | **List[str]** | List of responsibilities | [optional] 

## Example

```python
from openapi_client.models.member import Member

# TODO update the JSON string below
json = "{}"
# create an instance of Member from a JSON string
member_instance = Member.from_json(json)
# print the JSON string representation of the object
print(Member.to_json())

# convert the object into a dict
member_dict = member_instance.to_dict()
# create an instance of Member from a dict
member_from_dict = Member.from_dict(member_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


