# WebhooksApi

All URIs are relative to *https://believe.cjav.dev*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**matchCompletedWebhook**](WebhooksApi.md#matchCompletedWebhook) | **POST** /matchCompleted | Match Completed |
| [**teamMemberTransferredWebhook**](WebhooksApi.md#teamMemberTransferredWebhook) | **POST** /teamMemberTransferred | Team Member Transferred |


<a id="matchCompletedWebhook"></a>
# **matchCompletedWebhook**
> matchCompletedWebhook(matchCompletedEvent)

Match Completed

Fired when a football match completes. Contains final score, result, and Ted&#39;s post-match wisdom.

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.models.*;
import org.openapitools.client.api.WebhooksApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://believe.cjav.dev");

    WebhooksApi apiInstance = new WebhooksApi(defaultClient);
    MatchCompletedEvent matchCompletedEvent = new MatchCompletedEvent(); // MatchCompletedEvent | Match completed event payload
    try {
      apiInstance.matchCompletedWebhook(matchCompletedEvent);
    } catch (ApiException e) {
      System.err.println("Exception when calling WebhooksApi#matchCompletedWebhook");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **matchCompletedEvent** | [**MatchCompletedEvent**](MatchCompletedEvent.md)| Match completed event payload | |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Webhook received successfully |  -  |

<a id="teamMemberTransferredWebhook"></a>
# **teamMemberTransferredWebhook**
> teamMemberTransferredWebhook(teamMemberTransferredEvent)

Team Member Transferred

Fired when a player, coach, or staff member joins or departs from a team. Transfer news is big in football!

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.models.*;
import org.openapitools.client.api.WebhooksApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://believe.cjav.dev");

    WebhooksApi apiInstance = new WebhooksApi(defaultClient);
    TeamMemberTransferredEvent teamMemberTransferredEvent = new TeamMemberTransferredEvent(); // TeamMemberTransferredEvent | Team member transfer event payload
    try {
      apiInstance.teamMemberTransferredWebhook(teamMemberTransferredEvent);
    } catch (ApiException e) {
      System.err.println("Exception when calling WebhooksApi#teamMemberTransferredWebhook");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **teamMemberTransferredEvent** | [**TeamMemberTransferredEvent**](TeamMemberTransferredEvent.md)| Team member transfer event payload | |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Webhook received successfully |  -  |

