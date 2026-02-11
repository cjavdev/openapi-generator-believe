# # RegisteredWebhook

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**created_at** | **\DateTime** | When the webhook was registered |
**description** | **string** |  | [optional]
**event_types** | **string[]** | List of event types this webhook is subscribed to |
**id** | **string** | Unique webhook identifier |
**secret** | **string** | The secret key for verifying webhook signatures (base64 encoded) |
**url** | **string** | The URL to send webhook events to |

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
