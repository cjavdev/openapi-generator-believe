# OpenapiClient::WebhooksApi

All URIs are relative to *https://believe.cjav.dev*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**match_completed_webhook**](WebhooksApi.md#match_completed_webhook) | **POST** /matchCompleted | Match Completed |
| [**team_member_transferred_webhook**](WebhooksApi.md#team_member_transferred_webhook) | **POST** /teamMemberTransferred | Team Member Transferred |


## match_completed_webhook

> match_completed_webhook(match_completed_event)

Match Completed

Fired when a football match completes. Contains final score, result, and Ted's post-match wisdom.

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WebhooksApi.new
match_completed_event =  # MatchCompletedEvent | Match completed event payload

begin
  # Match Completed
  api_instance.match_completed_webhook(match_completed_event)
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebhooksApi->match_completed_webhook: #{e}"
end
```

#### Using the match_completed_webhook_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> match_completed_webhook_with_http_info(match_completed_event)

```ruby
begin
  # Match Completed
  data, status_code, headers = api_instance.match_completed_webhook_with_http_info(match_completed_event)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebhooksApi->match_completed_webhook_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **match_completed_event** | [**MatchCompletedEvent**](MatchCompletedEvent.md) | Match completed event payload |  |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined


## team_member_transferred_webhook

> team_member_transferred_webhook(team_member_transferred_event)

Team Member Transferred

Fired when a player, coach, or staff member joins or departs from a team. Transfer news is big in football!

### Examples

```ruby
require 'time'
require 'openapi_client'

api_instance = OpenapiClient::WebhooksApi.new
team_member_transferred_event =  # TeamMemberTransferredEvent | Team member transfer event payload

begin
  # Team Member Transferred
  api_instance.team_member_transferred_webhook(team_member_transferred_event)
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebhooksApi->team_member_transferred_webhook: #{e}"
end
```

#### Using the team_member_transferred_webhook_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> team_member_transferred_webhook_with_http_info(team_member_transferred_event)

```ruby
begin
  # Team Member Transferred
  data, status_code, headers = api_instance.team_member_transferred_webhook_with_http_info(team_member_transferred_event)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling WebhooksApi->team_member_transferred_webhook_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **team_member_transferred_event** | [**TeamMemberTransferredEvent**](TeamMemberTransferredEvent.md) | Team member transfer event payload |  |

### Return type

nil (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined

