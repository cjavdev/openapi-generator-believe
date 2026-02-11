# PressConferenceResponse

Ted's press conference response.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**actual_wisdom** | **str** | The actual wisdom beneath the humor | 
**deflection_humor** | **str** |  | [optional] 
**follow_up_dodge** | **str** | How Ted would dodge a follow-up | 
**reporter_reaction** | **str** | How reporters would react | 
**response** | **str** | Ted&#39;s press conference answer | 

## Example

```python
from openapi_client.models.press_conference_response import PressConferenceResponse

# TODO update the JSON string below
json = "{}"
# create an instance of PressConferenceResponse from a JSON string
press_conference_response_instance = PressConferenceResponse.from_json(json)
# print the JSON string representation of the object
print(PressConferenceResponse.to_json())

# convert the object into a dict
press_conference_response_dict = press_conference_response_instance.to_dict()
# create an instance of PressConferenceResponse from a dict
press_conference_response_from_dict = PressConferenceResponse.from_dict(press_conference_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


