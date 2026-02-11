# ReframeResponse

Reframed perspective response.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**daily_affirmation** | **str** | A daily affirmation to practice | 
**dr_sharon_insight** | **str** |  | [optional] 
**original_thought** | **str** | The original negative thought | 
**reframed_thought** | **str** | The thought reframed positively | 
**ted_perspective** | **str** | Ted&#39;s take on this thought | 

## Example

```python
from openapi_client.models.reframe_response import ReframeResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ReframeResponse from a JSON string
reframe_response_instance = ReframeResponse.from_json(json)
# print the JSON string representation of the object
print(ReframeResponse.to_json())

# convert the object into a dict
reframe_response_dict = reframe_response_instance.to_dict()
# create an instance of ReframeResponse from a dict
reframe_response_from_dict = ReframeResponse.from_dict(reframe_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


