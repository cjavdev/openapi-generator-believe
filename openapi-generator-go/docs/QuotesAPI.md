# \QuotesAPI

All URIs are relative to *https://believe.cjav.dev*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateQuoteQuotesPost**](QuotesAPI.md#CreateQuoteQuotesPost) | **Post** /quotes | Create a new quote
[**DeleteQuoteQuotesQuoteIdDelete**](QuotesAPI.md#DeleteQuoteQuotesQuoteIdDelete) | **Delete** /quotes/{quote_id} | Delete a quote
[**GetCharacterQuotesQuotesCharactersCharacterIdGet**](QuotesAPI.md#GetCharacterQuotesQuotesCharactersCharacterIdGet) | **Get** /quotes/characters/{character_id} | Get all quotes by a character
[**GetQuoteQuotesQuoteIdGet**](QuotesAPI.md#GetQuoteQuotesQuoteIdGet) | **Get** /quotes/{quote_id} | Get a quote by ID
[**GetQuotesByThemeQuotesThemesThemeGet**](QuotesAPI.md#GetQuotesByThemeQuotesThemesThemeGet) | **Get** /quotes/themes/{theme} | Get quotes by theme
[**GetRandomQuoteQuotesRandomGet**](QuotesAPI.md#GetRandomQuoteQuotesRandomGet) | **Get** /quotes/random | Get a random quote
[**ListQuotesQuotesGet**](QuotesAPI.md#ListQuotesQuotesGet) | **Get** /quotes | List all quotes
[**UpdateQuoteQuotesQuoteIdPatch**](QuotesAPI.md#UpdateQuoteQuotesQuoteIdPatch) | **Patch** /quotes/{quote_id} | Update a quote



## CreateQuoteQuotesPost

> Quote CreateQuoteQuotesPost(ctx).QuoteCreate(quoteCreate).Execute()

Create a new quote



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
	quoteCreate := *openapiclient.NewQuoteCreate("ted-lasso", "Ted playing darts against Rupert in the pub, explaining his philosophy", openapiclient.QuoteMoment("halftime_speech"), "Be curious, not judgmental.", openapiclient.QuoteTheme("belief")) // QuoteCreate | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.QuotesAPI.CreateQuoteQuotesPost(context.Background()).QuoteCreate(quoteCreate).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `QuotesAPI.CreateQuoteQuotesPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateQuoteQuotesPost`: Quote
	fmt.Fprintf(os.Stdout, "Response from `QuotesAPI.CreateQuoteQuotesPost`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateQuoteQuotesPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **quoteCreate** | [**QuoteCreate**](QuoteCreate.md) |  | 

### Return type

[**Quote**](Quote.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteQuoteQuotesQuoteIdDelete

> DeleteQuoteQuotesQuoteIdDelete(ctx, quoteId).Execute()

Delete a quote



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
	quoteId := "quoteId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.QuotesAPI.DeleteQuoteQuotesQuoteIdDelete(context.Background(), quoteId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `QuotesAPI.DeleteQuoteQuotesQuoteIdDelete``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**quoteId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteQuoteQuotesQuoteIdDeleteRequest struct via the builder pattern


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


## GetCharacterQuotesQuotesCharactersCharacterIdGet

> PaginatedResponseQuote GetCharacterQuotesQuotesCharactersCharacterIdGet(ctx, characterId).Skip(skip).Limit(limit).Execute()

Get all quotes by a character



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
	skip := int32(56) // int32 | Number of items to skip (offset) (optional) (default to 0)
	limit := int32(56) // int32 | Maximum number of items to return (max: 100) (optional) (default to 20)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.QuotesAPI.GetCharacterQuotesQuotesCharactersCharacterIdGet(context.Background(), characterId).Skip(skip).Limit(limit).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `QuotesAPI.GetCharacterQuotesQuotesCharactersCharacterIdGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetCharacterQuotesQuotesCharactersCharacterIdGet`: PaginatedResponseQuote
	fmt.Fprintf(os.Stdout, "Response from `QuotesAPI.GetCharacterQuotesQuotesCharactersCharacterIdGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**characterId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetCharacterQuotesQuotesCharactersCharacterIdGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **skip** | **int32** | Number of items to skip (offset) | [default to 0]
 **limit** | **int32** | Maximum number of items to return (max: 100) | [default to 20]

### Return type

[**PaginatedResponseQuote**](PaginatedResponseQuote.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetQuoteQuotesQuoteIdGet

> Quote GetQuoteQuotesQuoteIdGet(ctx, quoteId).Execute()

Get a quote by ID



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
	quoteId := "quoteId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.QuotesAPI.GetQuoteQuotesQuoteIdGet(context.Background(), quoteId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `QuotesAPI.GetQuoteQuotesQuoteIdGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetQuoteQuotesQuoteIdGet`: Quote
	fmt.Fprintf(os.Stdout, "Response from `QuotesAPI.GetQuoteQuotesQuoteIdGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**quoteId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetQuoteQuotesQuoteIdGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**Quote**](Quote.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetQuotesByThemeQuotesThemesThemeGet

> PaginatedResponseQuote GetQuotesByThemeQuotesThemesThemeGet(ctx, theme).Skip(skip).Limit(limit).Execute()

Get quotes by theme



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
	theme := openapiclient.QuoteTheme("belief") // QuoteTheme | 
	skip := int32(56) // int32 | Number of items to skip (offset) (optional) (default to 0)
	limit := int32(56) // int32 | Maximum number of items to return (max: 100) (optional) (default to 20)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.QuotesAPI.GetQuotesByThemeQuotesThemesThemeGet(context.Background(), theme).Skip(skip).Limit(limit).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `QuotesAPI.GetQuotesByThemeQuotesThemesThemeGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetQuotesByThemeQuotesThemesThemeGet`: PaginatedResponseQuote
	fmt.Fprintf(os.Stdout, "Response from `QuotesAPI.GetQuotesByThemeQuotesThemesThemeGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**theme** | [**QuoteTheme**](.md) |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetQuotesByThemeQuotesThemesThemeGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **skip** | **int32** | Number of items to skip (offset) | [default to 0]
 **limit** | **int32** | Maximum number of items to return (max: 100) | [default to 20]

### Return type

[**PaginatedResponseQuote**](PaginatedResponseQuote.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetRandomQuoteQuotesRandomGet

> Quote GetRandomQuoteQuotesRandomGet(ctx).CharacterId(characterId).Theme(theme).Inspirational(inspirational).Execute()

Get a random quote



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
	characterId := "characterId_example" // string | Filter by character (optional)
	theme := openapiclient.QuoteTheme("belief") // QuoteTheme | Filter by theme (optional)
	inspirational := true // bool | Filter inspirational quotes (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.QuotesAPI.GetRandomQuoteQuotesRandomGet(context.Background()).CharacterId(characterId).Theme(theme).Inspirational(inspirational).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `QuotesAPI.GetRandomQuoteQuotesRandomGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetRandomQuoteQuotesRandomGet`: Quote
	fmt.Fprintf(os.Stdout, "Response from `QuotesAPI.GetRandomQuoteQuotesRandomGet`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGetRandomQuoteQuotesRandomGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **characterId** | **string** | Filter by character | 
 **theme** | [**QuoteTheme**](QuoteTheme.md) | Filter by theme | 
 **inspirational** | **bool** | Filter inspirational quotes | 

### Return type

[**Quote**](Quote.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListQuotesQuotesGet

> PaginatedResponseQuote ListQuotesQuotesGet(ctx).CharacterId(characterId).Theme(theme).MomentType(momentType).Inspirational(inspirational).Funny(funny).Skip(skip).Limit(limit).Execute()

List all quotes



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
	characterId := "characterId_example" // string | Filter by character (optional)
	theme := openapiclient.QuoteTheme("belief") // QuoteTheme | Filter by theme (optional)
	momentType := openapiclient.QuoteMoment("halftime_speech") // QuoteMoment | Filter by moment type (optional)
	inspirational := true // bool | Filter inspirational quotes (optional)
	funny := true // bool | Filter funny quotes (optional)
	skip := int32(56) // int32 | Number of items to skip (offset) (optional) (default to 0)
	limit := int32(56) // int32 | Maximum number of items to return (max: 100) (optional) (default to 20)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.QuotesAPI.ListQuotesQuotesGet(context.Background()).CharacterId(characterId).Theme(theme).MomentType(momentType).Inspirational(inspirational).Funny(funny).Skip(skip).Limit(limit).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `QuotesAPI.ListQuotesQuotesGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListQuotesQuotesGet`: PaginatedResponseQuote
	fmt.Fprintf(os.Stdout, "Response from `QuotesAPI.ListQuotesQuotesGet`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListQuotesQuotesGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **characterId** | **string** | Filter by character | 
 **theme** | [**QuoteTheme**](QuoteTheme.md) | Filter by theme | 
 **momentType** | [**QuoteMoment**](QuoteMoment.md) | Filter by moment type | 
 **inspirational** | **bool** | Filter inspirational quotes | 
 **funny** | **bool** | Filter funny quotes | 
 **skip** | **int32** | Number of items to skip (offset) | [default to 0]
 **limit** | **int32** | Maximum number of items to return (max: 100) | [default to 20]

### Return type

[**PaginatedResponseQuote**](PaginatedResponseQuote.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateQuoteQuotesQuoteIdPatch

> Quote UpdateQuoteQuotesQuoteIdPatch(ctx, quoteId).QuoteUpdate(quoteUpdate).Execute()

Update a quote



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
	quoteId := "quoteId_example" // string | 
	quoteUpdate := *openapiclient.NewQuoteUpdate() // QuoteUpdate | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.QuotesAPI.UpdateQuoteQuotesQuoteIdPatch(context.Background(), quoteId).QuoteUpdate(quoteUpdate).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `QuotesAPI.UpdateQuoteQuotesQuoteIdPatch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateQuoteQuotesQuoteIdPatch`: Quote
	fmt.Fprintf(os.Stdout, "Response from `QuotesAPI.UpdateQuoteQuotesQuoteIdPatch`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**quoteId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateQuoteQuotesQuoteIdPatchRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **quoteUpdate** | [**QuoteUpdate**](QuoteUpdate.md) |  | 

### Return type

[**Quote**](Quote.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

