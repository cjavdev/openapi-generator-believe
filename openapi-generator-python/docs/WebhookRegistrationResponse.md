# WebhookRegistrationResponse

Response after registering a webhook.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** | Status message | [optional] [default to 'Webhook registered successfully']
**ted_says** | **str** | Ted&#39;s reaction | [optional] [default to 'You know what? Staying connected is what it\'s all about. Welcome to the team!']
**webhook** | [**RegisteredWebhook**](RegisteredWebhook.md) | The registered webhook details | 

## Example

```python
from openapi_client.models.webhook_registration_response import WebhookRegistrationResponse

# TODO update the JSON string below
json = "{}"
# create an instance of WebhookRegistrationResponse from a JSON string
webhook_registration_response_instance = WebhookRegistrationResponse.from_json(json)
# print the JSON string representation of the object
print(WebhookRegistrationResponse.to_json())

# convert the object into a dict
webhook_registration_response_dict = webhook_registration_response_instance.to_dict()
# create an instance of WebhookRegistrationResponse from a dict
webhook_registration_response_from_dict = WebhookRegistrationResponse.from_dict(webhook_registration_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


