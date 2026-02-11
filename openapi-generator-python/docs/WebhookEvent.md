# WebhookEvent

Union type for all webhook events. Use the event_type field to determine the specific event type.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**created_at** | **datetime** | When the event was created | 
**data** | [**TeamMemberTransferredData**](TeamMemberTransferredData.md) |  | 
**event_id** | **UUID** | Unique identifier for this event | 
**event_type** | **str** | The type of webhook event | 

## Example

```python
from openapi_client.models.webhook_event import WebhookEvent

# TODO update the JSON string below
json = "{}"
# create an instance of WebhookEvent from a JSON string
webhook_event_instance = WebhookEvent.from_json(json)
# print the JSON string representation of the object
print(WebhookEvent.to_json())

# convert the object into a dict
webhook_event_dict = webhook_event_instance.to_dict()
# create an instance of WebhookEvent from a dict
webhook_event_from_dict = WebhookEvent.from_dict(webhook_event_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


