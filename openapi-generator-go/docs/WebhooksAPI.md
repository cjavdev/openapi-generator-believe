# \WebhooksAPI

All URIs are relative to *https://believe.cjav.dev*

Method | HTTP request | Description
------------- | ------------- | -------------
[**MatchCompletedWebhook**](WebhooksAPI.md#MatchCompletedWebhook) | **Post** /matchCompleted | Match Completed
[**TeamMemberTransferredWebhook**](WebhooksAPI.md#TeamMemberTransferredWebhook) | **Post** /teamMemberTransferred | Team Member Transferred



## MatchCompletedWebhook

> MatchCompletedWebhook(ctx).MatchCompletedEvent(matchCompletedEvent).Execute()

Match Completed



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	matchCompletedEvent :=  // MatchCompletedEvent | Match completed event payload

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.WebhooksAPI.MatchCompletedWebhook(context.Background()).MatchCompletedEvent(matchCompletedEvent).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WebhooksAPI.MatchCompletedWebhook``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiMatchCompletedWebhookRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **matchCompletedEvent** | [**MatchCompletedEvent**](MatchCompletedEvent.md) | Match completed event payload | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## TeamMemberTransferredWebhook

> TeamMemberTransferredWebhook(ctx).TeamMemberTransferredEvent(teamMemberTransferredEvent).Execute()

Team Member Transferred



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	teamMemberTransferredEvent :=  // TeamMemberTransferredEvent | Team member transfer event payload

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.WebhooksAPI.TeamMemberTransferredWebhook(context.Background()).TeamMemberTransferredEvent(teamMemberTransferredEvent).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WebhooksAPI.TeamMemberTransferredWebhook``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiTeamMemberTransferredWebhookRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **teamMemberTransferredEvent** | [**TeamMemberTransferredEvent**](TeamMemberTransferredEvent.md) | Team member transfer event payload | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

