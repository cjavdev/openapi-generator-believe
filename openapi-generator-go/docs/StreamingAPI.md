# \StreamingAPI

All URIs are relative to *https://believe.cjav.dev*

Method | HTTP request | Description
------------- | ------------- | -------------
[**GetPepTalkPepTalkGet**](StreamingAPI.md#GetPepTalkPepTalkGet) | **Get** /pep-talk | Get a Pep Talk
[**StreamMatchCommentaryMatchesMatchIdCommentaryStreamPost**](StreamingAPI.md#StreamMatchCommentaryMatchesMatchIdCommentaryStreamPost) | **Post** /matches/{match_id}/commentary/stream | Stream Match Commentary
[**TestStreamStreamTestGet**](StreamingAPI.md#TestStreamStreamTestGet) | **Get** /stream/test | Test SSE Connection



## GetPepTalkPepTalkGet

> PepTalkResponse GetPepTalkPepTalkGet(ctx).Stream(stream).Execute()

Get a Pep Talk



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
	stream := true // bool | If true, returns SSE stream instead of full response (optional) (default to false)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.StreamingAPI.GetPepTalkPepTalkGet(context.Background()).Stream(stream).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `StreamingAPI.GetPepTalkPepTalkGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetPepTalkPepTalkGet`: PepTalkResponse
	fmt.Fprintf(os.Stdout, "Response from `StreamingAPI.GetPepTalkPepTalkGet`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGetPepTalkPepTalkGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **stream** | **bool** | If true, returns SSE stream instead of full response | [default to false]

### Return type

[**PepTalkResponse**](PepTalkResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, text/event-stream

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## StreamMatchCommentaryMatchesMatchIdCommentaryStreamPost

> interface{} StreamMatchCommentaryMatchesMatchIdCommentaryStreamPost(ctx, matchId).Execute()

Stream Match Commentary



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
	matchId := "matchId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.StreamingAPI.StreamMatchCommentaryMatchesMatchIdCommentaryStreamPost(context.Background(), matchId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `StreamingAPI.StreamMatchCommentaryMatchesMatchIdCommentaryStreamPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `StreamMatchCommentaryMatchesMatchIdCommentaryStreamPost`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `StreamingAPI.StreamMatchCommentaryMatchesMatchIdCommentaryStreamPost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**matchId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiStreamMatchCommentaryMatchesMatchIdCommentaryStreamPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

**interface{}**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, text/event-stream

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## TestStreamStreamTestGet

> interface{} TestStreamStreamTestGet(ctx).Execute()

Test SSE Connection



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
	resp, r, err := apiClient.StreamingAPI.TestStreamStreamTestGet(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `StreamingAPI.TestStreamStreamTestGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TestStreamStreamTestGet`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `StreamingAPI.TestStreamStreamTestGet`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiTestStreamStreamTestGetRequest struct via the builder pattern


### Return type

**interface{}**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, text/event-stream

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

