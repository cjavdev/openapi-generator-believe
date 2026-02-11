# MatchCompletedPayload

Payload for match.completed event.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**MatchCompletedData**](MatchCompletedData.md) | Event data | 
**event_type** | **str** | The type of webhook event | [optional] [default to 'match.completed']

## Example

```python
from openapi_client.models.match_completed_payload import MatchCompletedPayload

# TODO update the JSON string below
json = "{}"
# create an instance of MatchCompletedPayload from a JSON string
match_completed_payload_instance = MatchCompletedPayload.from_json(json)
# print the JSON string representation of the object
print(MatchCompletedPayload.to_json())

# convert the object into a dict
match_completed_payload_dict = match_completed_payload_instance.to_dict()
# create an instance of MatchCompletedPayload from a dict
match_completed_payload_from_dict = MatchCompletedPayload.from_dict(match_completed_payload_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


