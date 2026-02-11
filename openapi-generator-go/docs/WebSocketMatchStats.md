# WebSocketMatchStats

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**CornersAway** | **int32** | Away team corners | 
**CornersHome** | **int32** | Home team corners | 
**FoulsAway** | **int32** | Away team fouls | 
**FoulsHome** | **int32** | Home team fouls | 
**PossessionAway** | **float32** | Away team possession % | 
**PossessionHome** | **float32** | Home team possession % | 
**RedCardsAway** | **int32** | Away team red cards | 
**RedCardsHome** | **int32** | Home team red cards | 
**ShotsAway** | **int32** | Away team total shots | 
**ShotsHome** | **int32** | Home team total shots | 
**ShotsOnTargetAway** | **int32** | Away team shots on target | 
**ShotsOnTargetHome** | **int32** | Home team shots on target | 
**YellowCardsAway** | **int32** | Away team yellow cards | 
**YellowCardsHome** | **int32** | Home team yellow cards | 

## Methods

### NewWebSocketMatchStats

`func NewWebSocketMatchStats(cornersAway int32, cornersHome int32, foulsAway int32, foulsHome int32, possessionAway float32, possessionHome float32, redCardsAway int32, redCardsHome int32, shotsAway int32, shotsHome int32, shotsOnTargetAway int32, shotsOnTargetHome int32, yellowCardsAway int32, yellowCardsHome int32, ) *WebSocketMatchStats`

NewWebSocketMatchStats instantiates a new WebSocketMatchStats object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewWebSocketMatchStatsWithDefaults

`func NewWebSocketMatchStatsWithDefaults() *WebSocketMatchStats`

NewWebSocketMatchStatsWithDefaults instantiates a new WebSocketMatchStats object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCornersAway

`func (o *WebSocketMatchStats) GetCornersAway() int32`

GetCornersAway returns the CornersAway field if non-nil, zero value otherwise.

### GetCornersAwayOk

`func (o *WebSocketMatchStats) GetCornersAwayOk() (*int32, bool)`

GetCornersAwayOk returns a tuple with the CornersAway field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCornersAway

`func (o *WebSocketMatchStats) SetCornersAway(v int32)`

SetCornersAway sets CornersAway field to given value.


### GetCornersHome

`func (o *WebSocketMatchStats) GetCornersHome() int32`

GetCornersHome returns the CornersHome field if non-nil, zero value otherwise.

### GetCornersHomeOk

`func (o *WebSocketMatchStats) GetCornersHomeOk() (*int32, bool)`

GetCornersHomeOk returns a tuple with the CornersHome field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCornersHome

`func (o *WebSocketMatchStats) SetCornersHome(v int32)`

SetCornersHome sets CornersHome field to given value.


### GetFoulsAway

`func (o *WebSocketMatchStats) GetFoulsAway() int32`

GetFoulsAway returns the FoulsAway field if non-nil, zero value otherwise.

### GetFoulsAwayOk

`func (o *WebSocketMatchStats) GetFoulsAwayOk() (*int32, bool)`

GetFoulsAwayOk returns a tuple with the FoulsAway field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFoulsAway

`func (o *WebSocketMatchStats) SetFoulsAway(v int32)`

SetFoulsAway sets FoulsAway field to given value.


### GetFoulsHome

`func (o *WebSocketMatchStats) GetFoulsHome() int32`

GetFoulsHome returns the FoulsHome field if non-nil, zero value otherwise.

### GetFoulsHomeOk

`func (o *WebSocketMatchStats) GetFoulsHomeOk() (*int32, bool)`

GetFoulsHomeOk returns a tuple with the FoulsHome field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFoulsHome

`func (o *WebSocketMatchStats) SetFoulsHome(v int32)`

SetFoulsHome sets FoulsHome field to given value.


### GetPossessionAway

`func (o *WebSocketMatchStats) GetPossessionAway() float32`

GetPossessionAway returns the PossessionAway field if non-nil, zero value otherwise.

### GetPossessionAwayOk

`func (o *WebSocketMatchStats) GetPossessionAwayOk() (*float32, bool)`

GetPossessionAwayOk returns a tuple with the PossessionAway field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPossessionAway

`func (o *WebSocketMatchStats) SetPossessionAway(v float32)`

SetPossessionAway sets PossessionAway field to given value.


### GetPossessionHome

`func (o *WebSocketMatchStats) GetPossessionHome() float32`

GetPossessionHome returns the PossessionHome field if non-nil, zero value otherwise.

### GetPossessionHomeOk

`func (o *WebSocketMatchStats) GetPossessionHomeOk() (*float32, bool)`

GetPossessionHomeOk returns a tuple with the PossessionHome field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPossessionHome

