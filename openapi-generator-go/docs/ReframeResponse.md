# ReframeResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**DailyAffirmation** | **string** | A daily affirmation to practice | 
**DrSharonInsight** | Pointer to **NullableString** |  | [optional] 
**OriginalThought** | **string** | The original negative thought | 
**ReframedThought** | **string** | The thought reframed positively | 
**TedPerspective** | **string** | Ted&#39;s take on this thought | 

## Methods

### NewReframeResponse

`func NewReframeResponse(dailyAffirmation string, originalThought string, reframedThought string, tedPerspective string, ) *ReframeResponse`

NewReframeResponse instantiates a new ReframeResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewReframeResponseWithDefaults

`func NewReframeResponseWithDefaults() *ReframeResponse`

NewReframeResponseWithDefaults instantiates a new ReframeResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetDailyAffirmation

`func (o *ReframeResponse) GetDailyAffirmation() string`

GetDailyAffirmation returns the DailyAffirmation field if non-nil, zero value otherwise.

### GetDailyAffirmationOk

`func (o *ReframeResponse) GetDailyAffirmationOk() (*string, bool)`

GetDailyAffirmationOk returns a tuple with the DailyAffirmation field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDailyAffirmation

`func (o *ReframeResponse) SetDailyAffirmation(v string)`

SetDailyAffirmation sets DailyAffirmation field to given value.


### GetDrSharonInsight

`func (o *ReframeResponse) GetDrSharonInsight() string`

GetDrSharonInsight returns the DrSharonInsight field if non-nil, zero value otherwise.

### GetDrSharonInsightOk

`func (o *ReframeResponse) GetDrSharonInsightOk() (*string, bool)`

GetDrSharonInsightOk returns a tuple with the DrSharonInsight field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDrSharonInsight

`func (o *ReframeResponse) SetDrSharonInsight(v string)`

SetDrSharonInsight sets DrSharonInsight field to given value.

### HasDrSharonInsight

`func (o *ReframeResponse) HasDrSharonInsight() bool`

HasDrSharonInsight returns a boolean if a field has been set.

### SetDrSharonInsightNil

`func (o *ReframeResponse) SetDrSharonInsightNil(b bool)`

 SetDrSharonInsightNil sets the value for DrSharonInsight to be an explicit nil

### UnsetDrSharonInsight
`func (o *ReframeResponse) UnsetDrSharonInsight()`

UnsetDrSharonInsight ensures that no value is present for DrSharonInsight, not even an explicit nil
### GetOriginalThought

`func (o *ReframeResponse) GetOriginalThought() string`

GetOriginalThought returns the OriginalThought field if non-nil, zero value otherwise.

### GetOriginalThoughtOk

`func (o *ReframeResponse) GetOriginalThoughtOk() (*string, bool)`

GetOriginalThoughtOk returns a tuple with the OriginalThought field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOriginalThought

`func (o *ReframeResponse) SetOriginalThought(v string)`

SetOriginalThought sets OriginalThought field to given value.


### GetReframedThought

`func (o *ReframeResponse) GetReframedThought() string`

GetReframedThought returns the ReframedThought field if non-nil, zero value otherwise.

### GetReframedThoughtOk

`func (o *ReframeResponse) GetReframedThoughtOk() (*string, bool)`

GetReframedThoughtOk returns a tuple with the ReframedThought field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReframedThought

`func (o *ReframeResponse) SetReframedThought(v string)`

SetReframedThought sets ReframedThought field to given value.


### GetTedPerspective

`func (o *ReframeResponse) GetTedPerspective() string`

GetTedPerspective returns the TedPerspective field if non-nil, zero value otherwise.

### GetTedPerspectiveOk

`func (o *ReframeResponse) GetTedPerspectiveOk() (*string, bool)`

GetTedPerspectiveOk returns a tuple with the TedPerspective field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTedPerspective

`func (o *ReframeResponse) SetTedPerspective(v string)`

SetTedPerspective sets TedPerspective field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


