# EpisodeCreate

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AirDate** | **string** | Original air date | 
**BiscuitsWithBossMoment** | Pointer to **NullableString** |  | [optional] 
**CharacterFocus** | **[]string** | Characters with significant development | 
**Director** | **string** | Episode director | 
**EpisodeNumber** | **int32** | Episode number within season | 
**MainTheme** | **string** | Central theme of the episode | 
**MemorableMoments** | Pointer to **[]string** | Standout moments from the episode | [optional] 
**RuntimeMinutes** | **int32** | Episode runtime in minutes | 
**Season** | **int32** | Season number | 
**Synopsis** | **string** | Brief plot synopsis | 
**TedWisdom** | **string** | Key piece of Ted wisdom from the episode | 
**Title** | **string** | Episode title | 
**UsViewersMillions** | Pointer to **NullableFloat32** |  | [optional] 
**ViewerRating** | Pointer to **NullableFloat32** |  | [optional] 
**Writer** | **string** | Episode writer(s) | 

## Methods

### NewEpisodeCreate

`func NewEpisodeCreate(airDate string, characterFocus []string, director string, episodeNumber int32, mainTheme string, runtimeMinutes int32, season int32, synopsis string, tedWisdom string, title string, writer string, ) *EpisodeCreate`

NewEpisodeCreate instantiates a new EpisodeCreate object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewEpisodeCreateWithDefaults

`func NewEpisodeCreateWithDefaults() *EpisodeCreate`

NewEpisodeCreateWithDefaults instantiates a new EpisodeCreate object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAirDate

`func (o *EpisodeCreate) GetAirDate() string`

GetAirDate returns the AirDate field if non-nil, zero value otherwise.

### GetAirDateOk

`func (o *EpisodeCreate) GetAirDateOk() (*string, bool)`

GetAirDateOk returns a tuple with the AirDate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAirDate

`func (o *EpisodeCreate) SetAirDate(v string)`

SetAirDate sets AirDate field to given value.


### GetBiscuitsWithBossMoment

`func (o *EpisodeCreate) GetBiscuitsWithBossMoment() string`

GetBiscuitsWithBossMoment returns the BiscuitsWithBossMoment field if non-nil, zero value otherwise.

### GetBiscuitsWithBossMomentOk

`func (o *EpisodeCreate) GetBiscuitsWithBossMomentOk() (*string, bool)`

GetBiscuitsWithBossMomentOk returns a tuple with the BiscuitsWithBossMoment field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBiscuitsWithBossMoment

`func (o *EpisodeCreate) SetBiscuitsWithBossMoment(v string)`

SetBiscuitsWithBossMoment sets BiscuitsWithBossMoment field to given value.

### HasBiscuitsWithBossMoment

`func (o *EpisodeCreate) HasBiscuitsWithBossMoment() bool`

HasBiscuitsWithBossMoment returns a boolean if a field has been set.

### SetBiscuitsWithBossMomentNil

`func (o *EpisodeCreate) SetBiscuitsWithBossMomentNil(b bool)`

 SetBiscuitsWithBossMomentNil sets the value for BiscuitsWithBossMoment to be an explicit nil

### UnsetBiscuitsWithBossMoment
`func (o *EpisodeCreate) UnsetBiscuitsWithBossMoment()`

UnsetBiscuitsWithBossMoment ensures that no value is present for BiscuitsWithBossMoment, not even an explicit nil
### GetCharacterFocus

`func (o *EpisodeCreate) GetCharacterFocus() []string`

GetCharacterFocus returns the CharacterFocus field if non-nil, zero value otherwise.

### GetCharacterFocusOk

`func (o *EpisodeCreate) GetCharacterFocusOk() (*[]string, bool)`

GetCharacterFocusOk returns a tuple with the CharacterFocus field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCharacterFocus

`func (o *EpisodeCreate) SetCharacterFocus(v []string)`

SetCharacterFocus sets CharacterFocus field to given value.


### GetDirector

`func (o *EpisodeCreate) GetDirector() string`

GetDirector returns the Director field if non-nil, zero value otherwise.

### GetDirectorOk

`func (o *EpisodeCreate) GetDirectorOk() (*string, bool)`

GetDirectorOk returns a tuple with the Director field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDirector

`func (o *EpisodeCreate) SetDirector(v string)`

SetDirector sets Director field to given value.


### GetEpisodeNumber

`func (o *EpisodeCreate) GetEpisodeNumber() int32`

GetEpisodeNumber returns the EpisodeNumber field if non-nil, zero value otherwise.

### GetEpisodeNumberOk

`func (o *EpisodeCreate) GetEpisodeNumberOk() (*int32, bool)`

GetEpisodeNumberOk returns a tuple with the EpisodeNumber field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEpisodeNumber

`func (o *EpisodeCreate) SetEpisodeNumber(v int32)`

SetEpisodeNumber sets EpisodeNumber field to given value.


### GetMainTheme

`func (o *EpisodeCreate) GetMainTheme() string`

GetMainTheme returns the MainTheme field if non-nil, zero value otherwise.

### GetMainThemeOk

`func (o *EpisodeCreate) GetMainThemeOk() (*string, bool)`

GetMainThemeOk returns a tuple with the MainTheme field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMainTheme

`func (o *EpisodeCreate) SetMainTheme(v string)`

SetMainTheme sets MainTheme field to given value.


### GetMemorableMoments

`func (o *EpisodeCreate) GetMemorableMoments() []string`

