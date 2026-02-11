# WebhookDeliveryResult

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Error** | Pointer to **NullableString** |  | [optional] 
**StatusCode** | Pointer to **NullableInt32** |  | [optional] 
**Success** | **bool** | Whether delivery was successful | 
**Url** | **string** | URL the webhook was sent to | 
**WebhookId** | **string** | ID of the webhook | 

## Methods

### NewWebhookDeliveryResult

`func NewWebhookDeliveryResult(success bool, url string, webhookId string, ) *WebhookDeliveryResult`

NewWebhookDeliveryResult instantiates a new WebhookDeliveryResult object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewWebhookDeliveryResultWithDefaults

`func NewWebhookDeliveryResultWithDefaults() *WebhookDeliveryResult`

NewWebhookDeliveryResultWithDefaults instantiates a new WebhookDeliveryResult object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetError

`func (o *WebhookDeliveryResult) GetError() string`

GetError returns the Error field if non-nil, zero value otherwise.

### GetErrorOk

`func (o *WebhookDeliveryResult) GetErrorOk() (*string, bool)`

GetErrorOk returns a tuple with the Error field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetError

`func (o *WebhookDeliveryResult) SetError(v string)`

SetError sets Error field to given value.

### HasError

`func (o *WebhookDeliveryResult) HasError() bool`

HasError returns a boolean if a field has been set.

### SetErrorNil

`func (o *WebhookDeliveryResult) SetErrorNil(b bool)`

 SetErrorNil sets the value for Error to be an explicit nil

### UnsetError
`func (o *WebhookDeliveryResult) UnsetError()`

UnsetError ensures that no value is present for Error, not even an explicit nil
### GetStatusCode

`func (o *WebhookDeliveryResult) GetStatusCode() int32`

GetStatusCode returns the StatusCode field if non-nil, zero value otherwise.

### GetStatusCodeOk

`func (o *WebhookDeliveryResult) GetStatusCodeOk() (*int32, bool)`

GetStatusCodeOk returns a tuple with the StatusCode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatusCode

`func (o *WebhookDeliveryResult) SetStatusCode(v int32)`

SetStatusCode sets StatusCode field to given value.

### HasStatusCode

`func (o *WebhookDeliveryResult) HasStatusCode() bool`

HasStatusCode returns a boolean if a field has been set.

### SetStatusCodeNil

`func (o *WebhookDeliveryResult) SetStatusCodeNil(b bool)`

 SetStatusCodeNil sets the value for StatusCode to be an explicit nil

### UnsetStatusCode
`func (o *WebhookDeliveryResult) UnsetStatusCode()`

UnsetStatusCode ensures that no value is present for StatusCode, not even an explicit nil
### GetSuccess

`func (o *WebhookDeliveryResult) GetSuccess() bool`

GetSuccess returns the Success field if non-nil, zero value otherwise.

### GetSuccessOk

`func (o *WebhookDeliveryResult) GetSuccessOk() (*bool, bool)`

GetSuccessOk returns a tuple with the Success field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSuccess

`func (o *WebhookDeliveryResult) SetSuccess(v bool)`

SetSuccess sets Success field to given value.


### GetUrl

`func (o *WebhookDeliveryResult) GetUrl() string`

GetUrl returns the Url field if non-nil, zero value otherwise.

### GetUrlOk

`func (o *WebhookDeliveryResult) GetUrlOk() (*string, bool)`

GetUrlOk returns a tuple with the Url field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUrl

`func (o *WebhookDeliveryResult) SetUrl(v string)`

SetUrl sets Url field to given value.


### GetWebhookId

`func (o *WebhookDeliveryResult) GetWebhookId() string`

GetWebhookId returns the WebhookId field if non-nil, zero value otherwise.

### GetWebhookIdOk

`func (o *WebhookDeliveryResult) GetWebhookIdOk() (*string, bool)`

GetWebhookIdOk returns a tuple with the WebhookId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWebhookId

`func (o *WebhookDeliveryResult) SetWebhookId(v string)`

SetWebhookId sets WebhookId field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


