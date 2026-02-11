# MedicalStaffBase

Medical and wellness staff member.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**character_id** | **str** | ID of the character (references /characters/{id}) | 
**license_number** | **str** |  | [optional] 
**member_type** | **str** | Discriminator field indicating this is medical staff | [optional] [default to 'medical_staff']
**qualifications** | **List[str]** | Medical qualifications and degrees | [optional] 
**specialty** | [**MedicalSpecialty**](MedicalSpecialty.md) | Medical specialty | 
**team_id** | **str** | ID of the team they belong to | 
**years_with_team** | **int** | Number of years with the current team | 

## Example

```python
from openapi_client.models.medical_staff_base import MedicalStaffBase

# TODO update the JSON string below
json = "{}"
# create an instance of MedicalStaffBase from a JSON string
medical_staff_base_instance = MedicalStaffBase.from_json(json)
# print the JSON string representation of the object
print(MedicalStaffBase.to_json())

# convert the object into a dict
medical_staff_base_dict = medical_staff_base_instance.to_dict()
# create an instance of MedicalStaffBase from a dict
medical_staff_base_from_dict = MedicalStaffBase.from_dict(medical_staff_base_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


