# Org.OpenAPITools.Model.RegisteredWebhook
A registered webhook endpoint.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**CreatedAt** | **DateTime** | When the webhook was registered | 
**EventTypes** | **List&lt;RegisteredWebhook.EventTypesEnum&gt;** | List of event types this webhook is subscribed to | 
**Id** | **string** | Unique webhook identifier | 
**Secret** | **string** | The secret key for verifying webhook signatures (base64 encoded) | 
**Url** | **string** | The URL to send webhook events to | 
**Description** | **string** |  | [optional] 

[[Back to Model list]](../../README.md#documentation-for-models) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to README]](../../README.md)

