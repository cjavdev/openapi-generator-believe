# Quote

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**CharacterId** | **string** | ID of the character who said it | 
**Context** | **string** | Context in which the quote was said | 
**EpisodeId** | Pointer to **NullableString** |  | [optional] 
**Id** | **string** | Unique identifier | 
**IsFunny** | Pointer to **bool** | Whether this quote is humorous | [optional] [default to false]
**IsInspirational** | Pointer to **bool** | Whether this quote is inspirational | [optional] [default to true]
**MomentType** | [**QuoteMoment**](QuoteMoment.md) | Type of moment when the quote was said | 
**PopularityScore** | Pointer to **NullableFloat32** |  | [optional] 
**SecondaryThemes** | Pointer to [**[]QuoteTheme**](QuoteTheme.md) | Additional themes | [optional] 
**Text** | **string** | The quote text | 
**Theme** | [**QuoteTheme**](QuoteTheme.md) | Primary theme of the quote | 
**TimesShared** | Pointer to **NullableInt32** |  | [optional] 

## Methods

### NewQuote

`func NewQuote(characterId string, context string, id string, momentType QuoteMoment, text string, theme QuoteTheme, ) *Quote`

NewQuote instantiates a new Quote object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewQuoteWithDefaults

`func NewQuoteWithDefaults() *Quote`

NewQuoteWithDefaults instantiates a new Quote object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCharacterId

`func (o *Quote) GetCharacterId() string`

GetCharacterId returns the CharacterId field if non-nil, zero value otherwise.

### GetCharacterIdOk

`func (o *Quote) GetCharacterIdOk() (*string, bool)`

GetCharacterIdOk returns a tuple with the CharacterId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCharacterId

`func (o *Quote) SetCharacterId(v string)`

SetCharacterId sets CharacterId field to given value.


### GetContext

`func (o *Quote) GetContext() string`

GetContext returns the Context field if non-nil, zero value otherwise.

### GetContextOk

`func (o *Quote) GetContextOk() (*string, bool)`

GetContextOk returns a tuple with the Context field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetContext

`func (o *Quote) SetContext(v string)`

SetContext sets Context field to given value.


### GetEpisodeId

`func (o *Quote) GetEpisodeId() string`

GetEpisodeId returns the EpisodeId field if non-nil, zero value otherwise.

### GetEpisodeIdOk

`func (o *Quote) GetEpisodeIdOk() (*string, bool)`

GetEpisodeIdOk returns a tuple with the EpisodeId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEpisodeId

`func (o *Quote) SetEpisodeId(v string)`

SetEpisodeId sets EpisodeId field to given value.

### HasEpisodeId

`func (o *Quote) HasEpisodeId() bool`

HasEpisodeId returns a boolean if a field has been set.

### SetEpisodeIdNil

`func (o *Quote) SetEpisodeIdNil(b bool)`

 SetEpisodeIdNil sets the value for EpisodeId to be an explicit nil

### UnsetEpisodeId
`func (o *Quote) UnsetEpisodeId()`

UnsetEpisodeId ensures that no value is present for EpisodeId, not even an explicit nil
### GetId

`func (o *Quote) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *Quote) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *Quote) SetId(v string)`

SetId sets Id field to given value.


### GetIsFunny

`func (o *Quote) GetIsFunny() bool`

GetIsFunny returns the IsFunny field if non-nil, zero value otherwise.

### GetIsFunnyOk

`func (o *Quote) GetIsFunnyOk() (*bool, bool)`

GetIsFunnyOk returns a tuple with the IsFunny field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsFunny

`func (o *Quote) SetIsFunny(v bool)`

SetIsFunny sets IsFunny field to given value.

### HasIsFunny

`func (o *Quote) HasIsFunny() bool`

HasIsFunny returns a boolean if a field has been set.

### GetIsInspirational

`func (o *Quote) GetIsInspirational() bool`

GetIsInspirational returns the IsInspirational field if non-nil, zero value otherwise.

### GetIsInspirationalOk

`func (o *Quote) GetIsInspirationalOk() (*bool, bool)`

