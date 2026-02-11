# MatchCompletedEvent

Webhook event sent when a match completes.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**created_at** | **datetime** | When the event was created | 
**data** | [**MatchCompletedData**](MatchCompletedData.md) |  | 
**event_id** | **UUID** | Unique identifier for this event | 
**event_type** | **str** | The type of webhook event | 

## Example

```python
from openapi_client.models.match_completed_event import MatchCompletedEvent

# TODO update the JSON string below
json = "{}"
# create an instance of MatchCompletedEvent from a JSON string
match_completed_event_instance = MatchCompletedEvent.from_json(json)
# print the JSON string representation of the object
print(MatchCompletedEvent.to_json())

# convert the object into a dict
match_completed_event_dict = match_completed_event_instance.to_dict()
# create an instance of MatchCompletedEvent from a dict
match_completed_event_from_dict = MatchCompletedEvent.from_dict(match_completed_event_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


