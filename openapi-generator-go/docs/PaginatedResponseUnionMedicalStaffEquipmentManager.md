# PaginatedResponseUnionMedicalStaffEquipmentManager

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Data** | [**[]DataInner1**](DataInner1.md) |  | 
**HasMore** | **bool** | Whether there are more items after this page. | [readonly] 
**Limit** | **int32** |  | 
**Page** | **int32** | Current page number (1-indexed, for display purposes). | [readonly] 
**Pages** | **int32** | Total number of pages. | [readonly] 
**Skip** | **int32** |  | 
**Total** | **int32** |  | 

## Methods

### NewPaginatedResponseUnionMedicalStaffEquipmentManager

`func NewPaginatedResponseUnionMedicalStaffEquipmentManager(data []DataInner1, hasMore bool, limit int32, page int32, pages int32, skip int32, total int32, ) *PaginatedResponseUnionMedicalStaffEquipmentManager`

NewPaginatedResponseUnionMedicalStaffEquipmentManager instantiates a new PaginatedResponseUnionMedicalStaffEquipmentManager object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPaginatedResponseUnionMedicalStaffEquipmentManagerWithDefaults

`func NewPaginatedResponseUnionMedicalStaffEquipmentManagerWithDefaults() *PaginatedResponseUnionMedicalStaffEquipmentManager`

NewPaginatedResponseUnionMedicalStaffEquipmentManagerWithDefaults instantiates a new PaginatedResponseUnionMedicalStaffEquipmentManager object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetData

`func (o *PaginatedResponseUnionMedicalStaffEquipmentManager) GetData() []DataInner1`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *PaginatedResponseUnionMedicalStaffEquipmentManager) GetDataOk() (*[]DataInner1, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *PaginatedResponseUnionMedicalStaffEquipmentManager) SetData(v []DataInner1)`

SetData sets Data field to given value.


### GetHasMore

`func (o *PaginatedResponseUnionMedicalStaffEquipmentManager) GetHasMore() bool`

GetHasMore returns the HasMore field if non-nil, zero value otherwise.

### GetHasMoreOk

`func (o *PaginatedResponseUnionMedicalStaffEquipmentManager) GetHasMoreOk() (*bool, bool)`

GetHasMoreOk returns a tuple with the HasMore field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHasMore

`func (o *PaginatedResponseUnionMedicalStaffEquipmentManager) SetHasMore(v bool)`

SetHasMore sets HasMore field to given value.


### GetLimit

`func (o *PaginatedResponseUnionMedicalStaffEquipmentManager) GetLimit() int32`

GetLimit returns the Limit field if non-nil, zero value otherwise.

### GetLimitOk

`func (o *PaginatedResponseUnionMedicalStaffEquipmentManager) GetLimitOk() (*int32, bool)`

GetLimitOk returns a tuple with the Limit field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLimit

`func (o *PaginatedResponseUnionMedicalStaffEquipmentManager) SetLimit(v int32)`

SetLimit sets Limit field to given value.


### GetPage

`func (o *PaginatedResponseUnionMedicalStaffEquipmentManager) GetPage() int32`

GetPage returns the Page field if non-nil, zero value otherwise.

### GetPageOk

`func (o *PaginatedResponseUnionMedicalStaffEquipmentManager) GetPageOk() (*int32, bool)`

GetPageOk returns a tuple with the Page field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPage

`func (o *PaginatedResponseUnionMedicalStaffEquipmentManager) SetPage(v int32)`

SetPage sets Page field to given value.


### GetPages

`func (o *PaginatedResponseUnionMedicalStaffEquipmentManager) GetPages() int32`

GetPages returns the Pages field if non-nil, zero value otherwise.

### GetPagesOk

`func (o *PaginatedResponseUnionMedicalStaffEquipmentManager) GetPagesOk() (*int32, bool)`

GetPagesOk returns a tuple with the Pages field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPages

`func (o *PaginatedResponseUnionMedicalStaffEquipmentManager) SetPages(v int32)`

SetPages sets Pages field to given value.


### GetSkip

`func (o *PaginatedResponseUnionMedicalStaffEquipmentManager) GetSkip() int32`

GetSkip returns the Skip field if non-nil, zero value otherwise.

### GetSkipOk

`func (o *PaginatedResponseUnionMedicalStaffEquipmentManager) GetSkipOk() (*int32, bool)`

GetSkipOk returns a tuple with the Skip field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSkip

`func (o *PaginatedResponseUnionMedicalStaffEquipmentManager) SetSkip(v int32)`

SetSkip sets Skip field to given value.


### GetTotal

`func (o *PaginatedResponseUnionMedicalStaffEquipmentManager) GetTotal() int32`

GetTotal returns the Total field if non-nil, zero value otherwise.

### GetTotalOk

`func (o *PaginatedResponseUnionMedicalStaffEquipmentManager) GetTotalOk() (*int32, bool)`

GetTotalOk returns a tuple with the Total field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotal

`func (o *PaginatedResponseUnionMedicalStaffEquipmentManager) SetTotal(v int32)`

SetTotal sets Total field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


