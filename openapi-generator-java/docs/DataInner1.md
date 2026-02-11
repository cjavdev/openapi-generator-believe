

# DataInner1


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**characterId** | **String** | ID of the character (references /characters/{id}) |  |
|**id** | **String** | Unique identifier for this team membership |  |
|**licenseNumber** | **String** |  |  [optional] |
|**memberType** | [**MemberTypeEnum**](#MemberTypeEnum) | Discriminator field indicating this is an equipment manager |  [optional] |
|**qualifications** | **List&lt;String&gt;** | Medical qualifications and degrees |  [optional] |
|**specialty** | **MedicalSpecialty** | Medical specialty |  |
|**teamId** | **String** | ID of the team they belong to |  |
|**yearsWithTeam** | **Integer** | Number of years with the current team |  |
|**isHeadKitman** | **Boolean** | Whether this is the head equipment manager |  [optional] |
|**responsibilities** | **List&lt;String&gt;** | List of responsibilities |  [optional] |



## Enum: MemberTypeEnum

| Name | Value |
|---- | -----|
| EQUIPMENT_MANAGER | &quot;equipment_manager&quot; |



