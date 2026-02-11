

# CharacterCreate

Model for creating a new character.

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**background** | **String** | Character background and history |  |
|**dateOfBirth** | **LocalDate** |  |  [optional] |
|**email** | **String** |  |  [optional] |
|**emotionalStats** | [**EmotionalStats**](EmotionalStats.md) | Emotional intelligence stats |  |
|**growthArcs** | [**List&lt;GrowthArc&gt;**](GrowthArc.md) | Character development across seasons |  [optional] |
|**heightMeters** | **BigDecimal** |  |  [optional] |
|**name** | **String** | Character&#39;s full name |  |
|**personalityTraits** | **List&lt;String&gt;** | Key personality traits |  |
|**profileImageUrl** | **URI** |  |  [optional] |
|**role** | **CharacterRole** | Character&#39;s role |  |
|**salaryGbp** | [**SalaryGbp**](SalaryGbp.md) |  |  [optional] |
|**signatureQuotes** | **List&lt;String&gt;** | Memorable quotes from this character |  [optional] |
|**teamId** | **String** |  |  [optional] |



