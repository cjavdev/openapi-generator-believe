

# MedicalStaffBase

Medical and wellness staff member.

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**characterId** | **String** | ID of the character (references /characters/{id}) |  |
|**licenseNumber** | **String** |  |  [optional] |
|**memberType** | [**MemberTypeEnum**](#MemberTypeEnum) | Discriminator field indicating this is medical staff |  [optional] |
|**qualifications** | **List&lt;String&gt;** | Medical qualifications and degrees |  [optional] |
|**specialty** | **MedicalSpecialty** | Medical specialty |  |
|**teamId** | **String** | ID of the team they belong to |  |
|**yearsWithTeam** | **Integer** | Number of years with the current team |  |



## Enum: MemberTypeEnum

| Name | Value |
|---- | -----|
| MEDICAL_STAFF | &quot;medical_staff&quot; |



