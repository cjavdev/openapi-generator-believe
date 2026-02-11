# PaginatedResponseQuote

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Data** | [**[]Quote**](Quote.md) |  | 
**HasMore** | **bool** | Whether there are more items after this page. | [readonly] 
**Limit** | **int32** |  | 
**Page** | **int32** | Current page number (1-indexed, for display purposes). | [readonly] 
**Pages** | **int32** | Total number of pages. | [readonly] 
**Skip** | **int32** |  | 
**Total** | **int32** |  | 

## Methods

### NewPaginatedResponseQuote

`func NewPaginatedResponseQuote(data []Quote, hasMore bool, limit int32, page int32, pages int32, skip int32, total int32, ) *PaginatedResponseQuote`

NewPaginatedResponseQuote instantiates a new PaginatedResponseQuote object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPaginatedResponseQuoteWithDefaults

`func NewPaginatedResponseQuoteWithDefaults() *PaginatedResponseQuote`

NewPaginatedResponseQuoteWithDefaults instantiates a new PaginatedResponseQuote object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetData

`func (o *PaginatedResponseQuote) GetData() []Quote`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *PaginatedResponseQuote) GetDataOk() (*[]Quote, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *PaginatedResponseQuote) SetData(v []Quote)`

SetData sets Data field to given value.


### GetHasMore

`func (o *PaginatedResponseQuote) GetHasMore() bool`

GetHasMore returns the HasMore field if non-nil, zero value otherwise.

### GetHasMoreOk

`func (o *PaginatedResponseQuote) GetHasMoreOk() (*bool, bool)`

GetHasMoreOk returns a tuple with the HasMore field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHasMore

`func (o *PaginatedResponseQuote) SetHasMore(v bool)`

SetHasMore sets HasMore field to given value.


### GetLimit

`func (o *PaginatedResponseQuote) GetLimit() int32`

GetLimit returns the Limit field if non-nil, zero value otherwise.

### GetLimitOk

`func (o *PaginatedResponseQuote) GetLimitOk() (*int32, bool)`

GetLimitOk returns a tuple with the Limit field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLimit

`func (o *PaginatedResponseQuote) SetLimit(v int32)`

SetLimit sets Limit field to given value.


### GetPage

`func (o *PaginatedResponseQuote) GetPage() int32`

GetPage returns the Page field if non-nil, zero value otherwise.

### GetPageOk

`func (o *PaginatedResponseQuote) GetPageOk() (*int32, bool)`

GetPageOk returns a tuple with the Page field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPage

`func (o *PaginatedResponseQuote) SetPage(v int32)`

SetPage sets Page field to given value.


### GetPages

`func (o *PaginatedResponseQuote) GetPages() int32`

GetPages returns the Pages field if non-nil, zero value otherwise.

### GetPagesOk

`func (o *PaginatedResponseQuote) GetPagesOk() (*int32, bool)`

GetPagesOk returns a tuple with the Pages field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPages

`func (o *PaginatedResponseQuote) SetPages(v int32)`

SetPages sets Pages field to given value.


### GetSkip

`func (o *PaginatedResponseQuote) GetSkip() int32`

GetSkip returns the Skip field if non-nil, zero value otherwise.

### GetSkipOk

`func (o *PaginatedResponseQuote) GetSkipOk() (*int32, bool)`

GetSkipOk returns a tuple with the Skip field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSkip

`func (o *PaginatedResponseQuote) SetSkip(v int32)`

SetSkip sets Skip field to given value.


### GetTotal

`func (o *PaginatedResponseQuote) GetTotal() int32`

GetTotal returns the Total field if non-nil, zero value otherwise.

### GetTotalOk

`func (o *PaginatedResponseQuote) GetTotalOk() (*int32, bool)`

GetTotalOk returns a tuple with the Total field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotal

`func (o *PaginatedResponseQuote) SetTotal(v int32)`

SetTotal sets Total field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


