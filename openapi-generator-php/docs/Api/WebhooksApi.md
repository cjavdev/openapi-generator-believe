# OpenAPI\Client\WebhooksApi

Register webhook endpoints and trigger events for testing

All URIs are relative to https://believe.cjav.dev, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**matchCompletedWebhook()**](WebhooksApi.md#matchCompletedWebhook) | **POST** /matchCompleted | Match Completed |
| [**teamMemberTransferredWebhook()**](WebhooksApi.md#teamMemberTransferredWebhook) | **POST** /teamMemberTransferred | Team Member Transferred |


## `matchCompletedWebhook()`

```php
matchCompletedWebhook($match_completed_event)
```

Match Completed

Fired when a football match completes. Contains final score, result, and Ted's post-match wisdom.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new OpenAPI\Client\Api\WebhooksApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$match_completed_event = {"created_at":"2024-01-15T17:00:00Z","data":{"away_score":1,"away_team_id":"manchester-city","completed_at":"2024-01-15T16:52:00Z","home_score":2,"home_team_id":"afc-richmond","lesson_learned":"Believing in each other is more powerful than any tactics board.","man_of_the_match":"Jamie Tartt","match_id":"match-001","match_type":"league","result":"home_win","ted_post_match_quote":"Win or lose, we did it together. And that's what makes us a team, not just a group of people wearing the same color shirts."},"event_id":"evt_abc123def456","event_type":"match.completed"}; // \OpenAPI\Client\Model\MatchCompletedEvent | Match completed event payload

try {
    $apiInstance->matchCompletedWebhook($match_completed_event);
} catch (Exception $e) {
    echo 'Exception when calling WebhooksApi->matchCompletedWebhook: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **match_completed_event** | [**\OpenAPI\Client\Model\MatchCompletedEvent**](../Model/MatchCompletedEvent.md)| Match completed event payload | |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `teamMemberTransferredWebhook()`

```php
teamMemberTransferredWebhook($team_member_transferred_event)
```

Team Member Transferred

Fired when a player, coach, or staff member joins or departs from a team. Transfer news is big in football!

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new OpenAPI\Client\Api\WebhooksApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$team_member_transferred_event = {"created_at":"2024-01-10T09:00:00Z","data":{"character_id":"jamie-tartt","character_name":"Jamie Tartt","member_type":"player","previous_team_id":"manchester-city","previous_team_name":"Manchester City","team_id":"afc-richmond","team_member_id":"jamie-tartt-richmond","team_name":"AFC Richmond","ted_reaction":"You know what? Sometimes people need to go away to realize where they belong. Welcome home, Jamie.","transfer_fee_gbp":"15000000.00","transfer_type":"joined","years_with_previous_team":2},"event_id":"evt_xyz789ghi012","event_type":"team_member.transferred"}; // \OpenAPI\Client\Model\TeamMemberTransferredEvent | Team member transfer event payload

try {
    $apiInstance->teamMemberTransferredWebhook($team_member_transferred_event);
} catch (Exception $e) {
    echo 'Exception when calling WebhooksApi->teamMemberTransferredWebhook: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **team_member_transferred_event** | [**\OpenAPI\Client\Model\TeamMemberTransferredEvent**](../Model/TeamMemberTransferredEvent.md)| Team member transfer event payload | |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
