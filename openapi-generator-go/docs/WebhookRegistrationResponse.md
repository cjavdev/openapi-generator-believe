# WebhookRegistrationResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Message** | Pointer to **string** | Status message | [optional] [default to "Webhook registered successfully"]
**TedSays** | Pointer to **string** | Ted&#39;s reaction | [optional] [default to "You know what? Staying connected is what it's all about. Welcome to the team!"]
**Webhook** | [**RegisteredWebhook**](RegisteredWebhook.md) | The registered webhook details | 

## Methods

### NewWebhookRegistrationResponse

`func NewWebhookRegistrationResponse(webhook RegisteredWebhook, ) *WebhookRegistrationResponse`

NewWebhookRegistrationResponse instantiates a new WebhookRegistrationResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewWebhookRegistrationResponseWithDefaults

`func NewWebhookRegistrationResponseWithDefaults() *WebhookRegistrationResponse`

NewWebhookRegistrationResponseWithDefaults instantiates a new WebhookRegistrationResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetMessage

`func (o *WebhookRegistrationResponse) GetMessage() string`

GetMessage returns the Message field if non-nil, zero value otherwise.

### GetMessageOk

`func (o *WebhookRegistrationResponse) GetMessageOk() (*string, bool)`

GetMessageOk returns a tuple with the Message field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessage

`func (o *WebhookRegistrationResponse) SetMessage(v string)`

SetMessage sets Message field to given value.

### HasMessage

`func (o *WebhookRegistrationResponse) HasMessage() bool`

HasMessage returns a boolean if a field has been set.

### GetTedSays

`func (o *WebhookRegistrationResponse) GetTedSays() string`

GetTedSays returns the TedSays field if non-nil, zero value otherwise.

### GetTedSaysOk

`func (o *WebhookRegistrationResponse) GetTedSaysOk() (*string, bool)`

GetTedSaysOk returns a tuple with the TedSays field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTedSays

`func (o *WebhookRegistrationResponse) SetTedSays(v string)`

SetTedSays sets TedSays field to given value.

### HasTedSays

`func (o *WebhookRegistrationResponse) HasTedSays() bool`

HasTedSays returns a boolean if a field has been set.

### GetWebhook

`func (o *WebhookRegistrationResponse) GetWebhook() RegisteredWebhook`

GetWebhook returns the Webhook field if non-nil, zero value otherwise.

### GetWebhookOk

`func (o *WebhookRegistrationResponse) GetWebhookOk() (*RegisteredWebhook, bool)`

GetWebhookOk returns a tuple with the Webhook field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWebhook

`func (o *WebhookRegistrationResponse) SetWebhook(v RegisteredWebhook)`

SetWebhook sets Webhook field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


