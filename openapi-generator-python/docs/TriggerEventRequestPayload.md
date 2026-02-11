# TriggerEventRequestPayload


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**TeamMemberTransferredData**](TeamMemberTransferredData.md) | Event data | 
**event_type** | **str** | The type of webhook event | [optional] [default to 'team_member.transferred']

## Example

```python
from openapi_client.models.trigger_event_request_payload import TriggerEventRequestPayload

# TODO update the JSON string below
json = "{}"
# create an instance of TriggerEventRequestPayload from a JSON string
trigger_event_request_payload_instance = TriggerEventRequestPayload.from_json(json)
# print the JSON string representation of the object
print(TriggerEventRequestPayload.to_json())

# convert the object into a dict
trigger_event_request_payload_dict = trigger_event_request_payload_instance.to_dict()
# create an instance of TriggerEventRequestPayload from a dict
trigger_event_request_payload_from_dict = TriggerEventRequestPayload.from_dict(trigger_event_request_payload_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


