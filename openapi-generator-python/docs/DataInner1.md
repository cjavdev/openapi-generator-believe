# DataInner1


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**character_id** | **str** | ID of the character (references /characters/{id}) | 
**id** | **str** | Unique identifier for this team membership | 
**license_number** | **str** |  | [optional] 
**member_type** | **str** | Discriminator field indicating this is an equipment manager | [optional] [default to 'equipment_manager']
**qualifications** | **List[str]** | Medical qualifications and degrees | [optional] 
**specialty** | [**MedicalSpecialty**](MedicalSpecialty.md) | Medical specialty | 
**team_id** | **str** | ID of the team they belong to | 
**years_with_team** | **int** | Number of years with the current team | 
**is_head_kitman** | **bool** | Whether this is the head equipment manager | [optional] [default to False]
**responsibilities** | **List[str]** | List of responsibilities | [optional] 

## Example

```python
from openapi_client.models.data_inner1 import DataInner1

# TODO update the JSON string below
json = "{}"
# create an instance of DataInner1 from a JSON string
data_inner1_instance = DataInner1.from_json(json)
# print the JSON string representation of the object
print(DataInner1.to_json())

# convert the object into a dict
data_inner1_dict = data_inner1_instance.to_dict()
# create an instance of DataInner1 from a dict
data_inner1_from_dict = DataInner1.from_dict(data_inner1_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


