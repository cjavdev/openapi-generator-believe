# RegisteredWebhook

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**CreatedAt** | **time.Time** | When the webhook was registered | 
**Description** | Pointer to **NullableString** |  | [optional] 
**EventTypes** | **[]string** | List of event types this webhook is subscribed to | 
**Id** | **string** | Unique webhook identifier | 
**Secret** | **string** | The secret key for verifying webhook signatures (base64 encoded) | 
**Url** | **string** | The URL to send webhook events to | 

## Methods

### NewRegisteredWebhook

`func NewRegisteredWebhook(createdAt time.Time, eventTypes []string, id string, secret string, url string, ) *RegisteredWebhook`

NewRegisteredWebhook instantiates a new RegisteredWebhook object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewRegisteredWebhookWithDefaults

`func NewRegisteredWebhookWithDefaults() *RegisteredWebhook`

NewRegisteredWebhookWithDefaults instantiates a new RegisteredWebhook object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCreatedAt

`func (o *RegisteredWebhook) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *RegisteredWebhook) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *RegisteredWebhook) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.


### GetDescription

`func (o *RegisteredWebhook) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *RegisteredWebhook) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *RegisteredWebhook) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *RegisteredWebhook) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### SetDescriptionNil

`func (o *RegisteredWebhook) SetDescriptionNil(b bool)`

 SetDescriptionNil sets the value for Description to be an explicit nil

### UnsetDescription
`func (o *RegisteredWebhook) UnsetDescription()`

UnsetDescription ensures that no value is present for Description, not even an explicit nil
### GetEventTypes

`func (o *RegisteredWebhook) GetEventTypes() []string`

GetEventTypes returns the EventTypes field if non-nil, zero value otherwise.

### GetEventTypesOk

`func (o *RegisteredWebhook) GetEventTypesOk() (*[]string, bool)`

GetEventTypesOk returns a tuple with the EventTypes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEventTypes

`func (o *RegisteredWebhook) SetEventTypes(v []string)`

SetEventTypes sets EventTypes field to given value.


### GetId

`func (o *RegisteredWebhook) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *RegisteredWebhook) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *RegisteredWebhook) SetId(v string)`

SetId sets Id field to given value.


### GetSecret

`func (o *RegisteredWebhook) GetSecret() string`

GetSecret returns the Secret field if non-nil, zero value otherwise.

### GetSecretOk

`func (o *RegisteredWebhook) GetSecretOk() (*string, bool)`

GetSecretOk returns a tuple with the Secret field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSecret

`func (o *RegisteredWebhook) SetSecret(v string)`

SetSecret sets Secret field to given value.


### GetUrl

`func (o *RegisteredWebhook) GetUrl() string`

GetUrl returns the Url field if non-nil, zero value otherwise.

### GetUrlOk

`func (o *RegisteredWebhook) GetUrlOk() (*string, bool)`

GetUrlOk returns a tuple with the Url field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUrl

`func (o *RegisteredWebhook) SetUrl(v string)`

SetUrl sets Url field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


