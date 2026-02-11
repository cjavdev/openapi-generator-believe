# ReframeRequest

Request to reframe a negative thought.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**negative_thought** | **str** | The negative thought to reframe | 
**recurring** | **bool** | Is this a recurring thought? | [optional] [default to False]

## Example

```python
from openapi_client.models.reframe_request import ReframeRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ReframeRequest from a JSON string
reframe_request_instance = ReframeRequest.from_json(json)
# print the JSON string representation of the object
print(ReframeRequest.to_json())

# convert the object into a dict
reframe_request_dict = reframe_request_instance.to_dict()
# create an instance of ReframeRequest from a dict
reframe_request_from_dict = ReframeRequest.from_dict(reframe_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


