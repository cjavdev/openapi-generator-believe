# openapi_client.WebhooksApi

All URIs are relative to *https://believe.cjav.dev*

Method | HTTP request | Description
------------- | ------------- | -------------
[**match_completed_webhook**](WebhooksApi.md#match_completed_webhook) | **POST** /matchCompleted | Match Completed
[**team_member_transferred_webhook**](WebhooksApi.md#team_member_transferred_webhook) | **POST** /teamMemberTransferred | Team Member Transferred


# **match_completed_webhook**
> match_completed_webhook(match_completed_event)

Match Completed

Fired when a football match completes. Contains final score, result, and Ted's post-match wisdom.

### Example


```python
import openapi_client
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://believe.cjav.dev
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://believe.cjav.dev"
)


# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.WebhooksApi(api_client)
    match_completed_event = {"created_at":"2024-01-15T17:00:00Z","data":{"away_score":1,"away_team_id":"manchester-city","completed_at":"2024-01-15T16:52:00Z","home_score":2,"home_team_id":"afc-richmond","lesson_learned":"Believing in each other is more powerful than any tactics board.","man_of_the_match":"Jamie Tartt","match_id":"match-001","match_type":"league","result":"home_win","ted_post_match_quote":"Win or lose, we did it together. And that's what makes us a team, not just a group of people wearing the same color shirts."},"event_id":"evt_abc123def456","event_type":"match.completed"} # MatchCompletedEvent | Match completed event payload

    try:
        # Match Completed
        api_instance.match_completed_webhook(match_completed_event)
    except Exception as e:
        print("Exception when calling WebhooksApi->match_completed_webhook: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **match_completed_event** | [**MatchCompletedEvent**](MatchCompletedEvent.md)| Match completed event payload | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Webhook received successfully |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **team_member_transferred_webhook**
> team_member_transferred_webhook(team_member_transferred_event)

Team Member Transferred

Fired when a player, coach, or staff member joins or departs from a team. Transfer news is big in football!

### Example


```python
import openapi_client
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://believe.cjav.dev
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://believe.cjav.dev"
)


# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.WebhooksApi(api_client)
    team_member_transferred_event = {"created_at":"2024-01-10T09:00:00Z","data":{"character_id":"jamie-tartt","character_name":"Jamie Tartt","member_type":"player","previous_team_id":"manchester-city","previous_team_name":"Manchester City","team_id":"afc-richmond","team_member_id":"jamie-tartt-richmond","team_name":"AFC Richmond","ted_reaction":"You know what? Sometimes people need to go away to realize where they belong. Welcome home, Jamie.","transfer_fee_gbp":"15000000.00","transfer_type":"joined","years_with_previous_team":2},"event_id":"evt_xyz789ghi012","event_type":"team_member.transferred"} # TeamMemberTransferredEvent | Team member transfer event payload

    try:
        # Team Member Transferred
        api_instance.team_member_transferred_webhook(team_member_transferred_event)
    except Exception as e:
        print("Exception when calling WebhooksApi->team_member_transferred_webhook: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_member_transferred_event** | [**TeamMemberTransferredEvent**](TeamMemberTransferredEvent.md)| Team member transfer event payload | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Webhook received successfully |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

