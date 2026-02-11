# \InteractiveAPI

All URIs are relative to *https://believe.cjav.dev*

Method | HTTP request | Description
------------- | ------------- | -------------
[**BelieveEngineBelievePost**](InteractiveAPI.md#BelieveEngineBelievePost) | **Post** /believe | The Believe Engine
[**GetBiscuitBiscuitsBiscuitIdGet**](InteractiveAPI.md#GetBiscuitBiscuitsBiscuitIdGet) | **Get** /biscuits/{biscuit_id} | Get a Specific Biscuit
[**GetBiscuitsBiscuitsGet**](InteractiveAPI.md#GetBiscuitsBiscuitsGet) | **Get** /biscuits | Biscuits as a Service
[**GetCoachingPrincipleCoachingPrinciplesPrincipleIdGet**](InteractiveAPI.md#GetCoachingPrincipleCoachingPrinciplesPrincipleIdGet) | **Get** /coaching/principles/{principle_id} | Get a Specific Coaching Principle
[**GetCoachingPrinciplesCoachingPrinciplesGet**](InteractiveAPI.md#GetCoachingPrinciplesCoachingPrinciplesGet) | **Get** /coaching/principles | Get Coaching Principles
[**GetFreshBiscuitBiscuitsFreshGet**](InteractiveAPI.md#GetFreshBiscuitBiscuitsFreshGet) | **Get** /biscuits/fresh | Get a Fresh Biscuit
[**GetRandomPrincipleCoachingPrinciplesRandomGet**](InteractiveAPI.md#GetRandomPrincipleCoachingPrinciplesRandomGet) | **Get** /coaching/principles/random | Get a Random Coaching Principle
[**PressConferencePressPost**](InteractiveAPI.md#PressConferencePressPost) | **Post** /press | Press Conference Simulator
[**ReframeThoughtReframePost**](InteractiveAPI.md#ReframeThoughtReframePost) | **Post** /reframe | Reframe Negative Thoughts
[**ResolveConflictConflictsResolvePost**](InteractiveAPI.md#ResolveConflictConflictsResolvePost) | **Post** /conflicts/resolve | Resolve Conflicts



## BelieveEngineBelievePost

> BelieveResponse BelieveEngineBelievePost(ctx).BelieveRequest(believeRequest).Execute()

The Believe Engine



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
	believeRequest := *openapiclient.NewBelieveRequest("I just got passed over for a promotion I've been working toward for two years.", openapiclient.SituationType("work_challenge")) // BelieveRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InteractiveAPI.BelieveEngineBelievePost(context.Background()).BelieveRequest(believeRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InteractiveAPI.BelieveEngineBelievePost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BelieveEngineBelievePost`: BelieveResponse
	fmt.Fprintf(os.Stdout, "Response from `InteractiveAPI.BelieveEngineBelievePost`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiBelieveEngineBelievePostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **believeRequest** | [**BelieveRequest**](BelieveRequest.md) |  | 

### Return type

[**BelieveResponse**](BelieveResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetBiscuitBiscuitsBiscuitIdGet

> Biscuit GetBiscuitBiscuitsBiscuitIdGet(ctx, biscuitId).Execute()

Get a Specific Biscuit



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
	biscuitId := "biscuitId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InteractiveAPI.GetBiscuitBiscuitsBiscuitIdGet(context.Background(), biscuitId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InteractiveAPI.GetBiscuitBiscuitsBiscuitIdGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetBiscuitBiscuitsBiscuitIdGet`: Biscuit
	fmt.Fprintf(os.Stdout, "Response from `InteractiveAPI.GetBiscuitBiscuitsBiscuitIdGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**biscuitId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetBiscuitBiscuitsBiscuitIdGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**Biscuit**](Biscuit.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetBiscuitsBiscuitsGet

> PaginatedResponseBiscuit GetBiscuitsBiscuitsGet(ctx).Skip(skip).Limit(limit).Execute()

Biscuits as a Service



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
	skip := int32(56) // int32 | Number of items to skip (offset) (optional) (default to 0)
	limit := int32(56) // int32 | Maximum number of items to return (max: 100) (optional) (default to 20)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InteractiveAPI.GetBiscuitsBiscuitsGet(context.Background()).Skip(skip).Limit(limit).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InteractiveAPI.GetBiscuitsBiscuitsGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetBiscuitsBiscuitsGet`: PaginatedResponseBiscuit
	fmt.Fprintf(os.Stdout, "Response from `InteractiveAPI.GetBiscuitsBiscuitsGet`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGetBiscuitsBiscuitsGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **skip** | **int32** | Number of items to skip (offset) | [default to 0]
 **limit** | **int32** | Maximum number of items to return (max: 100) | [default to 20]

### Return type

[**PaginatedResponseBiscuit**](PaginatedResponseBiscuit.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetCoachingPrincipleCoachingPrinciplesPrincipleIdGet

> CoachingPrinciple GetCoachingPrincipleCoachingPrinciplesPrincipleIdGet(ctx, principleId).Execute()

Get a Specific Coaching Principle



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
	principleId := "principleId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InteractiveAPI.GetCoachingPrincipleCoachingPrinciplesPrincipleIdGet(context.Background(), principleId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InteractiveAPI.GetCoachingPrincipleCoachingPrinciplesPrincipleIdGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetCoachingPrincipleCoachingPrinciplesPrincipleIdGet`: CoachingPrinciple
	fmt.Fprintf(os.Stdout, "Response from `InteractiveAPI.GetCoachingPrincipleCoachingPrinciplesPrincipleIdGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**principleId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetCoachingPrincipleCoachingPrinciplesPrincipleIdGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**CoachingPrinciple**](CoachingPrinciple.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetCoachingPrinciplesCoachingPrinciplesGet

> PaginatedResponseCoachingPrinciple GetCoachingPrinciplesCoachingPrinciplesGet(ctx).Skip(skip).Limit(limit).Execute()

Get Coaching Principles



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
	skip := int32(56) // int32 | Number of items to skip (offset) (optional) (default to 0)
	limit := int32(56) // int32 | Maximum number of items to return (max: 100) (optional) (default to 20)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InteractiveAPI.GetCoachingPrinciplesCoachingPrinciplesGet(context.Background()).Skip(skip).Limit(limit).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InteractiveAPI.GetCoachingPrinciplesCoachingPrinciplesGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetCoachingPrinciplesCoachingPrinciplesGet`: PaginatedResponseCoachingPrinciple
	fmt.Fprintf(os.Stdout, "Response from `InteractiveAPI.GetCoachingPrinciplesCoachingPrinciplesGet`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGetCoachingPrinciplesCoachingPrinciplesGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **skip** | **int32** | Number of items to skip (offset) | [default to 0]
 **limit** | **int32** | Maximum number of items to return (max: 100) | [default to 20]

### Return type

[**PaginatedResponseCoachingPrinciple**](PaginatedResponseCoachingPrinciple.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetFreshBiscuitBiscuitsFreshGet

> Biscuit GetFreshBiscuitBiscuitsFreshGet(ctx).Execute()

Get a Fresh Biscuit



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
	resp, r, err := apiClient.InteractiveAPI.GetFreshBiscuitBiscuitsFreshGet(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InteractiveAPI.GetFreshBiscuitBiscuitsFreshGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetFreshBiscuitBiscuitsFreshGet`: Biscuit
	fmt.Fprintf(os.Stdout, "Response from `InteractiveAPI.GetFreshBiscuitBiscuitsFreshGet`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiGetFreshBiscuitBiscuitsFreshGetRequest struct via the builder pattern


### Return type

[**Biscuit**](Biscuit.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetRandomPrincipleCoachingPrinciplesRandomGet

> CoachingPrinciple GetRandomPrincipleCoachingPrinciplesRandomGet(ctx).Execute()

Get a Random Coaching Principle



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
	resp, r, err := apiClient.InteractiveAPI.GetRandomPrincipleCoachingPrinciplesRandomGet(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InteractiveAPI.GetRandomPrincipleCoachingPrinciplesRandomGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetRandomPrincipleCoachingPrinciplesRandomGet`: CoachingPrinciple
	fmt.Fprintf(os.Stdout, "Response from `InteractiveAPI.GetRandomPrincipleCoachingPrinciplesRandomGet`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiGetRandomPrincipleCoachingPrinciplesRandomGetRequest struct via the builder pattern


### Return type

[**CoachingPrinciple**](CoachingPrinciple.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## PressConferencePressPost

> PressConferenceResponse PressConferencePressPost(ctx).PressConferenceRequest(pressConferenceRequest).Execute()

Press Conference Simulator



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
	pressConferenceRequest := *openapiclient.NewPressConferenceRequest("Ted, your team just lost 5-0. How do you explain this embarrassing defeat?") // PressConferenceRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InteractiveAPI.PressConferencePressPost(context.Background()).PressConferenceRequest(pressConferenceRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InteractiveAPI.PressConferencePressPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PressConferencePressPost`: PressConferenceResponse
	fmt.Fprintf(os.Stdout, "Response from `InteractiveAPI.PressConferencePressPost`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiPressConferencePressPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **pressConferenceRequest** | [**PressConferenceRequest**](PressConferenceRequest.md) |  | 

### Return type

[**PressConferenceResponse**](PressConferenceResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ReframeThoughtReframePost

> ReframeResponse ReframeThoughtReframePost(ctx).ReframeRequest(reframeRequest).Execute()

Reframe Negative Thoughts



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
	reframeRequest := *openapiclient.NewReframeRequest("I'm not good enough for this job.") // ReframeRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InteractiveAPI.ReframeThoughtReframePost(context.Background()).ReframeRequest(reframeRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InteractiveAPI.ReframeThoughtReframePost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ReframeThoughtReframePost`: ReframeResponse
	fmt.Fprintf(os.Stdout, "Response from `InteractiveAPI.ReframeThoughtReframePost`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiReframeThoughtReframePostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **reframeRequest** | [**ReframeRequest**](ReframeRequest.md) |  | 

### Return type

[**ReframeResponse**](ReframeResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ResolveConflictConflictsResolvePost

> ConflictResolution ResolveConflictConflictsResolvePost(ctx).ConflictRequest(conflictRequest).Execute()

Resolve Conflicts



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
	conflictRequest := *openapiclient.NewConflictRequest(openapiclient.ConflictType("interpersonal"), "Alex keeps taking credit for my ideas in meetings and I'm getting resentful.", []string{"PartiesInvolved_example"}) // ConflictRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InteractiveAPI.ResolveConflictConflictsResolvePost(context.Background()).ConflictRequest(conflictRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InteractiveAPI.ResolveConflictConflictsResolvePost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ResolveConflictConflictsResolvePost`: ConflictResolution
	fmt.Fprintf(os.Stdout, "Response from `InteractiveAPI.ResolveConflictConflictsResolvePost`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiResolveConflictConflictsResolvePostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **conflictRequest** | [**ConflictRequest**](ConflictRequest.md) |  | 

### Return type

[**ConflictResolution**](ConflictResolution.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

