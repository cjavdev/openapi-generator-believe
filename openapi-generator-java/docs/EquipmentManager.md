

# EquipmentManager

Full equipment manager model with ID.

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**characterId** | **String** | ID of the character (references /characters/{id}) |  |
|**id** | **String** | Unique identifier for this team membership |  |
|**isHeadKitman** | **Boolean** | Whether this is the head equipment manager |  [optional] |
|**memberType** | [**MemberTypeEnum**](#MemberTypeEnum) | Discriminator field indicating this is an equipment manager |  [optional] |
|**responsibilities** | **List&lt;String&gt;** | List of responsibilities |  [optional] |
|**teamId** | **String** | ID of the team they belong to |  |
|**yearsWithTeam** | **Integer** | Number of years with the current team |  |



## Enum: MemberTypeEnum

| Name | Value |
|---- | -----|
| EQUIPMENT_MANAGER | &quot;equipment_manager&quot; |