GetMemorableMoments returns the MemorableMoments field if non-nil, zero value otherwise.

### GetMemorableMomentsOk

`func (o *EpisodeCreate) GetMemorableMomentsOk() (*[]string, bool)`

GetMemorableMomentsOk returns a tuple with the MemorableMoments field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMemorableMoments

`func (o *EpisodeCreate) SetMemorableMoments(v []string)`

SetMemorableMoments sets MemorableMoments field to given value.

### HasMemorableMoments

`func (o *EpisodeCreate) HasMemorableMoments() bool`

HasMemorableMoments returns a boolean if a field has been set.

### GetRuntimeMinutes

`func (o *EpisodeCreate) GetRuntimeMinutes() int32`

GetRuntimeMinutes returns the RuntimeMinutes field if non-nil, zero value otherwise.

### GetRuntimeMinutesOk

`func (o *EpisodeCreate) GetRuntimeMinutesOk() (*int32, bool)`

GetRuntimeMinutesOk returns a tuple with the RuntimeMinutes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRuntimeMinutes

`func (o *EpisodeCreate) SetRuntimeMinutes(v int32)`

SetRuntimeMinutes sets RuntimeMinutes field to given value.


### GetSeason

`func (o *EpisodeCreate) GetSeason() int32`

GetSeason returns the Season field if non-nil, zero value otherwise.

### GetSeasonOk

`func (o *EpisodeCreate) GetSeasonOk() (*int32, bool)`

GetSeasonOk returns a tuple with the Season field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSeason

`func (o *EpisodeCreate) SetSeason(v int32)`

SetSeason sets Season field to given value.


### GetSynopsis

`func (o *EpisodeCreate) GetSynopsis() string`

GetSynopsis returns the Synopsis field if non-nil, zero value otherwise.

### GetSynopsisOk

`func (o *EpisodeCreate) GetSynopsisOk() (*string, bool)`

GetSynopsisOk returns a tuple with the Synopsis field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSynopsis

`func (o *EpisodeCreate) SetSynopsis(v string)`

SetSynopsis sets Synopsis field to given value.


### GetTedWisdom

`func (o *EpisodeCreate) GetTedWisdom() string`

GetTedWisdom returns the TedWisdom field if non-nil, zero value otherwise.

### GetTedWisdomOk

`func (o *EpisodeCreate) GetTedWisdomOk() (*string, bool)`

GetTedWisdomOk returns a tuple with the TedWisdom field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTedWisdom

`func (o *EpisodeCreate) SetTedWisdom(v string)`

SetTedWisdom sets TedWisdom field to given value.


### GetTitle

`func (o *EpisodeCreate) GetTitle() string`

GetTitle returns the Title field if non-nil, zero value otherwise.

### GetTitleOk

`func (o *EpisodeCreate) GetTitleOk() (*string, bool)`

GetTitleOk returns a tuple with the Title field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTitle

`func (o *EpisodeCreate) SetTitle(v string)`

SetTitle sets Title field to given value.


### GetUsViewersMillions

`func (o *EpisodeCreate) GetUsViewersMillions() float32`

GetUsViewersMillions returns the UsViewersMillions field if non-nil, zero value otherwise.

### GetUsViewersMillionsOk

`func (o *EpisodeCreate) GetUsViewersMillionsOk() (*float32, bool)`

GetUsViewersMillionsOk returns a tuple with the UsViewersMillions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUsViewersMillions

`func (o *EpisodeCreate) SetUsViewersMillions(v float32)`

SetUsViewersMillions sets UsViewersMillions field to given value.

### HasUsViewersMillions

`func (o *EpisodeCreate) HasUsViewersMillions() bool`

HasUsViewersMillions returns a boolean if a field has been set.

### SetUsViewersMillionsNil

`func (o *EpisodeCreate) SetUsViewersMillionsNil(b bool)`

 SetUsViewersMillionsNil sets the value for UsViewersMillions to be an explicit nil

### UnsetUsViewersMillions
`func (o *EpisodeCreate) UnsetUsViewersMillions()`

UnsetUsViewersMillions ensures that no value is present for UsViewersMillions, not even an explicit nil
### GetViewerRating

`func (o *EpisodeCreate) GetViewerRating() float32`

GetViewerRating returns the ViewerRating field if non-nil, zero value otherwise.

### GetViewerRatingOk

`func (o *EpisodeCreate) GetViewerRatingOk() (*float32, bool)`

GetViewerRatingOk returns a tuple with the ViewerRating field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetViewerRating

`func (o *EpisodeCreate) SetViewerRating(v float32)`

SetViewerRating sets ViewerRating field to given value.

### HasViewerRating

`func (o *EpisodeCreate) HasViewerRating() bool`

HasViewerRating returns a boolean if a field has been set.

### SetViewerRatingNil

`func (o *EpisodeCreate) SetViewerRatingNil(b bool)`

 SetViewerRatingNil sets the value for ViewerRating to be an explicit nil

### UnsetViewerRating
`func (o *EpisodeCreate) UnsetViewerRating()`

UnsetViewerRating ensures that no value is present for ViewerRating, not even an explicit nil
### GetWriter

`func (o *EpisodeCreate) GetWriter() string`

GetWriter returns the Writer field if non-nil, zero value otherwise.

### GetWriterOk

`func (o *EpisodeCreate) GetWriterOk() (*string, bool)`

GetWriterOk returns a tuple with the Writer field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWriter

`func (o *EpisodeCreate) SetWriter(v string)`

SetWriter sets Writer field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


