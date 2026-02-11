# PaginatedResponseCoach

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Data** | [**[]Coach**](Coach.md) |  | 
**HasMore** | **bool** | Whether there are more items after this page. | [readonly] 
**Limit** | **int32** |  | 
**Page** | **int32** | Current page number (1-indexed, for display purposes). | [readonly] 
**Pages** | **int32** | Total number of pages. | [readonly] 
**Skip** | **int32** |  | 
**Total** | **int32** |  | 

## Methods

### NewPaginatedResponseCoach

`func NewPaginatedResponseCoach(data []Coach, hasMore bool, limit int32, page int32, pages int32, skip int32, total int32, ) *PaginatedResponseCoach`

NewPaginatedResponseCoach instantiates a new PaginatedResponseCoach object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPaginatedResponseCoachWithDefaults

`func NewPaginatedResponseCoachWithDefaults() *PaginatedResponseCoach`

NewPaginatedResponseCoachWithDefaults instantiates a new PaginatedResponseCoach object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetData

`func (o *PaginatedResponseCoach) GetData() []Coach`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *PaginatedResponseCoach) GetDataOk() (*[]Coach, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *PaginatedResponseCoach) SetData(v []Coach)`

SetData sets Data field to given value.


### GetHasMore

`func (o *PaginatedResponseCoach) GetHasMore() bool`

GetHasMore returns the HasMore field if non-nil, zero value otherwise.

### GetHasMoreOk

`func (o *PaginatedResponseCoach) GetHasMoreOk() (*bool, bool)`

GetHasMoreOk returns a tuple with the HasMore field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHasMore

`func (o *PaginatedResponseCoach) SetHasMore(v bool)`

SetHasMore sets HasMore field to given value.


### GetLimit

`func (o *PaginatedResponseCoach) GetLimit() int32`

GetLimit returns the Limit field if non-nil, zero value otherwise.

### GetLimitOk

`func (o *PaginatedResponseCoach) GetLimitOk() (*int32, bool)`

GetLimitOk returns a tuple with the Limit field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLimit

`func (o *PaginatedResponseCoach) SetLimit(v int32)`

SetLimit sets Limit field to given value.


### GetPage

`func (o *PaginatedResponseCoach) GetPage() int32`

GetPage returns the Page field if non-nil, zero value otherwise.

### GetPageOk

`func (o *PaginatedResponseCoach) GetPageOk() (*int32, bool)`

GetPageOk returns a tuple with the Page field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPage

`func (o *PaginatedResponseCoach) SetPage(v int32)`

SetPage sets Page field to given value.


### GetPages

`func (o *PaginatedResponseCoach) GetPages() int32`

GetPages returns the Pages field if non-nil, zero value otherwise.

### GetPagesOk

`func (o *PaginatedResponseCoach) GetPagesOk() (*int32, bool)`

GetPagesOk returns a tuple with the Pages field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPages

`func (o *PaginatedResponseCoach) SetPages(v int32)`

SetPages sets Pages field to given value.


### GetSkip

`func (o *PaginatedResponseCoach) GetSkip() int32`

GetSkip returns the Skip field if non-nil, zero value otherwise.

### GetSkipOk

`func (o *PaginatedResponseCoach) GetSkipOk() (*int32, bool)`

GetSkipOk returns a tuple with the Skip field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSkip

`func (o *PaginatedResponseCoach) SetSkip(v int32)`

SetSkip sets Skip field to given value.


### GetTotal

`func (o *PaginatedResponseCoach) GetTotal() int32`

GetTotal returns the Total field if non-nil, zero value otherwise.

### GetTotalOk

`func (o *PaginatedResponseCoach) GetTotalOk() (*int32, bool)`

GetTotalOk returns a tuple with the Total field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotal

`func (o *PaginatedResponseCoach) SetTotal(v int32)`

SetTotal sets Total field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