`func (o *WebSocketMatchStats) SetPossessionHome(v float32)`

SetPossessionHome sets PossessionHome field to given value.


### GetRedCardsAway

`func (o *WebSocketMatchStats) GetRedCardsAway() int32`

GetRedCardsAway returns the RedCardsAway field if non-nil, zero value otherwise.

### GetRedCardsAwayOk

`func (o *WebSocketMatchStats) GetRedCardsAwayOk() (*int32, bool)`

GetRedCardsAwayOk returns a tuple with the RedCardsAway field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRedCardsAway

`func (o *WebSocketMatchStats) SetRedCardsAway(v int32)`

SetRedCardsAway sets RedCardsAway field to given value.


### GetRedCardsHome

`func (o *WebSocketMatchStats) GetRedCardsHome() int32`

GetRedCardsHome returns the RedCardsHome field if non-nil, zero value otherwise.

### GetRedCardsHomeOk

`func (o *WebSocketMatchStats) GetRedCardsHomeOk() (*int32, bool)`

GetRedCardsHomeOk returns a tuple with the RedCardsHome field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRedCardsHome

`func (o *WebSocketMatchStats) SetRedCardsHome(v int32)`

SetRedCardsHome sets RedCardsHome field to given value.


### GetShotsAway

`func (o *WebSocketMatchStats) GetShotsAway() int32`

GetShotsAway returns the ShotsAway field if non-nil, zero value otherwise.

### GetShotsAwayOk

`func (o *WebSocketMatchStats) GetShotsAwayOk() (*int32, bool)`

GetShotsAwayOk returns a tuple with the ShotsAway field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShotsAway

`func (o *WebSocketMatchStats) SetShotsAway(v int32)`

SetShotsAway sets ShotsAway field to given value.


### GetShotsHome

`func (o *WebSocketMatchStats) GetShotsHome() int32`

GetShotsHome returns the ShotsHome field if non-nil, zero value otherwise.

### GetShotsHomeOk

`func (o *WebSocketMatchStats) GetShotsHomeOk() (*int32, bool)`

GetShotsHomeOk returns a tuple with the ShotsHome field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShotsHome

`func (o *WebSocketMatchStats) SetShotsHome(v int32)`

SetShotsHome sets ShotsHome field to given value.


### GetShotsOnTargetAway

`func (o *WebSocketMatchStats) GetShotsOnTargetAway() int32`

GetShotsOnTargetAway returns the ShotsOnTargetAway field if non-nil, zero value otherwise.

### GetShotsOnTargetAwayOk

`func (o *WebSocketMatchStats) GetShotsOnTargetAwayOk() (*int32, bool)`

GetShotsOnTargetAwayOk returns a tuple with the ShotsOnTargetAway field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShotsOnTargetAway

`func (o *WebSocketMatchStats) SetShotsOnTargetAway(v int32)`

SetShotsOnTargetAway sets ShotsOnTargetAway field to given value.


### GetShotsOnTargetHome

`func (o *WebSocketMatchStats) GetShotsOnTargetHome() int32`

GetShotsOnTargetHome returns the ShotsOnTargetHome field if non-nil, zero value otherwise.

### GetShotsOnTargetHomeOk

`func (o *WebSocketMatchStats) GetShotsOnTargetHomeOk() (*int32, bool)`

GetShotsOnTargetHomeOk returns a tuple with the ShotsOnTargetHome field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShotsOnTargetHome

`func (o *WebSocketMatchStats) SetShotsOnTargetHome(v int32)`

SetShotsOnTargetHome sets ShotsOnTargetHome field to given value.


### GetYellowCardsAway

`func (o *WebSocketMatchStats) GetYellowCardsAway() int32`

GetYellowCardsAway returns the YellowCardsAway field if non-nil, zero value otherwise.

### GetYellowCardsAwayOk

`func (o *WebSocketMatchStats) GetYellowCardsAwayOk() (*int32, bool)`

GetYellowCardsAwayOk returns a tuple with the YellowCardsAway field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetYellowCardsAway

`func (o *WebSocketMatchStats) SetYellowCardsAway(v int32)`

SetYellowCardsAway sets YellowCardsAway field to given value.


### GetYellowCardsHome

`func (o *WebSocketMatchStats) GetYellowCardsHome() int32`

GetYellowCardsHome returns the YellowCardsHome field if non-nil, zero value otherwise.

### GetYellowCardsHomeOk

`func (o *WebSocketMatchStats) GetYellowCardsHomeOk() (*int32, bool)`

GetYellowCardsHomeOk returns a tuple with the YellowCardsHome field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetYellowCardsHome

`func (o *WebSocketMatchStats) SetYellowCardsHome(v int32)`

SetYellowCardsHome sets YellowCardsHome field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


