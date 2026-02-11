
# MedicalStaffBase

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **characterId** | **kotlin.String** | ID of the character (references /characters/{id}) |  |
| **specialty** | [**MedicalSpecialty**](MedicalSpecialty.md) | Medical specialty |  |
| **teamId** | **kotlin.String** | ID of the team they belong to |  |
| **yearsWithTeam** | **kotlin.Int** | Number of years with the current team |  |
| **licenseNumber** | **kotlin.String** |  |  [optional] |
| **memberType** | [**inline**](#MemberType) | Discriminator field indicating this is medical staff |  [optional] |
| **qualifications** | **kotlin.collections.List&lt;kotlin.String&gt;** | Medical qualifications and degrees |  [optional] |


<a id="MemberType"></a>
## Enum: member_type
| Name | Value |
| ---- | ----- |
| memberType | medical_staff |



