

# ResponseGetTeamMemberTeamMembersMemberIdGet


## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**assists** | **Integer** | Total assists for the team |  [optional] |
|**characterId** | **String** | ID of the character (references /characters/{id}) |  |
|**goalsScored** | **Integer** | Total goals scored for the team |  [optional] |
|**id** | **String** | Unique identifier for this team membership |  |
|**isCaptain** | **Boolean** | Whether this player is team captain |  [optional] |
|**jerseyNumber** | **Integer** | Jersey/shirt number |  |
|**memberType** | [**MemberTypeEnum**](#MemberTypeEnum) | Discriminator field indicating this is an equipment manager |  [optional] |
|**position** | **Position** | Playing position on the field |  |
|**teamId** | **String** | ID of the team they belong to |  |
|**yearsWithTeam** | **Integer** | Number of years with the current team |  |
|**certifications** | **List&lt;String&gt;** | Coaching certifications and licenses |  [optional] |
|**specialty** | **MedicalSpecialty** | Medical specialty |  |
|**winRate** | **BigDecimal** |  |  [optional] |
|**licenseNumber** | **String** |  |  [optional] |
|**qualifications** | **List&lt;String&gt;** | Medical qualifications and degrees |  [optional] |
|**isHeadKitman** | **Boolean** | Whether this is the head equipment manager |  [optional] |
|**responsibilities** | **List&lt;String&gt;** | List of responsibilities |  [optional] |



## Enum: MemberTypeEnum

| Name | Value |
|---- | -----|
| EQUIPMENT_MANAGER | &quot;equipment_manager&quot; |



