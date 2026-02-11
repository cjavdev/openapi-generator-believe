
# DataInner

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **characterId** | **kotlin.String** | ID of the character (references /characters/{id}) |  |
| **id** | **kotlin.String** | Unique identifier for this team membership |  |
| **jerseyNumber** | **kotlin.Int** | Jersey/shirt number |  |
| **position** | [**Position**](Position.md) | Playing position on the field |  |
| **teamId** | **kotlin.String** | ID of the team they belong to |  |
| **yearsWithTeam** | **kotlin.Int** | Number of years with the current team |  |
| **specialty** | [**MedicalSpecialty**](MedicalSpecialty.md) | Medical specialty |  |
| **assists** | **kotlin.Int** | Total assists for the team |  [optional] |
| **goalsScored** | **kotlin.Int** | Total goals scored for the team |  [optional] |
| **isCaptain** | **kotlin.Boolean** | Whether this player is team captain |  [optional] |
| **memberType** | [**inline**](#MemberType) | Discriminator field indicating this is an equipment manager |  [optional] |
| **certifications** | **kotlin.collections.List&lt;kotlin.String&gt;** | Coaching certifications and licenses |  [optional] |
| **winRate** | [**java.math.BigDecimal**](java.math.BigDecimal.md) |  |  [optional] |
| **licenseNumber** | **kotlin.String** |  |  [optional] |
| **qualifications** | **kotlin.collections.List&lt;kotlin.String&gt;** | Medical qualifications and degrees |  [optional] |
| **isHeadKitman** | **kotlin.Boolean** | Whether this is the head equipment manager |  [optional] |
| **responsibilities** | **kotlin.collections.List&lt;kotlin.String&gt;** | List of responsibilities |  [optional] |


<a id="MemberType"></a>
## Enum: member_type
| Name | Value |
| ---- | ----- |
| memberType | equipment_manager |



