# \WebSocketAPI

All URIs are relative to *https://believe.cjav.dev*

Method | HTTP request | Description
------------- | ------------- | -------------
[**LiveMatchWebsocket**](WebSocketAPI.md#LiveMatchWebsocket) | **Get** /matches/live | Live Match Simulation WebSocket
[**WebsocketTest**](WebSocketAPI.md#WebsocketTest) | **Get** /ws/test | WebSocket Test Endpoint



## LiveMatchWebsocket

> LiveMatchWebsocket(ctx).HomeTeam(homeTeam).AwayTeam(awayTeam).Speed(speed).ExcitementLevel(excitementLevel).Execute()

Live Match Simulation WebSocket



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
	homeTeam := "homeTeam_example" // string | Home team name (optional) (default to "AFC Richmond")
	awayTeam := "awayTeam_example" // string | Away team name (optional) (default to "West Ham United")
	speed := float32(8.14) // float32 | Simulation speed multiplier (1.0 = real-time) (optional) (default to 1.0)
	excitementLevel := int32(56) // int32 | How eventful the match should be (1=boring, 10=chaos) (optional) (default to 5)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.WebSocketAPI.LiveMatchWebsocket(context.Background()).HomeTeam(homeTeam).AwayTeam(awayTeam).Speed(speed).ExcitementLevel(excitementLevel).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WebSocketAPI.LiveMatchWebsocket``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiLiveMatchWebsocketRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **homeTeam** | **string** | Home team name | [default to &quot;AFC Richmond&quot;]
 **awayTeam** | **string** | Away team name | [default to &quot;West Ham United&quot;]
 **speed** | **float32** | Simulation speed multiplier (1.0 &#x3D; real-time) | [default to 1.0]
 **excitementLevel** | **int32** | How eventful the match should be (1&#x3D;boring, 10&#x3D;chaos) | [default to 5]

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## WebsocketTest

> WebsocketTest(ctx).Execute()

WebSocket Test Endpoint



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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.WebSocketAPI.WebsocketTest(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WebSocketAPI.WebsocketTest``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiWebsocketTestRequest struct via the builder pattern


### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

