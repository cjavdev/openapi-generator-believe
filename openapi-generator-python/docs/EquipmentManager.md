# EquipmentManager

Full equipment manager model with ID.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**character_id** | **str** | ID of the character (references /characters/{id}) | 
**id** | **str** | Unique identifier for this team membership | 
**is_head_kitman** | **bool** | Whether this is the head equipment manager | [optional] [default to False]
**member_type** | **str** | Discriminator field indicating this is an equipment manager | [optional] [default to 'equipment_manager']
**responsibilities** | **List[str]** | List of responsibilities | [optional] 
**team_id** | **str** | ID of the team they belong to | 
**years_with_team** | **int** | Number of years with the current team | 

## Example

```python
from openapi_client.models.equipment_manager import EquipmentManager

# TODO update the JSON string below
json = "{}"
# create an instance of EquipmentManager from a JSON string
equipment_manager_instance = EquipmentManager.from_json(json)
# print the JSON string representation of the object
print(EquipmentManager.to_json())

# convert the object into a dict
equipment_manager_dict = equipment_manager_instance.to_dict()
# create an instance of EquipmentManager from a dict
equipment_manager_from_dict = EquipmentManager.from_dict(equipment_manager_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


