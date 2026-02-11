

# PlayerBase

A football player on the team.

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**assists** | **Integer** | Total assists for the team |  [optional] |
|**characterId** | **String** | ID of the character (references /characters/{id}) |  |
|**goalsScored** | **Integer** | Total goals scored for the team |  [optional] |
|**isCaptain** | **Boolean** | Whether this player is team captain |  [optional] |
|**jerseyNumber** | **Integer** | Jersey/shirt number |  |
|**memberType** | [**MemberTypeEnum**](#MemberTypeEnum) | Discriminator field indicating this is a player |  [optional] |
|**position** | **Position** | Playing position on the field |  |
|**teamId** | **String** | ID of the team they belong to |  |
|**yearsWithTeam** | **Integer** | Number of years with the current team |  |



## Enum: MemberTypeEnum

| Name | Value |
|---- | -----|
| PLAYER | &quot;player&quot; |



