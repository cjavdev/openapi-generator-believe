# # QuoteCreate

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**character_id** | **string** | ID of the character who said it |
**context** | **string** | Context in which the quote was said |
**episode_id** | **string** |  | [optional]
**is_funny** | **bool** | Whether this quote is humorous | [optional] [default to false]
**is_inspirational** | **bool** | Whether this quote is inspirational | [optional] [default to true]
**moment_type** | [**\OpenAPI\Client\Model\QuoteMoment**](QuoteMoment.md) | Type of moment when the quote was said |
**popularity_score** | **float** |  | [optional]
**secondary_themes** | [**\OpenAPI\Client\Model\QuoteTheme[]**](QuoteTheme.md) | Additional themes | [optional]
**text** | **string** | The quote text |
**theme** | [**\OpenAPI\Client\Model\QuoteTheme**](QuoteTheme.md) | Primary theme of the quote |
**times_shared** | **int** |  | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