GetIsInspirationalOk returns a tuple with the IsInspirational field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsInspirational

`func (o *Quote) SetIsInspirational(v bool)`

SetIsInspirational sets IsInspirational field to given value.

### HasIsInspirational

`func (o *Quote) HasIsInspirational() bool`

HasIsInspirational returns a boolean if a field has been set.

### GetMomentType

`func (o *Quote) GetMomentType() QuoteMoment`

GetMomentType returns the MomentType field if non-nil, zero value otherwise.

### GetMomentTypeOk

`func (o *Quote) GetMomentTypeOk() (*QuoteMoment, bool)`

GetMomentTypeOk returns a tuple with the MomentType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMomentType

`func (o *Quote) SetMomentType(v QuoteMoment)`

SetMomentType sets MomentType field to given value.


### GetPopularityScore

`func (o *Quote) GetPopularityScore() float32`

GetPopularityScore returns the PopularityScore field if non-nil, zero value otherwise.

### GetPopularityScoreOk

`func (o *Quote) GetPopularityScoreOk() (*float32, bool)`

GetPopularityScoreOk returns a tuple with the PopularityScore field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPopularityScore

`func (o *Quote) SetPopularityScore(v float32)`

SetPopularityScore sets PopularityScore field to given value.

### HasPopularityScore

`func (o *Quote) HasPopularityScore() bool`

HasPopularityScore returns a boolean if a field has been set.

### SetPopularityScoreNil

`func (o *Quote) SetPopularityScoreNil(b bool)`

 SetPopularityScoreNil sets the value for PopularityScore to be an explicit nil

### UnsetPopularityScore
`func (o *Quote) UnsetPopularityScore()`

UnsetPopularityScore ensures that no value is present for PopularityScore, not even an explicit nil
### GetSecondaryThemes

`func (o *Quote) GetSecondaryThemes() []QuoteTheme`

GetSecondaryThemes returns the SecondaryThemes field if non-nil, zero value otherwise.

### GetSecondaryThemesOk

`func (o *Quote) GetSecondaryThemesOk() (*[]QuoteTheme, bool)`

GetSecondaryThemesOk returns a tuple with the SecondaryThemes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSecondaryThemes

`func (o *Quote) SetSecondaryThemes(v []QuoteTheme)`

SetSecondaryThemes sets SecondaryThemes field to given value.

### HasSecondaryThemes

`func (o *Quote) HasSecondaryThemes() bool`

HasSecondaryThemes returns a boolean if a field has been set.

### GetText

`func (o *Quote) GetText() string`

GetText returns the Text field if non-nil, zero value otherwise.

### GetTextOk

`func (o *Quote) GetTextOk() (*string, bool)`

GetTextOk returns a tuple with the Text field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetText

`func (o *Quote) SetText(v string)`

SetText sets Text field to given value.


### GetTheme

`func (o *Quote) GetTheme() QuoteTheme`

GetTheme returns the Theme field if non-nil, zero value otherwise.

### GetThemeOk

`func (o *Quote) GetThemeOk() (*QuoteTheme, bool)`

GetThemeOk returns a tuple with the Theme field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTheme

`func (o *Quote) SetTheme(v QuoteTheme)`

SetTheme sets Theme field to given value.


### GetTimesShared

`func (o *Quote) GetTimesShared() int32`

GetTimesShared returns the TimesShared field if non-nil, zero value otherwise.

### GetTimesSharedOk

`func (o *Quote) GetTimesSharedOk() (*int32, bool)`

GetTimesSharedOk returns a tuple with the TimesShared field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTimesShared

`func (o *Quote) SetTimesShared(v int32)`

SetTimesShared sets TimesShared field to given value.

### HasTimesShared

`func (o *Quote) HasTimesShared() bool`

HasTimesShared returns a boolean if a field has been set.

### SetTimesSharedNil

`func (o *Quote) SetTimesSharedNil(b bool)`

 SetTimesSharedNil sets the value for TimesShared to be an explicit nil

### UnsetTimesShared
`func (o *Quote) UnsetTimesShared()`

UnsetTimesShared ensures that no value is present for TimesShared, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


