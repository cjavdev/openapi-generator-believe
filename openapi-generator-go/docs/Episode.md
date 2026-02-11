# Episode

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AirDate** | **string** | Original air date | 
**BiscuitsWithBossMoment** | Pointer to **NullableString** |  | [optional] 
**CharacterFocus** | **[]string** | Characters with significant development | 
**Director** | **string** | Episode director | 
**EpisodeNumber** | **int32** | Episode number within season | 
**Id** | **string** | Unique identifier (format: s##e##) | 
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

### NewEpisode

`func NewEpisode(airDate string, characterFocus []string, director string, episodeNumber int32, id string, mainTheme string, runtimeMinutes int32, season int32, synopsis string, tedWisdom string, title string, writer string, ) *Episode`

NewEpisode instantiates a new Episode object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewEpisodeWithDefaults

`func NewEpisodeWithDefaults() *Episode`

NewEpisodeWithDefaults instantiates a new Episode object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAirDate

`func (o *Episode) GetAirDate() string`

GetAirDate returns the AirDate field if non-nil, zero value otherwise.

### GetAirDateOk

`func (o *Episode) GetAirDateOk() (*string, bool)`

GetAirDateOk returns a tuple with the AirDate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAirDate

`func (o *Episode) SetAirDate(v string)`

SetAirDate sets AirDate field to given value.


### GetBiscuitsWithBossMoment

`func (o *Episode) GetBiscuitsWithBossMoment() string`

GetBiscuitsWithBossMoment returns the BiscuitsWithBossMoment field if non-nil, zero value otherwise.

### GetBiscuitsWithBossMomentOk

`func (o *Episode) GetBiscuitsWithBossMomentOk() (*string, bool)`

GetBiscuitsWithBossMomentOk returns a tuple with the BiscuitsWithBossMoment field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBiscuitsWithBossMoment

`func (o *Episode) SetBiscuitsWithBossMoment(v string)`

SetBiscuitsWithBossMoment sets BiscuitsWithBossMoment field to given value.

### HasBiscuitsWithBossMoment

`func (o *Episode) HasBiscuitsWithBossMoment() bool`

HasBiscuitsWithBossMoment returns a boolean if a field has been set.

### SetBiscuitsWithBossMomentNil

`func (o *Episode) SetBiscuitsWithBossMomentNil(b bool)`

 SetBiscuitsWithBossMomentNil sets the value for BiscuitsWithBossMoment to be an explicit nil

### UnsetBiscuitsWithBossMoment
`func (o *Episode) UnsetBiscuitsWithBossMoment()`

UnsetBiscuitsWithBossMoment ensures that no value is present for BiscuitsWithBossMoment, not even an explicit nil
### GetCharacterFocus

`func (o *Episode) GetCharacterFocus() []string`

GetCharacterFocus returns the CharacterFocus field if non-nil, zero value otherwise.

### GetCharacterFocusOk

`func (o *Episode) GetCharacterFocusOk() (*[]string, bool)`

GetCharacterFocusOk returns a tuple with the CharacterFocus field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCharacterFocus

`func (o *Episode) SetCharacterFocus(v []string)`

SetCharacterFocus sets CharacterFocus field to given value.


### GetDirector

`func (o *Episode) GetDirector() string`

GetDirector returns the Director field if non-nil, zero value otherwise.

### GetDirectorOk

`func (o *Episode) GetDirectorOk() (*string, bool)`

GetDirectorOk returns a tuple with the Director field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDirector

`func (o *Episode) SetDirector(v string)`

SetDirector sets Director field to given value.


### GetEpisodeNumber

`func (o *Episode) GetEpisodeNumber() int32`

GetEpisodeNumber returns the EpisodeNumber field if non-nil, zero value otherwise.

### GetEpisodeNumberOk

`func (o *Episode) GetEpisodeNumberOk() (*int32, bool)`

GetEpisodeNumberOk returns a tuple with the EpisodeNumber field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEpisodeNumber

`func (o *Episode) SetEpisodeNumber(v int32)`

SetEpisodeNumber sets EpisodeNumber field to given value.


### GetId

`func (o *Episode) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *Episode) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *Episode) SetId(v string)`

SetId sets Id field to given value.


### GetMainTheme

`func (o *Episode) GetMainTheme() string`

GetMainTheme returns the MainTheme field if non-nil, zero value otherwise.

### GetMainThemeOk

`func (o *Episode) GetMainThemeOk() (*string, bool)`

GetMainThemeOk returns a tuple with the MainTheme field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMainTheme

`func (o *Episode) SetMainTheme(v string)`

SetMainTheme sets MainTheme field to given value.


### GetMemorableMoments

`func (o *Episode) GetMemorableMoments() []string`

GetMemorableMoments returns the MemorableMoments field if non-nil, zero value otherwise.

### GetMemorableMomentsOk

`func (o *Episode) GetMemorableMomentsOk() (*[]string, bool)`

GetMemorableMomentsOk returns a tuple with the MemorableMoments field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMemorableMoments

`func (o *Episode) SetMemorableMoments(v []string)`

SetMemorableMoments sets MemorableMoments field to given value.

### HasMemorableMoments

`func (o *Episode) HasMemorableMoments() bool`

HasMemorableMoments returns a boolean if a field has been set.

### GetRuntimeMinutes

`func (o *Episode) GetRuntimeMinutes() int32`

GetRuntimeMinutes returns the RuntimeMinutes field if non-nil, zero value otherwise.

### GetRuntimeMinutesOk

`func (o *Episode) GetRuntimeMinutesOk() (*int32, bool)`

GetRuntimeMinutesOk returns a tuple with the RuntimeMinutes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRuntimeMinutes

`func (o *Episode) SetRuntimeMinutes(v int32)`

SetRuntimeMinutes sets RuntimeMinutes field to given value.


### GetSeason

`func (o *Episode) GetSeason() int32`

GetSeason returns the Season field if non-nil, zero value otherwise.

### GetSeasonOk

`func (o *Episode) GetSeasonOk() (*int32, bool)`

GetSeasonOk returns a tuple with the Season field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSeason

`func (o *Episode) SetSeason(v int32)`

SetSeason sets Season field to given value.


### GetSynopsis

`func (o *Episode) GetSynopsis() string`

GetSynopsis returns the Synopsis field if non-nil, zero value otherwise.

### GetSynopsisOk

`func (o *Episode) GetSynopsisOk() (*string, bool)`

GetSynopsisOk returns a tuple with the Synopsis field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSynopsis

`func (o *Episode) SetSynopsis(v string)`

SetSynopsis sets Synopsis field to given value.


### GetTedWisdom

`func (o *Episode) GetTedWisdom() string`

GetTedWisdom returns the TedWisdom field if non-nil, zero value otherwise.

### GetTedWisdomOk

`func (o *Episode) GetTedWisdomOk() (*string, bool)`

GetTedWisdomOk returns a tuple with the TedWisdom field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTedWisdom

`func (o *Episode) SetTedWisdom(v string)`

SetTedWisdom sets TedWisdom field to given value.


### GetTitle

`func (o *Episode) GetTitle() string`

GetTitle returns the Title field if non-nil, zero value otherwise.

### GetTitleOk

`func (o *Episode) GetTitleOk() (*string, bool)`

GetTitleOk returns a tuple with the Title field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTitle

`func (o *Episode) SetTitle(v string)`

SetTitle sets Title field to given value.


### GetUsViewersMillions

`func (o *Episode) GetUsViewersMillions() float32`

GetUsViewersMillions returns the UsViewersMillions field if non-nil, zero value otherwise.

### GetUsViewersMillionsOk

`func (o *Episode) GetUsViewersMillionsOk() (*float32, bool)`

GetUsViewersMillionsOk returns a tuple with the UsViewersMillions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUsViewersMillions

`func (o *Episode) SetUsViewersMillions(v float32)`

SetUsViewersMillions sets UsViewersMillions field to given value.

### HasUsViewersMillions

`func (o *Episode) HasUsViewersMillions() bool`

HasUsViewersMillions returns a boolean if a field has been set.

### SetUsViewersMillionsNil

`func (o *Episode) SetUsViewersMillionsNil(b bool)`

 SetUsViewersMillionsNil sets the value for UsViewersMillions to be an explicit nil

### UnsetUsViewersMillions
`func (o *Episode) UnsetUsViewersMillions()`

UnsetUsViewersMillions ensures that no value is present for UsViewersMillions, not even an explicit nil
### GetViewerRating

`func (o *Episode) GetViewerRating() float32`

GetViewerRating returns the ViewerRating field if non-nil, zero value otherwise.

### GetViewerRatingOk

`func (o *Episode) GetViewerRatingOk() (*float32, bool)`

GetViewerRatingOk returns a tuple with the ViewerRating field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetViewerRating

`func (o *Episode) SetViewerRating(v float32)`

SetViewerRating sets ViewerRating field to given value.

### HasViewerRating

`func (o *Episode) HasViewerRating() bool`

HasViewerRating returns a boolean if a field has been set.

### SetViewerRatingNil

`func (o *Episode) SetViewerRatingNil(b bool)`

 SetViewerRatingNil sets the value for ViewerRating to be an explicit nil

### UnsetViewerRating
`func (o *Episode) UnsetViewerRating()`

UnsetViewerRating ensures that no value is present for ViewerRating, not even an explicit nil
### GetWriter

`func (o *Episode) GetWriter() string`

GetWriter returns the Writer field if non-nil, zero value otherwise.

### GetWriterOk

`func (o *Episode) GetWriterOk() (*string, bool)`

GetWriterOk returns a tuple with the Writer field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWriter

`func (o *Episode) SetWriter(v string)`

SetWriter sets Writer field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


