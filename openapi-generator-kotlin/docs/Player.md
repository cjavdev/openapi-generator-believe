
# Player

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **characterId** | **kotlin.String** | ID of the character (references /characters/{id}) |  |
| **id** | **kotlin.String** | Unique identifier for this team membership |  |
| **jerseyNumber** | **kotlin.Int** | Jersey/shirt number |  |
| **position** | [**Position**](Position.md) | Playing position on the field |  |
| **teamId** | **kotlin.String** | ID of the team they belong to |  |
| **yearsWithTeam** | **kotlin.Int** | Number of years with the current team |  |
| **assists** | **kotlin.Int** | Total assists for the team |  [optional] |
| **goalsScored** | **kotlin.Int** | Total goals scored for the team |  [optional] |
| **isCaptain** | **kotlin.Boolean** | Whether this player is team captain |  [optional] |
| **memberType** | [**inline**](#MemberType) | Discriminator field indicating this is a player |  [optional] |


<a id="MemberType"></a>
## Enum: member_type
| Name | Value |
| ---- | ----- |
| memberType | player |



