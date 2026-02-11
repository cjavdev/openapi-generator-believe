# EquipmentManagerBase

Equipment and kit management staff.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**character_id** | **str** | ID of the character (references /characters/{id}) | 
**is_head_kitman** | **bool** | Whether this is the head equipment manager | [optional] [default to False]
**member_type** | **str** | Discriminator field indicating this is an equipment manager | [optional] [default to 'equipment_manager']
**responsibilities** | **List[str]** | List of responsibilities | [optional] 
**team_id** | **str** | ID of the team they belong to | 
**years_with_team** | **int** | Number of years with the current team | 

## Example

```python
from openapi_client.models.equipment_manager_base import EquipmentManagerBase

# TODO update the JSON string below
json = "{}"
# create an instance of EquipmentManagerBase from a JSON string
equipment_manager_base_instance = EquipmentManagerBase.from_json(json)
# print the JSON string representation of the object
print(EquipmentManagerBase.to_json())

# convert the object into a dict
equipment_manager_base_dict = equipment_manager_base_instance.to_dict()
# create an instance of EquipmentManagerBase from a dict
equipment_manager_base_from_dict = EquipmentManagerBase.from_dict(equipment_manager_base_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


