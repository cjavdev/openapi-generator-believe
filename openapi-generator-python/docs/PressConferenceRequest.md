# PressConferenceRequest

Request for press conference response.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**hostile** | **bool** | Is this a hostile question from Trent Crimm? | [optional] [default to False]
**question** | **str** | The press question to answer | 
**topic** | **str** |  | [optional] 

## Example

```python
from openapi_client.models.press_conference_request import PressConferenceRequest

# TODO update the JSON string below
json = "{}"
# create an instance of PressConferenceRequest from a JSON string
press_conference_request_instance = PressConferenceRequest.from_json(json)
# print the JSON string representation of the object
print(PressConferenceRequest.to_json())

# convert the object into a dict
press_conference_request_dict = press_conference_request_instance.to_dict()
# create an instance of PressConferenceRequest from a dict
press_conference_request_from_dict = PressConferenceRequest.from_dict(press_conference_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


