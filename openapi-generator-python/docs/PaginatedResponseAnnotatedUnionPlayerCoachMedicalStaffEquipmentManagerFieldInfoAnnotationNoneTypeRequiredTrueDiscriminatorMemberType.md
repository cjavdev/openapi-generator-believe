# PaginatedResponseAnnotatedUnionPlayerCoachMedicalStaffEquipmentManagerFieldInfoAnnotationNoneTypeRequiredTrueDiscriminatorMemberType


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[DataInner]**](DataInner.md) |  | 
**has_more** | **bool** | Whether there are more items after this page. | [readonly] 
**limit** | **int** |  | 
**page** | **int** | Current page number (1-indexed, for display purposes). | [readonly] 
**pages** | **int** | Total number of pages. | [readonly] 
**skip** | **int** |  | 
**total** | **int** |  | 

## Example

```python
from openapi_client.models.paginated_response_annotated_union_player_coach_medical_staff_equipment_manager_field_info_annotation_none_type_required_true_discriminator_member_type import PaginatedResponseAnnotatedUnionPlayerCoachMedicalStaffEquipmentManagerFieldInfoAnnotationNoneTypeRequiredTrueDiscriminatorMemberType

# TODO update the JSON string below
json = "{}"
# create an instance of PaginatedResponseAnnotatedUnionPlayerCoachMedicalStaffEquipmentManagerFieldInfoAnnotationNoneTypeRequiredTrueDiscriminatorMemberType from a JSON string
paginated_response_annotated_union_player_coach_medical_staff_equipment_manager_field_info_annotation_none_type_required_true_discriminator_member_type_instance = PaginatedResponseAnnotatedUnionPlayerCoachMedicalStaffEquipmentManagerFieldInfoAnnotationNoneTypeRequiredTrueDiscriminatorMemberType.from_json(json)
# print the JSON string representation of the object
print(PaginatedResponseAnnotatedUnionPlayerCoachMedicalStaffEquipmentManagerFieldInfoAnnotationNoneTypeRequiredTrueDiscriminatorMemberType.to_json())

# convert the object into a dict
paginated_response_annotated_union_player_coach_medical_staff_equipment_manager_field_info_annotation_none_type_required_true_discriminator_member_type_dict = paginated_response_annotated_union_player_coach_medical_staff_equipment_manager_field_info_annotation_none_type_required_true_discriminator_member_type_instance.to_dict()
# create an instance of PaginatedResponseAnnotatedUnionPlayerCoachMedicalStaffEquipmentManagerFieldInfoAnnotationNoneTypeRequiredTrueDiscriminatorMemberType from a dict
paginated_response_annotated_union_player_coach_medical_staff_equipment_manager_field_info_annotation_none_type_required_true_discriminator_member_type_from_dict = PaginatedResponseAnnotatedUnionPlayerCoachMedicalStaffEquipmentManagerFieldInfoAnnotationNoneTypeRequiredTrueDiscriminatorMemberType.from_dict(paginated_response_annotated_union_player_coach_medical_staff_equipment_manager_field_info_annotation_none_type_required_true_discriminator_member_type_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


