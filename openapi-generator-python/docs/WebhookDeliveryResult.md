# WebhookDeliveryResult

Result of delivering a webhook to a single endpoint.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**error** | **str** |  | [optional] 
**status_code** | **int** |  | [optional] 
**success** | **bool** | Whether delivery was successful | 
**url** | **str** | URL the webhook was sent to | 
**webhook_id** | **str** | ID of the webhook | 

## Example

```python
from openapi_client.models.webhook_delivery_result import WebhookDeliveryResult

# TODO update the JSON string below
json = "{}"
# create an instance of WebhookDeliveryResult from a JSON string
webhook_delivery_result_instance = WebhookDeliveryResult.from_json(json)
# print the JSON string representation of the object
print(WebhookDeliveryResult.to_json())

# convert the object into a dict
webhook_delivery_result_dict = webhook_delivery_result_instance.to_dict()
# create an instance of WebhookDeliveryResult from a dict
webhook_delivery_result_from_dict = WebhookDeliveryResult.from_dict(webhook_delivery_result_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


