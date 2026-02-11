# QuoteUpdate

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**CharacterId** | Pointer to **NullableString** |  | [optional] 
**Context** | Pointer to **NullableString** |  | [optional] 
**EpisodeId** | Pointer to **NullableString** |  | [optional] 
**IsFunny** | Pointer to **NullableBool** |  | [optional] 
**IsInspirational** | Pointer to **NullableBool** |  | [optional] 
**MomentType** | Pointer to [**NullableQuoteMoment**](QuoteMoment.md) |  | [optional] 
**PopularityScore** | Pointer to **NullableFloat32** |  | [optional] 
**SecondaryThemes** | Pointer to [**[]QuoteTheme**](QuoteTheme.md) |  | [optional] 
**Text** | Pointer to **NullableString** |  | [optional] 
**Theme** | Pointer to [**NullableQuoteTheme**](QuoteTheme.md) |  | [optional] 
**TimesShared** | Pointer to **NullableInt32** |  | [optional] 

## Methods

### NewQuoteUpdate

`func NewQuoteUpdate() *QuoteUpdate`

NewQuoteUpdate instantiates a new QuoteUpdate object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewQuoteUpdateWithDefaults

`func NewQuoteUpdateWithDefaults() *QuoteUpdate`

NewQuoteUpdateWithDefaults instantiates a new QuoteUpdate object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCharacterId

`func (o *QuoteUpdate) GetCharacterId() string`

GetCharacterId returns the CharacterId field if non-nil, zero value otherwise.

### GetCharacterIdOk

`func (o *QuoteUpdate) GetCharacterIdOk() (*string, bool)`

GetCharacterIdOk returns a tuple with the CharacterId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCharacterId

`func (o *QuoteUpdate) SetCharacterId(v string)`

SetCharacterId sets CharacterId field to given value.

### HasCharacterId

`func (o *QuoteUpdate) HasCharacterId() bool`

HasCharacterId returns a boolean if a field has been set.

### SetCharacterIdNil

`func (o *QuoteUpdate) SetCharacterIdNil(b bool)`

 SetCharacterIdNil sets the value for CharacterId to be an explicit nil

### UnsetCharacterId
`func (o *QuoteUpdate) UnsetCharacterId()`

UnsetCharacterId ensures that no value is present for CharacterId, not even an explicit nil
### GetContext

`func (o *QuoteUpdate) GetContext() string`

GetContext returns the Context field if non-nil, zero value otherwise.

### GetContextOk

`func (o *QuoteUpdate) GetContextOk() (*string, bool)`

GetContextOk returns a tuple with the Context field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetContext

`func (o *QuoteUpdate) SetContext(v string)`

SetContext sets Context field to given value.

### HasContext

`func (o *QuoteUpdate) HasContext() bool`

HasContext returns a boolean if a field has been set.

### SetContextNil

`func (o *QuoteUpdate) SetContextNil(b bool)`

 SetContextNil sets the value for Context to be an explicit nil

### UnsetContext
`func (o *QuoteUpdate) UnsetContext()`

UnsetContext ensures that no value is present for Context, not even an explicit nil
### GetEpisodeId

`func (o *QuoteUpdate) GetEpisodeId() string`

GetEpisodeId returns the EpisodeId field if non-nil, zero value otherwise.

### GetEpisodeIdOk

`func (o *QuoteUpdate) GetEpisodeIdOk() (*string, bool)`

GetEpisodeIdOk returns a tuple with the EpisodeId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEpisodeId

`func (o *QuoteUpdate) SetEpisodeId(v string)`

SetEpisodeId sets EpisodeId field to given value.

### HasEpisodeId

`func (o *QuoteUpdate) HasEpisodeId() bool`

HasEpisodeId returns a boolean if a field has been set.

### SetEpisodeIdNil

`func (o *QuoteUpdate) SetEpisodeIdNil(b bool)`

 SetEpisodeIdNil sets the value for EpisodeId to be an explicit nil

### UnsetEpisodeId
`func (o *QuoteUpdate) UnsetEpisodeId()`

