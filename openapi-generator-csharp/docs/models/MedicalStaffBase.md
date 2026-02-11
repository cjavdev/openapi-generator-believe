# Org.OpenAPITools.Model.MedicalStaffBase
Medical and wellness staff member.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**CharacterId** | **string** | ID of the character (references /characters/{id}) | 
**Specialty** | **MedicalSpecialty** | Medical specialty | 
**TeamId** | **string** | ID of the team they belong to | 
**YearsWithTeam** | **int** | Number of years with the current team | 
**LicenseNumber** | **string** |  | [optional] 
**MemberType** | **string** | Discriminator field indicating this is medical staff | [optional] [default to MemberTypeEnum.MedicalStaff]
**Qualifications** | **List&lt;string&gt;** | Medical qualifications and degrees | [optional] 

[[Back to Model list]](../../README.md#documentation-for-models) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to README]](../../README.md)

