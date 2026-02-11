

# Coach

Full coach model with ID.

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**certifications** | **List&lt;String&gt;** | Coaching certifications and licenses |  [optional] |
|**characterId** | **String** | ID of the character (references /characters/{id}) |  |
|**id** | **String** | Unique identifier for this team membership |  |
|**memberType** | [**MemberTypeEnum**](#MemberTypeEnum) | Discriminator field indicating this is a coach |  [optional] |
|**specialty** | **CoachSpecialty** | Coaching specialty/role |  |
|**teamId** | **String** | ID of the team they belong to |  |
|**winRate** | **BigDecimal** |  |  [optional] |
|**yearsWithTeam** | **Integer** | Number of years with the current team |  |



## Enum: MemberTypeEnum

| Name | Value |
|---- | -----|
| COACH | &quot;coach&quot; |



