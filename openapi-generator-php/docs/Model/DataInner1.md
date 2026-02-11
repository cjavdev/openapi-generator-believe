# # DataInner1

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**character_id** | **string** | ID of the character (references /characters/{id}) |
**id** | **string** | Unique identifier for this team membership |
**license_number** | **string** |  | [optional]
**member_type** | **string** | Discriminator field indicating this is an equipment manager | [optional] [default to 'equipment_manager']
**qualifications** | **string[]** | Medical qualifications and degrees | [optional]
**specialty** | [**\OpenAPI\Client\Model\MedicalSpecialty**](MedicalSpecialty.md) | Medical specialty |
**team_id** | **string** | ID of the team they belong to |
**years_with_team** | **int** | Number of years with the current team |
**is_head_kitman** | **bool** | Whether this is the head equipment manager | [optional] [default to false]
**responsibilities** | **string[]** | List of responsibilities | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
