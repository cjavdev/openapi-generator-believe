# Org.OpenAPITools.Api.WebhooksApi

All URIs are relative to *https://believe.cjav.dev*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**MatchCompletedWebhook**](WebhooksApi.md#matchcompletedwebhook) | **POST** /matchCompleted | Match Completed |
| [**TeamMemberTransferredWebhook**](WebhooksApi.md#teammembertransferredwebhook) | **POST** /teamMemberTransferred | Team Member Transferred |

<a id="matchcompletedwebhook"></a>
# **MatchCompletedWebhook**
> void MatchCompletedWebhook (MatchCompletedEvent matchCompletedEvent)

Match Completed

Fired when a football match completes. Contains final score, result, and Ted's post-match wisdom.


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **matchCompletedEvent** | [**MatchCompletedEvent**](MatchCompletedEvent.md) | Match completed event payload |  |

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
| **200** | Webhook received successfully |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="teammembertransferredwebhook"></a>
# **TeamMemberTransferredWebhook**
> void TeamMemberTransferredWebhook (TeamMemberTransferredEvent teamMemberTransferredEvent)

Team Member Transferred

Fired when a player, coach, or staff member joins or departs from a team. Transfer news is big in football!


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **teamMemberTransferredEvent** | [**TeamMemberTransferredEvent**](TeamMemberTransferredEvent.md) | Team member transfer event payload |  |

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
| **200** | Webhook received successfully |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

