# QuotesApi

All URIs are relative to *https://believe.cjav.dev*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createQuoteQuotesPost**](QuotesApi.md#createquotequotespost) | **POST** /quotes | Create a new quote |
| [**deleteQuoteQuotesQuoteIdDelete**](QuotesApi.md#deletequotequotesquoteiddelete) | **DELETE** /quotes/{quote_id} | Delete a quote |
| [**getCharacterQuotesQuotesCharactersCharacterIdGet**](QuotesApi.md#getcharacterquotesquotescharacterscharacteridget) | **GET** /quotes/characters/{character_id} | Get all quotes by a character |
| [**getQuoteQuotesQuoteIdGet**](QuotesApi.md#getquotequotesquoteidget) | **GET** /quotes/{quote_id} | Get a quote by ID |
| [**getQuotesByThemeQuotesThemesThemeGet**](QuotesApi.md#getquotesbythemequotesthemesthemeget) | **GET** /quotes/themes/{theme} | Get quotes by theme |
| [**getRandomQuoteQuotesRandomGet**](QuotesApi.md#getrandomquotequotesrandomget) | **GET** /quotes/random | Get a random quote |
| [**listQuotesQuotesGet**](QuotesApi.md#listquotesquotesget) | **GET** /quotes | List all quotes |
| [**updateQuoteQuotesQuoteIdPatch**](QuotesApi.md#updatequotequotesquoteidpatch) | **PATCH** /quotes/{quote_id} | Update a quote |



## createQuoteQuotesPost

> Quote createQuoteQuotesPost(quoteCreate)

Create a new quote

Add a new memorable quote to the collection.

### Example

```ts
import {
  Configuration,
  QuotesApi,
} from '';
import type { CreateQuoteQuotesPostRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new QuotesApi(config);

  const body = {
    // QuoteCreate
    quoteCreate: ...,
  } satisfies CreateQuoteQuotesPostRequest;

  try {
    const data = await api.createQuoteQuotesPost(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **quoteCreate** | [QuoteCreate](QuoteCreate.md) |  | |

### Return type

[**Quote**](Quote.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Quote created successfully |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deleteQuoteQuotesQuoteIdDelete

> deleteQuoteQuotesQuoteIdDelete(quoteId)

Delete a quote

Remove a quote from the collection.

### Example

```ts
import {
  Configuration,
  QuotesApi,
} from '';
import type { DeleteQuoteQuotesQuoteIdDeleteRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new QuotesApi(config);

  const body = {
    // string
    quoteId: quoteId_example,
  } satisfies DeleteQuoteQuotesQuoteIdDeleteRequest;

  try {
    const data = await api.deleteQuoteQuotesQuoteIdDelete(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **quoteId** | `string` |  | [Defaults to `undefined`] |

### Return type

`void` (Empty response body)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | Quote deleted successfully |  -  |
| **404** | Quote not found |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getCharacterQuotesQuotesCharactersCharacterIdGet

> PaginatedResponseQuote getCharacterQuotesQuotesCharactersCharacterIdGet(characterId, skip, limit)

Get all quotes by a character

Get a paginated list of quotes from a specific character.

### Example

```ts
import {
  Configuration,
  QuotesApi,
} from '';
import type { GetCharacterQuotesQuotesCharactersCharacterIdGetRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new QuotesApi(config);

  const body = {
    // string
    characterId: characterId_example,
    // number | Number of items to skip (offset) (optional)
    skip: 56,
    // number | Maximum number of items to return (max: 100) (optional)
    limit: 56,
  } satisfies GetCharacterQuotesQuotesCharactersCharacterIdGetRequest;

  try {
    const data = await api.getCharacterQuotesQuotesCharactersCharacterIdGet(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **characterId** | `string` |  | [Defaults to `undefined`] |
| **skip** | `number` | Number of items to skip (offset) | [Optional] [Defaults to `0`] |
| **limit** | `number` | Maximum number of items to return (max: 100) | [Optional] [Defaults to `20`] |

### Return type

[**PaginatedResponseQuote**](PaginatedResponseQuote.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Paginated list of quotes from the character |  -  |
| **404** | No quotes found for character |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getQuoteQuotesQuoteIdGet

> Quote getQuoteQuotesQuoteIdGet(quoteId)

Get a quote by ID

Retrieve a specific quote by its ID.

### Example

```ts
import {
  Configuration,
  QuotesApi,
} from '';
import type { GetQuoteQuotesQuoteIdGetRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new QuotesApi(config);

  const body = {
    // string
    quoteId: quoteId_example,
  } satisfies GetQuoteQuotesQuoteIdGetRequest;

  try {
    const data = await api.getQuoteQuotesQuoteIdGet(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **quoteId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**Quote**](Quote.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Quote details |  -  |
| **404** | Quote not found |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getQuotesByThemeQuotesThemesThemeGet

> PaginatedResponseQuote getQuotesByThemeQuotesThemesThemeGet(theme, skip, limit)

Get quotes by theme

Get a paginated list of quotes related to a specific theme.

### Example

```ts
import {
  Configuration,
  QuotesApi,
} from '';
import type { GetQuotesByThemeQuotesThemesThemeGetRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new QuotesApi(config);

  const body = {
    // QuoteTheme
    theme: ...,
    // number | Number of items to skip (offset) (optional)
    skip: 56,
    // number | Maximum number of items to return (max: 100) (optional)
    limit: 56,
  } satisfies GetQuotesByThemeQuotesThemesThemeGetRequest;

  try {
    const data = await api.getQuotesByThemeQuotesThemesThemeGet(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **theme** | `QuoteTheme` |  | [Defaults to `undefined`] [Enum: belief, teamwork, curiosity, kindness, resilience, vulnerability, growth, humor, wisdom, leadership, love, forgiveness, philosophy, romance, cultural-pride, cultural-differences, antagonism, celebration, identity, isolation, power, sacrifice, standards, confidence, conflict, honesty, integrity] |
| **skip** | `number` | Number of items to skip (offset) | [Optional] [Defaults to `0`] |
| **limit** | `number` | Maximum number of items to return (max: 100) | [Optional] [Defaults to `20`] |

### Return type

[**PaginatedResponseQuote**](PaginatedResponseQuote.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Paginated list of quotes for the theme |  -  |
| **404** | No quotes found for theme |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getRandomQuoteQuotesRandomGet

> Quote getRandomQuoteQuotesRandomGet(characterId, theme, inspirational)

Get a random quote

Get a random Ted Lasso quote, optionally filtered.

### Example

```ts
import {
  Configuration,
  QuotesApi,
} from '';
import type { GetRandomQuoteQuotesRandomGetRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new QuotesApi(config);

  const body = {
    // string | Filter by character (optional)
    characterId: characterId_example,
    // QuoteTheme | Filter by theme (optional)
    theme: ...,
    // boolean | Filter inspirational quotes (optional)
    inspirational: true,
  } satisfies GetRandomQuoteQuotesRandomGetRequest;

  try {
    const data = await api.getRandomQuoteQuotesRandomGet(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **characterId** | `string` | Filter by character | [Optional] [Defaults to `undefined`] |
| **theme** | `QuoteTheme` | Filter by theme | [Optional] [Defaults to `undefined`] [Enum: belief, teamwork, curiosity, kindness, resilience, vulnerability, growth, humor, wisdom, leadership, love, forgiveness, philosophy, romance, cultural-pride, cultural-differences, antagonism, celebration, identity, isolation, power, sacrifice, standards, confidence, conflict, honesty, integrity] |
| **inspirational** | `boolean` | Filter inspirational quotes | [Optional] [Defaults to `undefined`] |

### Return type

[**Quote**](Quote.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | A random quote |  -  |
| **404** | No quotes found matching criteria |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## listQuotesQuotesGet

> PaginatedResponseQuote listQuotesQuotesGet(characterId, theme, momentType, inspirational, funny, skip, limit)

List all quotes

Get a paginated list of all memorable Ted Lasso quotes with optional filtering.

### Example

```ts
import {
  Configuration,
  QuotesApi,
} from '';
import type { ListQuotesQuotesGetRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new QuotesApi(config);

  const body = {
    // string | Filter by character (optional)
    characterId: characterId_example,
    // QuoteTheme | Filter by theme (optional)
    theme: ...,
    // QuoteMoment | Filter by moment type (optional)
    momentType: ...,
    // boolean | Filter inspirational quotes (optional)
    inspirational: true,
    // boolean | Filter funny quotes (optional)
    funny: true,
    // number | Number of items to skip (offset) (optional)
    skip: 56,
    // number | Maximum number of items to return (max: 100) (optional)
    limit: 56,
  } satisfies ListQuotesQuotesGetRequest;

  try {
    const data = await api.listQuotesQuotesGet(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **characterId** | `string` | Filter by character | [Optional] [Defaults to `undefined`] |
| **theme** | `QuoteTheme` | Filter by theme | [Optional] [Defaults to `undefined`] [Enum: belief, teamwork, curiosity, kindness, resilience, vulnerability, growth, humor, wisdom, leadership, love, forgiveness, philosophy, romance, cultural-pride, cultural-differences, antagonism, celebration, identity, isolation, power, sacrifice, standards, confidence, conflict, honesty, integrity] |
| **momentType** | `QuoteMoment` | Filter by moment type | [Optional] [Defaults to `undefined`] [Enum: halftime_speech, press_conference, locker_room, training, biscuits_with_boss, pub, one_on_one, celebration, crisis, casual, confrontation] |
| **inspirational** | `boolean` | Filter inspirational quotes | [Optional] [Defaults to `undefined`] |
| **funny** | `boolean` | Filter funny quotes | [Optional] [Defaults to `undefined`] |
| **skip** | `number` | Number of items to skip (offset) | [Optional] [Defaults to `0`] |
| **limit** | `number` | Maximum number of items to return (max: 100) | [Optional] [Defaults to `20`] |

### Return type

[**PaginatedResponseQuote**](PaginatedResponseQuote.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Paginated list of quotes |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## updateQuoteQuotesQuoteIdPatch

> Quote updateQuoteQuotesQuoteIdPatch(quoteId, quoteUpdate)

Update a quote

Update specific fields of an existing quote.

### Example

```ts
import {
  Configuration,
  QuotesApi,
} from '';
import type { UpdateQuoteQuotesQuoteIdPatchRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new QuotesApi(config);

  const body = {
    // string
    quoteId: quoteId_example,
    // QuoteUpdate
    quoteUpdate: ...,
  } satisfies UpdateQuoteQuotesQuoteIdPatchRequest;

  try {
    const data = await api.updateQuoteQuotesQuoteIdPatch(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **quoteId** | `string` |  | [Defaults to `undefined`] |
| **quoteUpdate** | [QuoteUpdate](QuoteUpdate.md) |  | |

### Return type

[**Quote**](Quote.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Quote updated successfully |  -  |
| **404** | Quote not found |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

