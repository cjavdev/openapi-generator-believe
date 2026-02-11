# QuoteUpdate

Model for updating a quote (all fields optional).

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**character_id** | **str** |  | [optional] 
**context** | **str** |  | [optional] 
**episode_id** | **str** |  | [optional] 
**is_funny** | **bool** |  | [optional] 
**is_inspirational** | **bool** |  | [optional] 
**moment_type** | [**QuoteMoment**](QuoteMoment.md) |  | [optional] 
**popularity_score** | **float** |  | [optional] 
**secondary_themes** | [**List[QuoteTheme]**](QuoteTheme.md) |  | [optional] 
**text** | **str** |  | [optional] 
**theme** | [**QuoteTheme**](QuoteTheme.md) |  | [optional] 
**times_shared** | **int** |  | [optional] 

## Example

```python
from openapi_client.models.quote_update import QuoteUpdate

# TODO update the JSON string below
json = "{}"
# create an instance of QuoteUpdate from a JSON string
quote_update_instance = QuoteUpdate.from_json(json)
# print the JSON string representation of the object
print(QuoteUpdate.to_json())

# convert the object into a dict
quote_update_dict = quote_update_instance.to_dict()
# create an instance of QuoteUpdate from a dict
quote_update_from_dict = QuoteUpdate.from_dict(quote_update_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


