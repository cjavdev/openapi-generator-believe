
# EquipmentManagerBase

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **characterId** | **kotlin.String** | ID of the character (references /characters/{id}) |  |
| **teamId** | **kotlin.String** | ID of the team they belong to |  |
| **yearsWithTeam** | **kotlin.Int** | Number of years with the current team |  |
| **isHeadKitman** | **kotlin.Boolean** | Whether this is the head equipment manager |  [optional] |
| **memberType** | [**inline**](#MemberType) | Discriminator field indicating this is an equipment manager |  [optional] |
| **responsibilities** | **kotlin.collections.List&lt;kotlin.String&gt;** | List of responsibilities |  [optional] |


<a id="MemberType"></a>
## Enum: member_type
| Name | Value |
| ---- | ----- |
| memberType | equipment_manager |



