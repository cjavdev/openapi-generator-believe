# Org.OpenAPITools.Model.WebSocketLiveMatchEvent
A live match event with full details.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Commentary** | **string** | Match commentary for this event | 
**Description** | **string** | Human-readable event description | 
**EventId** | **int** | Unique event sequence number | 
**EventType** | **string** | Type of match event | 
**Minute** | **int** | Match minute | 
**Score** | [**WebSocketMatchScore**](WebSocketMatchScore.md) |  | 
**Stats** | [**WebSocketMatchStats**](WebSocketMatchStats.md) |  | 
**AddedTime** | **int** | Added/injury time minutes | [optional] 
**CrowdReaction** | **string** | Crowd reaction to the event | [optional] 
**Player** | [**WebSocketPlayerInfo**](WebSocketPlayerInfo.md) |  | [optional] 
**SecondaryPlayer** | [**WebSocketPlayerInfo**](WebSocketPlayerInfo.md) | Second player involved (e.g., assist, replaced player) | [optional] 
**Team** | **string** | Which team the event relates to | [optional] 
**TedReaction** | **string** | Ted Lasso&#39;s sideline reaction | [optional] 

[[Back to Model list]](../../README.md#documentation-for-models) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to README]](../../README.md)

