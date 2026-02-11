# Org.OpenAPITools.Api.QuotesApi

All URIs are relative to *https://believe.cjav.dev*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**CreateQuoteQuotesPost**](QuotesApi.md#createquotequotespost) | **POST** /quotes | Create a new quote |
| [**DeleteQuoteQuotesQuoteIdDelete**](QuotesApi.md#deletequotequotesquoteiddelete) | **DELETE** /quotes/{quote_id} | Delete a quote |
| [**GetCharacterQuotesQuotesCharactersCharacterIdGet**](QuotesApi.md#getcharacterquotesquotescharacterscharacteridget) | **GET** /quotes/characters/{character_id} | Get all quotes by a character |
| [**GetQuoteQuotesQuoteIdGet**](QuotesApi.md#getquotequotesquoteidget) | **GET** /quotes/{quote_id} | Get a quote by ID |
| [**GetQuotesByThemeQuotesThemesThemeGet**](QuotesApi.md#getquotesbythemequotesthemesthemeget) | **GET** /quotes/themes/{theme} | Get quotes by theme |
| [**GetRandomQuoteQuotesRandomGet**](QuotesApi.md#getrandomquotequotesrandomget) | **GET** /quotes/random | Get a random quote |
| [**ListQuotesQuotesGet**](QuotesApi.md#listquotesquotesget) | **GET** /quotes | List all quotes |
| [**UpdateQuoteQuotesQuoteIdPatch**](QuotesApi.md#updatequotequotesquoteidpatch) | **PATCH** /quotes/{quote_id} | Update a quote |

<a id="createquotequotespost"></a>
# **CreateQuoteQuotesPost**
> Quote CreateQuoteQuotesPost (QuoteCreate quoteCreate)

Create a new quote

Add a new memorable quote to the collection.


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **quoteCreate** | [**QuoteCreate**](QuoteCreate.md) |  |  |

### Return type

[**Quote**](Quote.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Quote created successfully |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="deletequotequotesquoteiddelete"></a>
# **DeleteQuoteQuotesQuoteIdDelete**
> void DeleteQuoteQuotesQuoteIdDelete (string quoteId)

Delete a quote

Remove a quote from the collection.


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **quoteId** | **string** |  |  |

### Return type

void (empty response body)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | Quote deleted successfully |  -  |
| **404** | Quote not found |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="getcharacterquotesquotescharacterscharacteridget"></a>
# **GetCharacterQuotesQuotesCharactersCharacterIdGet**
> PaginatedResponseQuote GetCharacterQuotesQuotesCharactersCharacterIdGet (string characterId, int skip = null, int limit = null)

Get all quotes by a character

Get a paginated list of quotes from a specific character.


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **characterId** | **string** |  |  |
| **skip** | **int** | Number of items to skip (offset) | [optional] [default to 0] |
| **limit** | **int** | Maximum number of items to return (max: 100) | [optional] [default to 20] |

### Return type

[**PaginatedResponseQuote**](PaginatedResponseQuote.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Paginated list of quotes from the character |  -  |
| **404** | No quotes found for character |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="getquotequotesquoteidget"></a>
# **GetQuoteQuotesQuoteIdGet**
> Quote GetQuoteQuotesQuoteIdGet (string quoteId)

Get a quote by ID

Retrieve a specific quote by its ID.


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **quoteId** | **string** |  |  |

### Return type

[**Quote**](Quote.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Quote details |  -  |
| **404** | Quote not found |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="getquotesbythemequotesthemesthemeget"></a>
# **GetQuotesByThemeQuotesThemesThemeGet**
> PaginatedResponseQuote GetQuotesByThemeQuotesThemesThemeGet (QuoteTheme theme, int skip = null, int limit = null)

Get quotes by theme

Get a paginated list of quotes related to a specific theme.


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **theme** | **QuoteTheme** |  |  |
| **skip** | **int** | Number of items to skip (offset) | [optional] [default to 0] |
| **limit** | **int** | Maximum number of items to return (max: 100) | [optional] [default to 20] |

### Return type

[**PaginatedResponseQuote**](PaginatedResponseQuote.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Paginated list of quotes for the theme |  -  |
| **404** | No quotes found for theme |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="getrandomquotequotesrandomget"></a>
# **GetRandomQuoteQuotesRandomGet**
> Quote GetRandomQuoteQuotesRandomGet (string characterId = null, QuoteTheme theme = null, bool inspirational = null)

Get a random quote

Get a random Ted Lasso quote, optionally filtered.


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **characterId** | **string** | Filter by character | [optional]  |
| **theme** | **QuoteTheme** | Filter by theme | [optional]  |
| **inspirational** | **bool** | Filter inspirational quotes | [optional]  |

### Return type

[**Quote**](Quote.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | A random quote |  -  |
| **404** | No quotes found matching criteria |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="listquotesquotesget"></a>
# **ListQuotesQuotesGet**
> PaginatedResponseQuote ListQuotesQuotesGet (string characterId = null, QuoteTheme theme = null, QuoteMoment momentType = null, bool inspirational = null, bool funny = null, int skip = null, int limit = null)

List all quotes

Get a paginated list of all memorable Ted Lasso quotes with optional filtering.


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **characterId** | **string** | Filter by character | [optional]  |
| **theme** | **QuoteTheme** | Filter by theme | [optional]  |
| **momentType** | **QuoteMoment** | Filter by moment type | [optional]  |
| **inspirational** | **bool** | Filter inspirational quotes | [optional]  |
| **funny** | **bool** | Filter funny quotes | [optional]  |
| **skip** | **int** | Number of items to skip (offset) | [optional] [default to 0] |
| **limit** | **int** | Maximum number of items to return (max: 100) | [optional] [default to 20] |

### Return type

[**PaginatedResponseQuote**](PaginatedResponseQuote.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Paginated list of quotes |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="updatequotequotesquoteidpatch"></a>
# **UpdateQuoteQuotesQuoteIdPatch**
> Quote UpdateQuoteQuotesQuoteIdPatch (string quoteId, QuoteUpdate quoteUpdate)

Update a quote

Update specific fields of an existing quote.


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **quoteId** | **string** |  |  |
| **quoteUpdate** | [**QuoteUpdate**](QuoteUpdate.md) |  |  |

### Return type

[**Quote**](Quote.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Quote updated successfully |  -  |
| **404** | Quote not found |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

