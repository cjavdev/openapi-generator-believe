
# Coach

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **characterId** | **kotlin.String** | ID of the character (references /characters/{id}) |  |
| **id** | **kotlin.String** | Unique identifier for this team membership |  |
| **specialty** | [**CoachSpecialty**](CoachSpecialty.md) | Coaching specialty/role |  |
| **teamId** | **kotlin.String** | ID of the team they belong to |  |
| **yearsWithTeam** | **kotlin.Int** | Number of years with the current team |  |
| **certifications** | **kotlin.collections.List&lt;kotlin.String&gt;** | Coaching certifications and licenses |  [optional] |
| **memberType** | [**inline**](#MemberType) | Discriminator field indicating this is a coach |  [optional] |
| **winRate** | [**java.math.BigDecimal**](java.math.BigDecimal.md) |  |  [optional] |


<a id="MemberType"></a>
## Enum: member_type
| Name | Value |
| ---- | ----- |
| memberType | coach |



