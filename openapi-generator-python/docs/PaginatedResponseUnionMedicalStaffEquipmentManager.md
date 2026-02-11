# PaginatedResponseUnionMedicalStaffEquipmentManager


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[DataInner1]**](DataInner1.md) |  | 
**has_more** | **bool** | Whether there are more items after this page. | [readonly] 
**limit** | **int** |  | 
**page** | **int** | Current page number (1-indexed, for display purposes). | [readonly] 
**pages** | **int** | Total number of pages. | [readonly] 
**skip** | **int** |  | 
**total** | **int** |  | 

## Example

```python
from openapi_client.models.paginated_response_union_medical_staff_equipment_manager import PaginatedResponseUnionMedicalStaffEquipmentManager

# TODO update the JSON string below
json = "{}"
# create an instance of PaginatedResponseUnionMedicalStaffEquipmentManager from a JSON string
paginated_response_union_medical_staff_equipment_manager_instance = PaginatedResponseUnionMedicalStaffEquipmentManager.from_json(json)
# print the JSON string representation of the object
print(PaginatedResponseUnionMedicalStaffEquipmentManager.to_json())

# convert the object into a dict
paginated_response_union_medical_staff_equipment_manager_dict = paginated_response_union_medical_staff_equipment_manager_instance.to_dict()
# create an instance of PaginatedResponseUnionMedicalStaffEquipmentManager from a dict
paginated_response_union_medical_staff_equipment_manager_from_dict = PaginatedResponseUnionMedicalStaffEquipmentManager.from_dict(paginated_response_union_medical_staff_equipment_manager_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


