# PaginatedResponsePlayer

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Data** | [**[]Player**](Player.md) |  | 
**HasMore** | **bool** | Whether there are more items after this page. | [readonly] 
**Limit** | **int32** |  | 
**Page** | **int32** | Current page number (1-indexed, for display purposes). | [readonly] 
**Pages** | **int32** | Total number of pages. | [readonly] 
**Skip** | **int32** |  | 
**Total** | **int32** |  | 

## Methods

### NewPaginatedResponsePlayer

`func NewPaginatedResponsePlayer(data []Player, hasMore bool, limit int32, page int32, pages int32, skip int32, total int32, ) *PaginatedResponsePlayer`

NewPaginatedResponsePlayer instantiates a new PaginatedResponsePlayer object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPaginatedResponsePlayerWithDefaults

`func NewPaginatedResponsePlayerWithDefaults() *PaginatedResponsePlayer`

NewPaginatedResponsePlayerWithDefaults instantiates a new PaginatedResponsePlayer object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetData

`func (o *PaginatedResponsePlayer) GetData() []Player`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *PaginatedResponsePlayer) GetDataOk() (*[]Player, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *PaginatedResponsePlayer) SetData(v []Player)`

SetData sets Data field to given value.


### GetHasMore

`func (o *PaginatedResponsePlayer) GetHasMore() bool`

GetHasMore returns the HasMore field if non-nil, zero value otherwise.

### GetHasMoreOk

`func (o *PaginatedResponsePlayer) GetHasMoreOk() (*bool, bool)`

GetHasMoreOk returns a tuple with the HasMore field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHasMore

`func (o *PaginatedResponsePlayer) SetHasMore(v bool)`

SetHasMore sets HasMore field to given value.


### GetLimit

`func (o *PaginatedResponsePlayer) GetLimit() int32`

GetLimit returns the Limit field if non-nil, zero value otherwise.

### GetLimitOk

`func (o *PaginatedResponsePlayer) GetLimitOk() (*int32, bool)`

GetLimitOk returns a tuple with the Limit field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLimit

`func (o *PaginatedResponsePlayer) SetLimit(v int32)`

SetLimit sets Limit field to given value.


### GetPage

`func (o *PaginatedResponsePlayer) GetPage() int32`

GetPage returns the Page field if non-nil, zero value otherwise.

### GetPageOk

`func (o *PaginatedResponsePlayer) GetPageOk() (*int32, bool)`

GetPageOk returns a tuple with the Page field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPage

`func (o *PaginatedResponsePlayer) SetPage(v int32)`

SetPage sets Page field to given value.


### GetPages

`func (o *PaginatedResponsePlayer) GetPages() int32`

GetPages returns the Pages field if non-nil, zero value otherwise.

### GetPagesOk

`func (o *PaginatedResponsePlayer) GetPagesOk() (*int32, bool)`

GetPagesOk returns a tuple with the Pages field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPages

`func (o *PaginatedResponsePlayer) SetPages(v int32)`

SetPages sets Pages field to given value.


### GetSkip

`func (o *PaginatedResponsePlayer) GetSkip() int32`

GetSkip returns the Skip field if non-nil, zero value otherwise.

### GetSkipOk

`func (o *PaginatedResponsePlayer) GetSkipOk() (*int32, bool)`

GetSkipOk returns a tuple with the Skip field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSkip

`func (o *PaginatedResponsePlayer) SetSkip(v int32)`

SetSkip sets Skip field to given value.


### GetTotal

`func (o *PaginatedResponsePlayer) GetTotal() int32`

GetTotal returns the Total field if non-nil, zero value otherwise.

### GetTotalOk

`func (o *PaginatedResponsePlayer) GetTotalOk() (*int32, bool)`

GetTotalOk returns a tuple with the Total field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotal

`func (o *PaginatedResponsePlayer) SetTotal(v int32)`

SetTotal sets Total field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


