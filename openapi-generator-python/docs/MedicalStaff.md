# MedicalStaff

Full medical staff model with ID.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**character_id** | **str** | ID of the character (references /characters/{id}) | 
**id** | **str** | Unique identifier for this team membership | 
**license_number** | **str** |  | [optional] 
**member_type** | **str** | Discriminator field indicating this is medical staff | [optional] [default to 'medical_staff']
**qualifications** | **List[str]** | Medical qualifications and degrees | [optional] 
**specialty** | [**MedicalSpecialty**](MedicalSpecialty.md) | Medical specialty | 
**team_id** | **str** | ID of the team they belong to | 
**years_with_team** | **int** | Number of years with the current team | 

## Example

```python
from openapi_client.models.medical_staff import MedicalStaff

# TODO update the JSON string below
json = "{}"
# create an instance of MedicalStaff from a JSON string
medical_staff_instance = MedicalStaff.from_json(json)
# print the JSON string representation of the object
print(MedicalStaff.to_json())

# convert the object into a dict
medical_staff_dict = medical_staff_instance.to_dict()
# create an instance of MedicalStaff from a dict
medical_staff_from_dict = MedicalStaff.from_dict(medical_staff_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


