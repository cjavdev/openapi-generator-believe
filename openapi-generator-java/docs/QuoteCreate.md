

# QuoteCreate

Model for creating a new quote.

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**characterId** | **String** | ID of the character who said it |  |
|**context** | **String** | Context in which the quote was said |  |
|**episodeId** | **String** |  |  [optional] |
|**isFunny** | **Boolean** | Whether this quote is humorous |  [optional] |
|**isInspirational** | **Boolean** | Whether this quote is inspirational |  [optional] |
|**momentType** | **QuoteMoment** | Type of moment when the quote was said |  |
|**popularityScore** | **BigDecimal** |  |  [optional] |
|**secondaryThemes** | **List&lt;QuoteTheme&gt;** | Additional themes |  [optional] |
|**text** | **String** | The quote text |  |
|**theme** | **QuoteTheme** | Primary theme of the quote |  |
|**timesShared** | **Integer** |  |  [optional] |



