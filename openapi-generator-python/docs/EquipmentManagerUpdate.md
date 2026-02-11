# EquipmentManagerUpdate

Update model for equipment managers.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**is_head_kitman** | **bool** |  | [optional] 
**responsibilities** | **List[str]** |  | [optional] 
**team_id** | **str** |  | [optional] 
**years_with_team** | **int** |  | [optional] 

## Example

```python
from openapi_client.models.equipment_manager_update import EquipmentManagerUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of EquipmentManagerUpdate from a JSON string
equipment_manager_update_instance = EquipmentManagerUpdate.from_json(json)
# print the JSON string representation of the object
print(EquipmentManagerUpdate.to_json())

# convert the object into a dict
equipment_manager_update_dict = equipment_manager_update_instance.to_dict()
# create an instance of EquipmentManagerUpdate from a dict
equipment_manager_update_from_dict = EquipmentManagerUpdate.from_dict(equipment_manager_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


