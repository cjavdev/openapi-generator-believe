# Org.OpenAPITools.Model.QuoteCreate
Model for creating a new quote.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**CharacterId** | **string** | ID of the character who said it | 
**Context** | **string** | Context in which the quote was said | 
**MomentType** | **QuoteMoment** | Type of moment when the quote was said | 
**Text** | **string** | The quote text | 
**Theme** | **QuoteTheme** | Primary theme of the quote | 
**EpisodeId** | **string** |  | [optional] 
**IsFunny** | **bool** | Whether this quote is humorous | [optional] [default to false]
**IsInspirational** | **bool** | Whether this quote is inspirational | [optional] [default to true]
**PopularityScore** | **decimal** |  | [optional] 
**SecondaryThemes** | [**List&lt;QuoteTheme&gt;**](QuoteTheme.md) | Additional themes | [optional] 
**TimesShared** | **int** |  | [optional] 

[[Back to Model list]](../../README.md#documentation-for-models) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to README]](../../README.md)

