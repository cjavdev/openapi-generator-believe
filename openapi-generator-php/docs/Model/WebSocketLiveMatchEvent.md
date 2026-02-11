# # WebSocketLiveMatchEvent

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**added_time** | **int** | Added/injury time minutes | [optional]
**commentary** | **string** | Match commentary for this event |
**crowd_reaction** | **string** | Crowd reaction to the event | [optional]
**description** | **string** | Human-readable event description |
**event_id** | **int** | Unique event sequence number |
**event_type** | **string** | Type of match event |
**minute** | **int** | Match minute |
**player** | [**\OpenAPI\Client\Model\WebSocketPlayerInfo**](WebSocketPlayerInfo.md) |  | [optional]
**score** | [**\OpenAPI\Client\Model\WebSocketMatchScore**](WebSocketMatchScore.md) |  |
**secondary_player** | [**\OpenAPI\Client\Model\WebSocketPlayerInfo**](WebSocketPlayerInfo.md) | Second player involved (e.g., assist, replaced player) | [optional]
**stats** | [**\OpenAPI\Client\Model\WebSocketMatchStats**](WebSocketMatchStats.md) |  |
**team** | **string** | Which team the event relates to | [optional]
**ted_reaction** | **string** | Ted Lasso&#39;s sideline reaction | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