UnsetEpisodeId ensures that no value is present for EpisodeId, not even an explicit nil
### GetIsFunny

`func (o *QuoteUpdate) GetIsFunny() bool`

GetIsFunny returns the IsFunny field if non-nil, zero value otherwise.

### GetIsFunnyOk

`func (o *QuoteUpdate) GetIsFunnyOk() (*bool, bool)`

GetIsFunnyOk returns a tuple with the IsFunny field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsFunny

`func (o *QuoteUpdate) SetIsFunny(v bool)`

SetIsFunny sets IsFunny field to given value.

### HasIsFunny

`func (o *QuoteUpdate) HasIsFunny() bool`

HasIsFunny returns a boolean if a field has been set.

### SetIsFunnyNil

`func (o *QuoteUpdate) SetIsFunnyNil(b bool)`

 SetIsFunnyNil sets the value for IsFunny to be an explicit nil

### UnsetIsFunny
`func (o *QuoteUpdate) UnsetIsFunny()`

UnsetIsFunny ensures that no value is present for IsFunny, not even an explicit nil
### GetIsInspirational

`func (o *QuoteUpdate) GetIsInspirational() bool`

GetIsInspirational returns the IsInspirational field if non-nil, zero value otherwise.

### GetIsInspirationalOk

`func (o *QuoteUpdate) GetIsInspirationalOk() (*bool, bool)`

GetIsInspirationalOk returns a tuple with the IsInspirational field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsInspirational

`func (o *QuoteUpdate) SetIsInspirational(v bool)`

SetIsInspirational sets IsInspirational field to given value.

### HasIsInspirational

`func (o *QuoteUpdate) HasIsInspirational() bool`

HasIsInspirational returns a boolean if a field has been set.

### SetIsInspirationalNil

`func (o *QuoteUpdate) SetIsInspirationalNil(b bool)`

 SetIsInspirationalNil sets the value for IsInspirational to be an explicit nil

### UnsetIsInspirational
`func (o *QuoteUpdate) UnsetIsInspirational()`

UnsetIsInspirational ensures that no value is present for IsInspirational, not even an explicit nil
### GetMomentType

`func (o *QuoteUpdate) GetMomentType() QuoteMoment`

GetMomentType returns the MomentType field if non-nil, zero value otherwise.

### GetMomentTypeOk

`func (o *QuoteUpdate) GetMomentTypeOk() (*QuoteMoment, bool)`

GetMomentTypeOk returns a tuple with the MomentType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMomentType

`func (o *QuoteUpdate) SetMomentType(v QuoteMoment)`

SetMomentType sets MomentType field to given value.

### HasMomentType

`func (o *QuoteUpdate) HasMomentType() bool`

HasMomentType returns a boolean if a field has been set.

### SetMomentTypeNil

`func (o *QuoteUpdate) SetMomentTypeNil(b bool)`

 SetMomentTypeNil sets the value for MomentType to be an explicit nil

### UnsetMomentType
`func (o *QuoteUpdate) UnsetMomentType()`

UnsetMomentType ensures that no value is present for MomentType, not even an explicit nil
### GetPopularityScore

`func (o *QuoteUpdate) GetPopularityScore() float32`

GetPopularityScore returns the PopularityScore field if non-nil, zero value otherwise.

### GetPopularityScoreOk

`func (o *QuoteUpdate) GetPopularityScoreOk() (*float32, bool)`

GetPopularityScoreOk returns a tuple with the PopularityScore field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPopularityScore

`func (o *QuoteUpdate) SetPopularityScore(v float32)`

SetPopularityScore sets PopularityScore field to given value.

### HasPopularityScore

`func (o *QuoteUpdate) HasPopularityScore() bool`

HasPopularityScore returns a boolean if a field has been set.

### SetPopularityScoreNil

`func (o *QuoteUpdate) SetPopularityScoreNil(b bool)`

 SetPopularityScoreNil sets the value for PopularityScore to be an explicit nil

