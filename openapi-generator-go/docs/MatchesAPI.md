# \MatchesAPI

All URIs are relative to *https://believe.cjav.dev*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateMatchMatchesPost**](MatchesAPI.md#CreateMatchMatchesPost) | **Post** /matches | Create a new match
[**DeleteMatchMatchesMatchIdDelete**](MatchesAPI.md#DeleteMatchMatchesMatchIdDelete) | **Delete** /matches/{match_id} | Delete a match
[**GetMatchLessonMatchesMatchIdLessonGet**](MatchesAPI.md#GetMatchLessonMatchesMatchIdLessonGet) | **Get** /matches/{match_id}/lesson | Get match lesson
[**GetMatchMatchesMatchIdGet**](MatchesAPI.md#GetMatchMatchesMatchIdGet) | **Get** /matches/{match_id} | Get a match by ID
[**GetTurningPointsMatchesMatchIdTurningPointsGet**](MatchesAPI.md#GetTurningPointsMatchesMatchIdTurningPointsGet) | **Get** /matches/{match_id}/turning-points | Get match turning points
[**ListMatchesMatchesGet**](MatchesAPI.md#ListMatchesMatchesGet) | **Get** /matches | List all matches
[**UpdateMatchMatchesMatchIdPatch**](MatchesAPI.md#UpdateMatchMatchesMatchIdPatch) | **Patch** /matches/{match_id} | Update a match



## CreateMatchMatchesPost

> Match CreateMatchMatchesPost(ctx).MatchCreate(matchCreate).Execute()

Create a new match



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
    "time"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	matchCreate := *openapiclient.NewMatchCreate("manchester-city", time.Now(), "afc-richmond", openapiclient.MatchType("league")) // MatchCreate | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MatchesAPI.CreateMatchMatchesPost(context.Background()).MatchCreate(matchCreate).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MatchesAPI.CreateMatchMatchesPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateMatchMatchesPost`: Match
	fmt.Fprintf(os.Stdout, "Response from `MatchesAPI.CreateMatchMatchesPost`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateMatchMatchesPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **matchCreate** | [**MatchCreate**](MatchCreate.md) |  | 

### Return type

[**Match**](Match.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteMatchMatchesMatchIdDelete

> DeleteMatchMatchesMatchIdDelete(ctx, matchId).Execute()

Delete a match



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
	r, err := apiClient.MatchesAPI.DeleteMatchMatchesMatchIdDelete(context.Background(), matchId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MatchesAPI.DeleteMatchMatchesMatchIdDelete``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**matchId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteMatchMatchesMatchIdDeleteRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

 (empty response body)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetMatchLessonMatchesMatchIdLessonGet

> map[string]interface{} GetMatchLessonMatchesMatchIdLessonGet(ctx, matchId).Execute()

Get match lesson



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
	resp, r, err := apiClient.MatchesAPI.GetMatchLessonMatchesMatchIdLessonGet(context.Background(), matchId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MatchesAPI.GetMatchLessonMatchesMatchIdLessonGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetMatchLessonMatchesMatchIdLessonGet`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `MatchesAPI.GetMatchLessonMatchesMatchIdLessonGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**matchId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetMatchLessonMatchesMatchIdLessonGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

**map[string]interface{}**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetMatchMatchesMatchIdGet

> Match GetMatchMatchesMatchIdGet(ctx, matchId).Execute()

Get a match by ID



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
	resp, r, err := apiClient.MatchesAPI.GetMatchMatchesMatchIdGet(context.Background(), matchId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MatchesAPI.GetMatchMatchesMatchIdGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetMatchMatchesMatchIdGet`: Match
	fmt.Fprintf(os.Stdout, "Response from `MatchesAPI.GetMatchMatchesMatchIdGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**matchId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetMatchMatchesMatchIdGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**Match**](Match.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetTurningPointsMatchesMatchIdTurningPointsGet

> []map[string]interface{} GetTurningPointsMatchesMatchIdTurningPointsGet(ctx, matchId).Execute()

Get match turning points



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
	resp, r, err := apiClient.MatchesAPI.GetTurningPointsMatchesMatchIdTurningPointsGet(context.Background(), matchId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MatchesAPI.GetTurningPointsMatchesMatchIdTurningPointsGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetTurningPointsMatchesMatchIdTurningPointsGet`: []map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `MatchesAPI.GetTurningPointsMatchesMatchIdTurningPointsGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**matchId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetTurningPointsMatchesMatchIdTurningPointsGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**[]map[string]interface{}**](map.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListMatchesMatchesGet

> PaginatedResponseMatch ListMatchesMatchesGet(ctx).TeamId(teamId).Result(result).MatchType(matchType).Skip(skip).Limit(limit).Execute()

List all matches



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
	teamId := "teamId_example" // string | Filter by team (home or away) (optional)
	result := openapiclient.MatchResult("win") // MatchResult | Filter by result (optional)
	matchType := openapiclient.MatchType("league") // MatchType | Filter by match type (optional)
	skip := int32(56) // int32 | Number of items to skip (offset) (optional) (default to 0)
	limit := int32(56) // int32 | Maximum number of items to return (max: 100) (optional) (default to 20)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MatchesAPI.ListMatchesMatchesGet(context.Background()).TeamId(teamId).Result(result).MatchType(matchType).Skip(skip).Limit(limit).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MatchesAPI.ListMatchesMatchesGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListMatchesMatchesGet`: PaginatedResponseMatch
	fmt.Fprintf(os.Stdout, "Response from `MatchesAPI.ListMatchesMatchesGet`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListMatchesMatchesGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **teamId** | **string** | Filter by team (home or away) | 
 **result** | [**MatchResult**](MatchResult.md) | Filter by result | 
 **matchType** | [**MatchType**](MatchType.md) | Filter by match type | 
 **skip** | **int32** | Number of items to skip (offset) | [default to 0]
 **limit** | **int32** | Maximum number of items to return (max: 100) | [default to 20]

### Return type

[**PaginatedResponseMatch**](PaginatedResponseMatch.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateMatchMatchesMatchIdPatch

> Match UpdateMatchMatchesMatchIdPatch(ctx, matchId).MatchUpdate(matchUpdate).Execute()

Update a match



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
	matchUpdate := *openapiclient.NewMatchUpdate() // MatchUpdate | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MatchesAPI.UpdateMatchMatchesMatchIdPatch(context.Background(), matchId).MatchUpdate(matchUpdate).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MatchesAPI.UpdateMatchMatchesMatchIdPatch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateMatchMatchesMatchIdPatch`: Match
	fmt.Fprintf(os.Stdout, "Response from `MatchesAPI.UpdateMatchMatchesMatchIdPatch`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**matchId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateMatchMatchesMatchIdPatchRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **matchUpdate** | [**MatchUpdate**](MatchUpdate.md) |  | 

### Return type

[**Match**](Match.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

