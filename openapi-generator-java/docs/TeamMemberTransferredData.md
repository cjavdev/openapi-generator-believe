

# TeamMemberTransferredData

Data payload for a team member transfer event.

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**characterId** | **String** | ID of the character (links to /characters) |  |
|**characterName** | **String** | Name of the character |  |
|**memberType** | [**MemberTypeEnum**](#MemberTypeEnum) | Type of team member |  |
|**previousTeamId** | **String** | Previous team ID (for joins from another team) |  [optional] |
|**previousTeamName** | **String** | Previous team name (for joins from another team) |  [optional] |
|**teamId** | **String** | ID of the team involved |  |
|**teamMemberId** | **String** | ID of the team member |  |
|**teamName** | **String** | Name of the team involved |  |
|**tedReaction** | **String** | Ted&#39;s reaction to the transfer |  |
|**transferFeeGbp** | **String** | Transfer fee in GBP (for players) |  [optional] |
|**transferType** | [**TransferTypeEnum**](#TransferTypeEnum) | Whether the member joined or departed |  |
|**yearsWithPreviousTeam** | **Integer** | Years spent with previous team |  [optional] |



## Enum: MemberTypeEnum

| Name | Value |
|---- | -----|
| PLAYER | &quot;player&quot; |
| COACH | &quot;coach&quot; |
| MEDICAL_STAFF | &quot;medical_staff&quot; |
| EQUIPMENT_MANAGER | &quot;equipment_manager&quot; |



## Enum: TransferTypeEnum

| Name | Value |
|---- | -----|
| JOINED | &quot;joined&quot; |
| DEPARTED | &quot;departed&quot; |