### UnsetPopularityScore
`func (o *QuoteUpdate) UnsetPopularityScore()`

UnsetPopularityScore ensures that no value is present for PopularityScore, not even an explicit nil
### GetSecondaryThemes

`func (o *QuoteUpdate) GetSecondaryThemes() []QuoteTheme`

GetSecondaryThemes returns the SecondaryThemes field if non-nil, zero value otherwise.

### GetSecondaryThemesOk

`func (o *QuoteUpdate) GetSecondaryThemesOk() (*[]QuoteTheme, bool)`

GetSecondaryThemesOk returns a tuple with the SecondaryThemes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSecondaryThemes

`func (o *QuoteUpdate) SetSecondaryThemes(v []QuoteTheme)`

SetSecondaryThemes sets SecondaryThemes field to given value.

### HasSecondaryThemes

`func (o *QuoteUpdate) HasSecondaryThemes() bool`

HasSecondaryThemes returns a boolean if a field has been set.

### SetSecondaryThemesNil

`func (o *QuoteUpdate) SetSecondaryThemesNil(b bool)`

 SetSecondaryThemesNil sets the value for SecondaryThemes to be an explicit nil

### UnsetSecondaryThemes
`func (o *QuoteUpdate) UnsetSecondaryThemes()`

UnsetSecondaryThemes ensures that no value is present for SecondaryThemes, not even an explicit nil
### GetText

`func (o *QuoteUpdate) GetText() string`

GetText returns the Text field if non-nil, zero value otherwise.

### GetTextOk

`func (o *QuoteUpdate) GetTextOk() (*string, bool)`

GetTextOk returns a tuple with the Text field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetText

`func (o *QuoteUpdate) SetText(v string)`

SetText sets Text field to given value.

### HasText

`func (o *QuoteUpdate) HasText() bool`

HasText returns a boolean if a field has been set.

### SetTextNil

`func (o *QuoteUpdate) SetTextNil(b bool)`

 SetTextNil sets the value for Text to be an explicit nil

### UnsetText
`func (o *QuoteUpdate) UnsetText()`

UnsetText ensures that no value is present for Text, not even an explicit nil
### GetTheme

`func (o *QuoteUpdate) GetTheme() QuoteTheme`

GetTheme returns the Theme field if non-nil, zero value otherwise.

### GetThemeOk

`func (o *QuoteUpdate) GetThemeOk() (*QuoteTheme, bool)`

GetThemeOk returns a tuple with the Theme field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTheme

`func (o *QuoteUpdate) SetTheme(v QuoteTheme)`

SetTheme sets Theme field to given value.

### HasTheme

`func (o *QuoteUpdate) HasTheme() bool`

HasTheme returns a boolean if a field has been set.

### SetThemeNil

`func (o *QuoteUpdate) SetThemeNil(b bool)`

 SetThemeNil sets the value for Theme to be an explicit nil

### UnsetTheme
`func (o *QuoteUpdate) UnsetTheme()`

UnsetTheme ensures that no value is present for Theme, not even an explicit nil
### GetTimesShared

`func (o *QuoteUpdate) GetTimesShared() int32`

GetTimesShared returns the TimesShared field if non-nil, zero value otherwise.

### GetTimesSharedOk

`func (o *QuoteUpdate) GetTimesSharedOk() (*int32, bool)`

GetTimesSharedOk returns a tuple with the TimesShared field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTimesShared

`func (o *QuoteUpdate) SetTimesShared(v int32)`

SetTimesShared sets TimesShared field to given value.

### HasTimesShared

`func (o *QuoteUpdate) HasTimesShared() bool`

HasTimesShared returns a boolean if a field has been set.

### SetTimesSharedNil

`func (o *QuoteUpdate) SetTimesSharedNil(b bool)`

 SetTimesSharedNil sets the value for TimesShared to be an explicit nil

### UnsetTimesShared
`func (o *QuoteUpdate) UnsetTimesShared()`

UnsetTimesShared ensures that no value is present for TimesShared, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


