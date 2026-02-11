# \TeamsAPI

All URIs are relative to *https://believe.cjav.dev*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateTeamTeamsPost**](TeamsAPI.md#CreateTeamTeamsPost) | **Post** /teams | Create a new team
[**DeleteTeamLogoTeamsTeamIdLogoFileIdDelete**](TeamsAPI.md#DeleteTeamLogoTeamsTeamIdLogoFileIdDelete) | **Delete** /teams/{team_id}/logo/{file_id} | Delete team logo
[**DeleteTeamTeamsTeamIdDelete**](TeamsAPI.md#DeleteTeamTeamsTeamIdDelete) | **Delete** /teams/{team_id} | Delete a team
[**DownloadTeamLogoTeamsTeamIdLogoFileIdGet**](TeamsAPI.md#DownloadTeamLogoTeamsTeamIdLogoFileIdGet) | **Get** /teams/{team_id}/logo/{file_id} | Download team logo
[**GetTeamCultureTeamsTeamIdCultureGet**](TeamsAPI.md#GetTeamCultureTeamsTeamIdCultureGet) | **Get** /teams/{team_id}/culture | Get team culture details
[**GetTeamRivalsTeamsTeamIdRivalsGet**](TeamsAPI.md#GetTeamRivalsTeamsTeamIdRivalsGet) | **Get** /teams/{team_id}/rivals | Get team&#39;s rivals
[**GetTeamTeamsTeamIdGet**](TeamsAPI.md#GetTeamTeamsTeamIdGet) | **Get** /teams/{team_id} | Get a team by ID
[**ListTeamLogosTeamsTeamIdLogosGet**](TeamsAPI.md#ListTeamLogosTeamsTeamIdLogosGet) | **Get** /teams/{team_id}/logos | List team logos
[**ListTeamsTeamsGet**](TeamsAPI.md#ListTeamsTeamsGet) | **Get** /teams | List all teams
[**UpdateTeamTeamsTeamIdPatch**](TeamsAPI.md#UpdateTeamTeamsTeamIdPatch) | **Patch** /teams/{team_id} | Update a team
[**UploadTeamLogoTeamsTeamIdLogoPost**](TeamsAPI.md#UploadTeamLogoTeamsTeamIdLogoPost) | **Post** /teams/{team_id}/logo | Upload team logo



## CreateTeamTeamsPost

> Team CreateTeamTeamsPost(ctx).TeamCreate(teamCreate).Execute()

Create a new team



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
	teamCreate := *openapiclient.NewTeamCreate(int32(85), int32(1897), openapiclient.League("Premier League"), "AFC Richmond", "Nelson Road", *openapiclient.NewTeamValues("Believe", []string{"SecondaryValues_example"}, "Football is life!")) // TeamCreate | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TeamsAPI.CreateTeamTeamsPost(context.Background()).TeamCreate(teamCreate).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TeamsAPI.CreateTeamTeamsPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateTeamTeamsPost`: Team
	fmt.Fprintf(os.Stdout, "Response from `TeamsAPI.CreateTeamTeamsPost`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateTeamTeamsPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **teamCreate** | [**TeamCreate**](TeamCreate.md) |  | 

### Return type

[**Team**](Team.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteTeamLogoTeamsTeamIdLogoFileIdDelete

> DeleteTeamLogoTeamsTeamIdLogoFileIdDelete(ctx, teamId, fileId).Execute()

Delete team logo



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
	teamId := "teamId_example" // string | 
	fileId := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.TeamsAPI.DeleteTeamLogoTeamsTeamIdLogoFileIdDelete(context.Background(), teamId, fileId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TeamsAPI.DeleteTeamLogoTeamsTeamIdLogoFileIdDelete``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**teamId** | **string** |  | 
**fileId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteTeamLogoTeamsTeamIdLogoFileIdDeleteRequest struct via the builder pattern


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


## DeleteTeamTeamsTeamIdDelete

> DeleteTeamTeamsTeamIdDelete(ctx, teamId).Execute()

Delete a team



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
	teamId := "teamId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.TeamsAPI.DeleteTeamTeamsTeamIdDelete(context.Background(), teamId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TeamsAPI.DeleteTeamTeamsTeamIdDelete``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**teamId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteTeamTeamsTeamIdDeleteRequest struct via the builder pattern


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


## DownloadTeamLogoTeamsTeamIdLogoFileIdGet

> interface{} DownloadTeamLogoTeamsTeamIdLogoFileIdGet(ctx, teamId, fileId).Execute()

Download team logo



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
	teamId := "teamId_example" // string | 
	fileId := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TeamsAPI.DownloadTeamLogoTeamsTeamIdLogoFileIdGet(context.Background(), teamId, fileId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TeamsAPI.DownloadTeamLogoTeamsTeamIdLogoFileIdGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DownloadTeamLogoTeamsTeamIdLogoFileIdGet`: interface{}
	fmt.Fprintf(os.Stdout, "Response from `TeamsAPI.DownloadTeamLogoTeamsTeamIdLogoFileIdGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**teamId** | **string** |  | 
**fileId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDownloadTeamLogoTeamsTeamIdLogoFileIdGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

**interface{}**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, image/*

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetTeamCultureTeamsTeamIdCultureGet

> map[string]interface{} GetTeamCultureTeamsTeamIdCultureGet(ctx, teamId).Execute()

Get team culture details



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
	teamId := "teamId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TeamsAPI.GetTeamCultureTeamsTeamIdCultureGet(context.Background(), teamId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TeamsAPI.GetTeamCultureTeamsTeamIdCultureGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetTeamCultureTeamsTeamIdCultureGet`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `TeamsAPI.GetTeamCultureTeamsTeamIdCultureGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**teamId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetTeamCultureTeamsTeamIdCultureGetRequest struct via the builder pattern


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


## GetTeamRivalsTeamsTeamIdRivalsGet

> []Team GetTeamRivalsTeamsTeamIdRivalsGet(ctx, teamId).Execute()

Get team's rivals



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
	teamId := "teamId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TeamsAPI.GetTeamRivalsTeamsTeamIdRivalsGet(context.Background(), teamId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TeamsAPI.GetTeamRivalsTeamsTeamIdRivalsGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetTeamRivalsTeamsTeamIdRivalsGet`: []Team
	fmt.Fprintf(os.Stdout, "Response from `TeamsAPI.GetTeamRivalsTeamsTeamIdRivalsGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**teamId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetTeamRivalsTeamsTeamIdRivalsGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**[]Team**](Team.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetTeamTeamsTeamIdGet

> Team GetTeamTeamsTeamIdGet(ctx, teamId).Execute()

Get a team by ID



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
	teamId := "teamId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TeamsAPI.GetTeamTeamsTeamIdGet(context.Background(), teamId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TeamsAPI.GetTeamTeamsTeamIdGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetTeamTeamsTeamIdGet`: Team
	fmt.Fprintf(os.Stdout, "Response from `TeamsAPI.GetTeamTeamsTeamIdGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**teamId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetTeamTeamsTeamIdGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**Team**](Team.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListTeamLogosTeamsTeamIdLogosGet

> []FileUploadResponse ListTeamLogosTeamsTeamIdLogosGet(ctx, teamId).Execute()

List team logos



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
	teamId := "teamId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TeamsAPI.ListTeamLogosTeamsTeamIdLogosGet(context.Background(), teamId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TeamsAPI.ListTeamLogosTeamsTeamIdLogosGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListTeamLogosTeamsTeamIdLogosGet`: []FileUploadResponse
	fmt.Fprintf(os.Stdout, "Response from `TeamsAPI.ListTeamLogosTeamsTeamIdLogosGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**teamId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiListTeamLogosTeamsTeamIdLogosGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**[]FileUploadResponse**](FileUploadResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListTeamsTeamsGet

> PaginatedResponseTeam ListTeamsTeamsGet(ctx).League(league).MinCultureScore(minCultureScore).Skip(skip).Limit(limit).Execute()

List all teams



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
	league := openapiclient.League("Premier League") // League | Filter by league (optional)
	minCultureScore := int32(56) // int32 | Minimum culture score (optional)
	skip := int32(56) // int32 | Number of items to skip (offset) (optional) (default to 0)
	limit := int32(56) // int32 | Maximum number of items to return (max: 100) (optional) (default to 20)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TeamsAPI.ListTeamsTeamsGet(context.Background()).League(league).MinCultureScore(minCultureScore).Skip(skip).Limit(limit).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TeamsAPI.ListTeamsTeamsGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListTeamsTeamsGet`: PaginatedResponseTeam
	fmt.Fprintf(os.Stdout, "Response from `TeamsAPI.ListTeamsTeamsGet`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListTeamsTeamsGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **league** | [**League**](League.md) | Filter by league | 
 **minCultureScore** | **int32** | Minimum culture score | 
 **skip** | **int32** | Number of items to skip (offset) | [default to 0]
 **limit** | **int32** | Maximum number of items to return (max: 100) | [default to 20]

### Return type

[**PaginatedResponseTeam**](PaginatedResponseTeam.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateTeamTeamsTeamIdPatch

> Team UpdateTeamTeamsTeamIdPatch(ctx, teamId).TeamUpdate(teamUpdate).Execute()

Update a team



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
	teamId := "teamId_example" // string | 
	teamUpdate := *openapiclient.NewTeamUpdate() // TeamUpdate | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TeamsAPI.UpdateTeamTeamsTeamIdPatch(context.Background(), teamId).TeamUpdate(teamUpdate).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TeamsAPI.UpdateTeamTeamsTeamIdPatch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateTeamTeamsTeamIdPatch`: Team
	fmt.Fprintf(os.Stdout, "Response from `TeamsAPI.UpdateTeamTeamsTeamIdPatch`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**teamId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateTeamTeamsTeamIdPatchRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **teamUpdate** | [**TeamUpdate**](TeamUpdate.md) |  | 

### Return type

[**Team**](Team.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UploadTeamLogoTeamsTeamIdLogoPost

> FileUploadResponse UploadTeamLogoTeamsTeamIdLogoPost(ctx, teamId).File(file).Execute()

Upload team logo



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
	teamId := "teamId_example" // string | 
	file := os.NewFile(1234, "some_file") // *os.File | Logo image file

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TeamsAPI.UploadTeamLogoTeamsTeamIdLogoPost(context.Background(), teamId).File(file).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TeamsAPI.UploadTeamLogoTeamsTeamIdLogoPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UploadTeamLogoTeamsTeamIdLogoPost`: FileUploadResponse
	fmt.Fprintf(os.Stdout, "Response from `TeamsAPI.UploadTeamLogoTeamsTeamIdLogoPost`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**teamId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUploadTeamLogoTeamsTeamIdLogoPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **file** | ***os.File** | Logo image file | 

### Return type

[**FileUploadResponse**](FileUploadResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

