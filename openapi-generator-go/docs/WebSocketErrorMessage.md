# WebSocketErrorMessage

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Code** | **string** | Error code | 
**Message** | **string** | Error description | 
**Type** | **string** | Message type | 

## Methods

### NewWebSocketErrorMessage

`func NewWebSocketErrorMessage(code string, message string, type_ string, ) *WebSocketErrorMessage`

NewWebSocketErrorMessage instantiates a new WebSocketErrorMessage object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewWebSocketErrorMessageWithDefaults

`func NewWebSocketErrorMessageWithDefaults() *WebSocketErrorMessage`

NewWebSocketErrorMessageWithDefaults instantiates a new WebSocketErrorMessage object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCode

`func (o *WebSocketErrorMessage) GetCode() string`

GetCode returns the Code field if non-nil, zero value otherwise.

### GetCodeOk

`func (o *WebSocketErrorMessage) GetCodeOk() (*string, bool)`

GetCodeOk returns a tuple with the Code field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCode

`func (o *WebSocketErrorMessage) SetCode(v string)`

SetCode sets Code field to given value.


### GetMessage

`func (o *WebSocketErrorMessage) GetMessage() string`

GetMessage returns the Message field if non-nil, zero value otherwise.

### GetMessageOk

`func (o *WebSocketErrorMessage) GetMessageOk() (*string, bool)`

GetMessageOk returns a tuple with the Message field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessage

`func (o *WebSocketErrorMessage) SetMessage(v string)`

SetMessage sets Message field to given value.


### GetType

`func (o *WebSocketErrorMessage) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *WebSocketErrorMessage) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *WebSocketErrorMessage) SetType(v string)`

SetType sets Type field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


