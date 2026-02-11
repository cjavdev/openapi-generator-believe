# BelieveResponse

Response from the Believe Engine.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**action_suggestion** | **str** | Suggested action to take | 
**believe_score** | **int** | Your current believe-o-meter score | 
**goldfish_wisdom** | **str** | A reminder to have a goldfish memory when needed | 
**relevant_quote** | **str** | A relevant Ted Lasso quote | 
**ted_response** | **str** | Ted&#39;s motivational response | 

## Example

```python
from openapi_client.models.believe_response import BelieveResponse

# TODO update the JSON string below
json = "{}"
# create an instance of BelieveResponse from a JSON string
believe_response_instance = BelieveResponse.from_json(json)
# print the JSON string representation of the object
print(BelieveResponse.to_json())

# convert the object into a dict
believe_response_dict = believe_response_instance.to_dict()
# create an instance of BelieveResponse from a dict
believe_response_from_dict = BelieveResponse.from_dict(believe_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


