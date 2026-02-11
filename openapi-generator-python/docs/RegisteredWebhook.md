# RegisteredWebhook

A registered webhook endpoint.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**created_at** | **datetime** | When the webhook was registered | 
**description** | **str** |  | [optional] 
**event_types** | **List[str]** | List of event types this webhook is subscribed to | 
**id** | **str** | Unique webhook identifier | 
**secret** | **str** | The secret key for verifying webhook signatures (base64 encoded) | 
**url** | **str** | The URL to send webhook events to | 

## Example

```python
from openapi_client.models.registered_webhook import RegisteredWebhook

# TODO update the JSON string below
json = "{}"
# create an instance of RegisteredWebhook from a JSON string
registered_webhook_instance = RegisteredWebhook.from_json(json)
# print the JSON string representation of the object
print(RegisteredWebhook.to_json())

# convert the object into a dict
registered_webhook_dict = registered_webhook_instance.to_dict()
# create an instance of RegisteredWebhook from a dict
registered_webhook_from_dict = RegisteredWebhook.from_dict(registered_webhook_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


