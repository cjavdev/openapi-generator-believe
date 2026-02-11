# # MedicalStaffBase

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**character_id** | **string** | ID of the character (references /characters/{id}) |
**license_number** | **string** |  | [optional]
**member_type** | **string** | Discriminator field indicating this is medical staff | [optional] [default to 'medical_staff']
**qualifications** | **string[]** | Medical qualifications and degrees | [optional]
**specialty** | [**\OpenAPI\Client\Model\MedicalSpecialty**](MedicalSpecialty.md) | Medical specialty |
**team_id** | **string** | ID of the team they belong to |
**years_with_team** | **int** | Number of years with the current team |

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
