# MedicalStaffUpdate

Update model for medical staff.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**license_number** | **str** |  | [optional] 
**qualifications** | **List[str]** |  | [optional] 
**specialty** | [**MedicalSpecialty**](MedicalSpecialty.md) |  | [optional] 
**team_id** | **str** |  | [optional] 
**years_with_team** | **int** |  | [optional] 

## Example

```python
from openapi_client.models.medical_staff_update import MedicalStaffUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of MedicalStaffUpdate from a JSON string
medical_staff_update_instance = MedicalStaffUpdate.from_json(json)
# print the JSON string representation of the object
print(MedicalStaffUpdate.to_json())

# convert the object into a dict
medical_staff_update_dict = medical_staff_update_instance.to_dict()
# create an instance of MedicalStaffUpdate from a dict
medical_staff_update_from_dict = MedicalStaffUpdate.from_dict(medical_staff_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


