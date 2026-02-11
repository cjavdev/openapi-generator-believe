# \EpisodesAPI

All URIs are relative to *https://believe.cjav.dev*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateEpisodeEpisodesPost**](EpisodesAPI.md#CreateEpisodeEpisodesPost) | **Post** /episodes | Create a new episode
[**DeleteEpisodeEpisodesEpisodeIdDelete**](EpisodesAPI.md#DeleteEpisodeEpisodesEpisodeIdDelete) | **Delete** /episodes/{episode_id} | Delete an episode
[**GetEpisodeEpisodesEpisodeIdGet**](EpisodesAPI.md#GetEpisodeEpisodesEpisodeIdGet) | **Get** /episodes/{episode_id} | Get an episode by ID
[**GetEpisodeWisdomEpisodesEpisodeIdWisdomGet**](EpisodesAPI.md#GetEpisodeWisdomEpisodesEpisodeIdWisdomGet) | **Get** /episodes/{episode_id}/wisdom | Get episode wisdom
[**GetSeasonEpisodesEpisodesSeasonsSeasonNumberGet**](EpisodesAPI.md#GetSeasonEpisodesEpisodesSeasonsSeasonNumberGet) | **Get** /episodes/seasons/{season_number} | Get all episodes from a season
[**ListEpisodesEpisodesGet**](EpisodesAPI.md#ListEpisodesEpisodesGet) | **Get** /episodes | List all episodes
[**UpdateEpisodeEpisodesEpisodeIdPatch**](EpisodesAPI.md#UpdateEpisodeEpisodesEpisodeIdPatch) | **Patch** /episodes/{episode_id} | Update an episode



## CreateEpisodeEpisodesPost

> Episode CreateEpisodeEpisodesPost(ctx).EpisodeCreate(episodeCreate).Execute()

Create a new episode



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
	episodeCreate := *openapiclient.NewEpisodeCreate(time.Now(), []string{"CharacterFocus_example"}, "Director_example", int32(123), "Taking chances and believing in yourself", int32(123), int32(123), "American football coach Ted Lasso is hired to manage AFC Richmond, a struggling English Premier League team.", "Taking on a challenge is a lot like riding a horse. If you're comfortable while you're doing it, you're probably doing it wrong.", "Pilot", "Writer_example") // EpisodeCreate | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EpisodesAPI.CreateEpisodeEpisodesPost(context.Background()).EpisodeCreate(episodeCreate).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EpisodesAPI.CreateEpisodeEpisodesPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateEpisodeEpisodesPost`: Episode
	fmt.Fprintf(os.Stdout, "Response from `EpisodesAPI.CreateEpisodeEpisodesPost`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateEpisodeEpisodesPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **episodeCreate** | [**EpisodeCreate**](EpisodeCreate.md) |  | 

### Return type

[**Episode**](Episode.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteEpisodeEpisodesEpisodeIdDelete

> DeleteEpisodeEpisodesEpisodeIdDelete(ctx, episodeId).Execute()

Delete an episode



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
	episodeId := "episodeId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.EpisodesAPI.DeleteEpisodeEpisodesEpisodeIdDelete(context.Background(), episodeId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EpisodesAPI.DeleteEpisodeEpisodesEpisodeIdDelete``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**episodeId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteEpisodeEpisodesEpisodeIdDeleteRequest struct via the builder pattern


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


## GetEpisodeEpisodesEpisodeIdGet

> Episode GetEpisodeEpisodesEpisodeIdGet(ctx, episodeId).Execute()

Get an episode by ID



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
	episodeId := "episodeId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EpisodesAPI.GetEpisodeEpisodesEpisodeIdGet(context.Background(), episodeId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EpisodesAPI.GetEpisodeEpisodesEpisodeIdGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetEpisodeEpisodesEpisodeIdGet`: Episode
	fmt.Fprintf(os.Stdout, "Response from `EpisodesAPI.GetEpisodeEpisodesEpisodeIdGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**episodeId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetEpisodeEpisodesEpisodeIdGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**Episode**](Episode.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetEpisodeWisdomEpisodesEpisodeIdWisdomGet

> map[string]interface{} GetEpisodeWisdomEpisodesEpisodeIdWisdomGet(ctx, episodeId).Execute()

Get episode wisdom



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
	episodeId := "episodeId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EpisodesAPI.GetEpisodeWisdomEpisodesEpisodeIdWisdomGet(context.Background(), episodeId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EpisodesAPI.GetEpisodeWisdomEpisodesEpisodeIdWisdomGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetEpisodeWisdomEpisodesEpisodeIdWisdomGet`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `EpisodesAPI.GetEpisodeWisdomEpisodesEpisodeIdWisdomGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**episodeId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetEpisodeWisdomEpisodesEpisodeIdWisdomGetRequest struct via the builder pattern


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


## GetSeasonEpisodesEpisodesSeasonsSeasonNumberGet

> PaginatedResponseEpisode GetSeasonEpisodesEpisodesSeasonsSeasonNumberGet(ctx, seasonNumber).Skip(skip).Limit(limit).Execute()

Get all episodes from a season



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
	seasonNumber := int32(56) // int32 | 
	skip := int32(56) // int32 | Number of items to skip (offset) (optional) (default to 0)
	limit := int32(56) // int32 | Maximum number of items to return (max: 100) (optional) (default to 20)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EpisodesAPI.GetSeasonEpisodesEpisodesSeasonsSeasonNumberGet(context.Background(), seasonNumber).Skip(skip).Limit(limit).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EpisodesAPI.GetSeasonEpisodesEpisodesSeasonsSeasonNumberGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetSeasonEpisodesEpisodesSeasonsSeasonNumberGet`: PaginatedResponseEpisode
	fmt.Fprintf(os.Stdout, "Response from `EpisodesAPI.GetSeasonEpisodesEpisodesSeasonsSeasonNumberGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**seasonNumber** | **int32** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetSeasonEpisodesEpisodesSeasonsSeasonNumberGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **skip** | **int32** | Number of items to skip (offset) | [default to 0]
 **limit** | **int32** | Maximum number of items to return (max: 100) | [default to 20]

### Return type

[**PaginatedResponseEpisode**](PaginatedResponseEpisode.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListEpisodesEpisodesGet

> PaginatedResponseEpisode ListEpisodesEpisodesGet(ctx).Season(season).CharacterFocus(characterFocus).Skip(skip).Limit(limit).Execute()

List all episodes



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
	season := int32(56) // int32 | Filter by season (optional)
	characterFocus := "characterFocus_example" // string | Filter by character focus (character ID) (optional)
	skip := int32(56) // int32 | Number of items to skip (offset) (optional) (default to 0)
	limit := int32(56) // int32 | Maximum number of items to return (max: 100) (optional) (default to 20)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EpisodesAPI.ListEpisodesEpisodesGet(context.Background()).Season(season).CharacterFocus(characterFocus).Skip(skip).Limit(limit).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EpisodesAPI.ListEpisodesEpisodesGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListEpisodesEpisodesGet`: PaginatedResponseEpisode
	fmt.Fprintf(os.Stdout, "Response from `EpisodesAPI.ListEpisodesEpisodesGet`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListEpisodesEpisodesGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **season** | **int32** | Filter by season | 
 **characterFocus** | **string** | Filter by character focus (character ID) | 
 **skip** | **int32** | Number of items to skip (offset) | [default to 0]
 **limit** | **int32** | Maximum number of items to return (max: 100) | [default to 20]

### Return type

[**PaginatedResponseEpisode**](PaginatedResponseEpisode.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateEpisodeEpisodesEpisodeIdPatch

> Episode UpdateEpisodeEpisodesEpisodeIdPatch(ctx, episodeId).EpisodeUpdate(episodeUpdate).Execute()

Update an episode



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
	episodeId := "episodeId_example" // string | 
	episodeUpdate := *openapiclient.NewEpisodeUpdate() // EpisodeUpdate | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EpisodesAPI.UpdateEpisodeEpisodesEpisodeIdPatch(context.Background(), episodeId).EpisodeUpdate(episodeUpdate).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EpisodesAPI.UpdateEpisodeEpisodesEpisodeIdPatch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateEpisodeEpisodesEpisodeIdPatch`: Episode
	fmt.Fprintf(os.Stdout, "Response from `EpisodesAPI.UpdateEpisodeEpisodesEpisodeIdPatch`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**episodeId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateEpisodeEpisodesEpisodeIdPatchRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **episodeUpdate** | [**EpisodeUpdate**](EpisodeUpdate.md) |  | 

### Return type

[**Episode**](Episode.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

