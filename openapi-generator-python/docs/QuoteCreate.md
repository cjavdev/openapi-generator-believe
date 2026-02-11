# QuoteCreate

Model for creating a new quote.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**character_id** | **str** | ID of the character who said it | 
**context** | **str** | Context in which the quote was said | 
**episode_id** | **str** |  | [optional] 
**is_funny** | **bool** | Whether this quote is humorous | [optional] [default to False]
**is_inspirational** | **bool** | Whether this quote is inspirational | [optional] [default to True]
**moment_type** | [**QuoteMoment**](QuoteMoment.md) | Type of moment when the quote was said | 
**popularity_score** | **float** |  | [optional] 
**secondary_themes** | [**List[QuoteTheme]**](QuoteTheme.md) | Additional themes | [optional] 
**text** | **str** | The quote text | 
**theme** | [**QuoteTheme**](QuoteTheme.md) | Primary theme of the quote | 
**times_shared** | **int** |  | [optional] 

## Example

```python
from openapi_client.models.quote_create import QuoteCreate

# TODO update the JSON string below
json = "{}"
# create an instance of QuoteCreate from a JSON string
quote_create_instance = QuoteCreate.from_json(json)
# print the JSON string representation of the object
print(QuoteCreate.to_json())

# convert the object into a dict
quote_create_dict = quote_create_instance.to_dict()
# create an instance of QuoteCreate from a dict
quote_create_from_dict = QuoteCreate.from_dict(quote_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


