# WebhooksApi

All URIs are relative to *https://believe.cjav.dev*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**matchCompletedWebhook**](WebhooksApi.md#matchcompletedwebhook) | **POST** /matchCompleted | Match Completed |
| [**teamMemberTransferredWebhook**](WebhooksApi.md#teammembertransferredwebhook) | **POST** /teamMemberTransferred | Team Member Transferred |



## matchCompletedWebhook

> matchCompletedWebhook(matchCompletedEvent)

Match Completed

Fired when a football match completes. Contains final score, result, and Ted\&#39;s post-match wisdom.

### Example

```ts
import {
  Configuration,
  WebhooksApi,
} from '';
import type { MatchCompletedWebhookRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const api = new WebhooksApi();

  const body = {
    // MatchCompletedEvent | Match completed event payload
    matchCompletedEvent: {"created_at":"2024-01-15T17:00:00Z","data":{"away_score":1,"away_team_id":"manchester-city","completed_at":"2024-01-15T16:52:00Z","home_score":2,"home_team_id":"afc-richmond","lesson_learned":"Believing in each other is more powerful than any tactics board.","man_of_the_match":"Jamie Tartt","match_id":"match-001","match_type":"league","result":"home_win","ted_post_match_quote":"Win or lose, we did it together. And that's what makes us a team, not just a group of people wearing the same color shirts."},"event_id":"evt_abc123def456","event_type":"match.completed"},
  } satisfies MatchCompletedWebhookRequest;

  try {
    const data = await api.matchCompletedWebhook(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **matchCompletedEvent** | [MatchCompletedEvent](MatchCompletedEvent.md) | Match completed event payload | |

### Return type

`void` (Empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: Not defined


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Webhook received successfully |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## teamMemberTransferredWebhook

> teamMemberTransferredWebhook(teamMemberTransferredEvent)

Team Member Transferred

Fired when a player, coach, or staff member joins or departs from a team. Transfer news is big in football!

### Example

```ts
import {
  Configuration,
  WebhooksApi,
} from '';
import type { TeamMemberTransferredWebhookRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const api = new WebhooksApi();

  const body = {
    // TeamMemberTransferredEvent | Team member transfer event payload
    teamMemberTransferredEvent: {"created_at":"2024-01-10T09:00:00Z","data":{"character_id":"jamie-tartt","character_name":"Jamie Tartt","member_type":"player","previous_team_id":"manchester-city","previous_team_name":"Manchester City","team_id":"afc-richmond","team_member_id":"jamie-tartt-richmond","team_name":"AFC Richmond","ted_reaction":"You know what? Sometimes people need to go away to realize where they belong. Welcome home, Jamie.","transfer_fee_gbp":"15000000.00","transfer_type":"joined","years_with_previous_team":2},"event_id":"evt_xyz789ghi012","event_type":"team_member.transferred"},
  } satisfies TeamMemberTransferredWebhookRequest;

  try {
    const data = await api.teamMemberTransferredWebhook(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **teamMemberTransferredEvent** | [TeamMemberTransferredEvent](TeamMemberTransferredEvent.md) | Team member transfer event payload | |

### Return type

`void` (Empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: Not defined


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Webhook received successfully |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

