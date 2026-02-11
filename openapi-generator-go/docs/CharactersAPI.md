# \CharactersAPI

All URIs are relative to *https://believe.cjav.dev*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateCharacterCharactersPost**](CharactersAPI.md#CreateCharacterCharactersPost) | **Post** /characters | Create a new character
[**DeleteCharacterCharactersCharacterIdDelete**](CharactersAPI.md#DeleteCharacterCharactersCharacterIdDelete) | **Delete** /characters/{character_id} | Delete a character
[**GetCharacterCharactersCharacterIdGet**](CharactersAPI.md#GetCharacterCharactersCharacterIdGet) | **Get** /characters/{character_id} | Get a character by ID
[**GetCharacterQuotesCharactersCharacterIdQuotesGet**](CharactersAPI.md#GetCharacterQuotesCharactersCharacterIdQuotesGet) | **Get** /characters/{character_id}/quotes | Get character&#39;s signature quotes
[**ListCharactersCharactersGet**](CharactersAPI.md#ListCharactersCharactersGet) | **Get** /characters | List all characters
[**UpdateCharacterCharactersCharacterIdPatch**](CharactersAPI.md#UpdateCharacterCharactersCharacterIdPatch) | **Patch** /characters/{character_id} | Update a character



## CreateCharacterCharactersPost

> Character CreateCharacterCharactersPost(ctx).CharacterCreate(characterCreate).Execute()

Create a new character



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
	characterCreate := *openapiclient.NewCharacterCreate("Former American football coach from Kansas who moved to London to coach AFC Richmond", *openapiclient.NewEmotionalStats(int32(99), int32(100), int32(95), int32(90), int32(80)), "Ted Lasso", []string{"PersonalityTraits_example"}, openapiclient.CharacterRole("coach")) // CharacterCreate | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CharactersAPI.CreateCharacterCharactersPost(context.Background()).CharacterCreate(characterCreate).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CharactersAPI.CreateCharacterCharactersPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateCharacterCharactersPost`: Character
	fmt.Fprintf(os.Stdout, "Response from `CharactersAPI.CreateCharacterCharactersPost`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateCharacterCharactersPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **characterCreate** | [**CharacterCreate**](CharacterCreate.md) |  | 

### Return type

[**Character**](Character.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteCharacterCharactersCharacterIdDelete

> DeleteCharacterCharactersCharacterIdDelete(ctx, characterId).Execute()

Delete a character



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
	characterId := "characterId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.CharactersAPI.DeleteCharacterCharactersCharacterIdDelete(context.Background(), characterId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CharactersAPI.DeleteCharacterCharactersCharacterIdDelete``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**characterId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteCharacterCharactersCharacterIdDeleteRequest struct via the builder pattern


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


## GetCharacterCharactersCharacterIdGet

> Character GetCharacterCharactersCharacterIdGet(ctx, characterId).Execute()

Get a character by ID



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
	characterId := "characterId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CharactersAPI.GetCharacterCharactersCharacterIdGet(context.Background(), characterId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CharactersAPI.GetCharacterCharactersCharacterIdGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetCharacterCharactersCharacterIdGet`: Character
	fmt.Fprintf(os.Stdout, "Response from `CharactersAPI.GetCharacterCharactersCharacterIdGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**characterId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetCharacterCharactersCharacterIdGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**Character**](Character.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetCharacterQuotesCharactersCharacterIdQuotesGet

> []*string GetCharacterQuotesCharactersCharacterIdQuotesGet(ctx, characterId).Execute()

Get character's signature quotes



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
	characterId := "characterId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CharactersAPI.GetCharacterQuotesCharactersCharacterIdQuotesGet(context.Background(), characterId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CharactersAPI.GetCharacterQuotesCharactersCharacterIdQuotesGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetCharacterQuotesCharactersCharacterIdQuotesGet`: []*string
	fmt.Fprintf(os.Stdout, "Response from `CharactersAPI.GetCharacterQuotesCharactersCharacterIdQuotesGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**characterId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetCharacterQuotesCharactersCharacterIdQuotesGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

**[]*string**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListCharactersCharactersGet

> PaginatedResponseCharacter ListCharactersCharactersGet(ctx).Role(role).TeamId(teamId).MinOptimism(minOptimism).Skip(skip).Limit(limit).Execute()

List all characters



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
	role := openapiclient.CharacterRole("coach") // CharacterRole | Filter by role (optional)
	teamId := "teamId_example" // string | Filter by team ID (optional)
	minOptimism := int32(56) // int32 | Minimum optimism score (optional)
	skip := int32(56) // int32 | Number of items to skip (offset) (optional) (default to 0)
	limit := int32(56) // int32 | Maximum number of items to return (max: 100) (optional) (default to 20)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CharactersAPI.ListCharactersCharactersGet(context.Background()).Role(role).TeamId(teamId).MinOptimism(minOptimism).Skip(skip).Limit(limit).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CharactersAPI.ListCharactersCharactersGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListCharactersCharactersGet`: PaginatedResponseCharacter
	fmt.Fprintf(os.Stdout, "Response from `CharactersAPI.ListCharactersCharactersGet`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListCharactersCharactersGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **role** | [**CharacterRole**](CharacterRole.md) | Filter by role | 
 **teamId** | **string** | Filter by team ID | 
 **minOptimism** | **int32** | Minimum optimism score | 
 **skip** | **int32** | Number of items to skip (offset) | [default to 0]
 **limit** | **int32** | Maximum number of items to return (max: 100) | [default to 20]

### Return type

[**PaginatedResponseCharacter**](PaginatedResponseCharacter.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateCharacterCharactersCharacterIdPatch

> Character UpdateCharacterCharactersCharacterIdPatch(ctx, characterId).CharacterUpdate(characterUpdate).Execute()

Update a character



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
	characterId := "characterId_example" // string | 
	characterUpdate := *openapiclient.NewCharacterUpdate() // CharacterUpdate | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CharactersAPI.UpdateCharacterCharactersCharacterIdPatch(context.Background(), characterId).CharacterUpdate(characterUpdate).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CharactersAPI.UpdateCharacterCharactersCharacterIdPatch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateCharacterCharactersCharacterIdPatch`: Character
	fmt.Fprintf(os.Stdout, "Response from `CharactersAPI.UpdateCharacterCharactersCharacterIdPatch`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**characterId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateCharacterCharactersCharacterIdPatchRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **characterUpdate** | [**CharacterUpdate**](CharacterUpdate.md) |  | 

### Return type

[**Character**](Character.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

