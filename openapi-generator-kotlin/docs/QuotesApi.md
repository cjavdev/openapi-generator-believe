# QuotesApi

All URIs are relative to *https://believe.cjav.dev*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createQuoteQuotesPost**](QuotesApi.md#createQuoteQuotesPost) | **POST** /quotes | Create a new quote |
| [**deleteQuoteQuotesQuoteIdDelete**](QuotesApi.md#deleteQuoteQuotesQuoteIdDelete) | **DELETE** /quotes/{quote_id} | Delete a quote |
| [**getCharacterQuotesQuotesCharactersCharacterIdGet**](QuotesApi.md#getCharacterQuotesQuotesCharactersCharacterIdGet) | **GET** /quotes/characters/{character_id} | Get all quotes by a character |
| [**getQuoteQuotesQuoteIdGet**](QuotesApi.md#getQuoteQuotesQuoteIdGet) | **GET** /quotes/{quote_id} | Get a quote by ID |
| [**getQuotesByThemeQuotesThemesThemeGet**](QuotesApi.md#getQuotesByThemeQuotesThemesThemeGet) | **GET** /quotes/themes/{theme} | Get quotes by theme |
| [**getRandomQuoteQuotesRandomGet**](QuotesApi.md#getRandomQuoteQuotesRandomGet) | **GET** /quotes/random | Get a random quote |
| [**listQuotesQuotesGet**](QuotesApi.md#listQuotesQuotesGet) | **GET** /quotes | List all quotes |
| [**updateQuoteQuotesQuoteIdPatch**](QuotesApi.md#updateQuoteQuotesQuoteIdPatch) | **PATCH** /quotes/{quote_id} | Update a quote |


<a id="createQuoteQuotesPost"></a>
# **createQuoteQuotesPost**
> Quote createQuoteQuotesPost(quoteCreate)

Create a new quote

Add a new memorable quote to the collection.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = QuotesApi()
val quoteCreate : QuoteCreate =  // QuoteCreate | 
try {
    val result : Quote = apiInstance.createQuoteQuotesPost(quoteCreate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling QuotesApi#createQuoteQuotesPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling QuotesApi#createQuoteQuotesPost")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **quoteCreate** | [**QuoteCreate**](QuoteCreate.md)|  | |

### Return type

[**Quote**](Quote.md)

### Authorization


Configure HTTPBearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="deleteQuoteQuotesQuoteIdDelete"></a>
# **deleteQuoteQuotesQuoteIdDelete**
> deleteQuoteQuotesQuoteIdDelete(quoteId)

Delete a quote

Remove a quote from the collection.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = QuotesApi()
val quoteId : kotlin.String = quoteId_example // kotlin.String | 
try {
    apiInstance.deleteQuoteQuotesQuoteIdDelete(quoteId)
} catch (e: ClientException) {
    println("4xx response calling QuotesApi#deleteQuoteQuotesQuoteIdDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling QuotesApi#deleteQuoteQuotesQuoteIdDelete")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **quoteId** | **kotlin.String**|  | |

### Return type

null (empty response body)

### Authorization


Configure HTTPBearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="getCharacterQuotesQuotesCharactersCharacterIdGet"></a>
# **getCharacterQuotesQuotesCharactersCharacterIdGet**
> PaginatedResponseQuote getCharacterQuotesQuotesCharactersCharacterIdGet(characterId, skip, limit)

Get all quotes by a character

Get a paginated list of quotes from a specific character.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = QuotesApi()
val characterId : kotlin.String = characterId_example // kotlin.String | 
val skip : kotlin.Int = 56 // kotlin.Int | Number of items to skip (offset)
val limit : kotlin.Int = 56 // kotlin.Int | Maximum number of items to return (max: 100)
try {
    val result : PaginatedResponseQuote = apiInstance.getCharacterQuotesQuotesCharactersCharacterIdGet(characterId, skip, limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling QuotesApi#getCharacterQuotesQuotesCharactersCharacterIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling QuotesApi#getCharacterQuotesQuotesCharactersCharacterIdGet")
    e.printStackTrace()
}
```

### Parameters
| **characterId** | **kotlin.String**|  | |
| **skip** | **kotlin.Int**| Number of items to skip (offset) | [optional] [default to 0] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.Int**| Maximum number of items to return (max: 100) | [optional] [default to 20] |

### Return type

[**PaginatedResponseQuote**](PaginatedResponseQuote.md)

### Authorization


Configure HTTPBearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="getQuoteQuotesQuoteIdGet"></a>
# **getQuoteQuotesQuoteIdGet**
> Quote getQuoteQuotesQuoteIdGet(quoteId)

Get a quote by ID

Retrieve a specific quote by its ID.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = QuotesApi()
val quoteId : kotlin.String = quoteId_example // kotlin.String | 
try {
    val result : Quote = apiInstance.getQuoteQuotesQuoteIdGet(quoteId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling QuotesApi#getQuoteQuotesQuoteIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling QuotesApi#getQuoteQuotesQuoteIdGet")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **quoteId** | **kotlin.String**|  | |

### Return type

[**Quote**](Quote.md)

### Authorization


Configure HTTPBearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="getQuotesByThemeQuotesThemesThemeGet"></a>
# **getQuotesByThemeQuotesThemesThemeGet**
> PaginatedResponseQuote getQuotesByThemeQuotesThemesThemeGet(theme, skip, limit)

Get quotes by theme

Get a paginated list of quotes related to a specific theme.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = QuotesApi()
val theme : QuoteTheme =  // QuoteTheme | 
val skip : kotlin.Int = 56 // kotlin.Int | Number of items to skip (offset)
val limit : kotlin.Int = 56 // kotlin.Int | Maximum number of items to return (max: 100)
try {
    val result : PaginatedResponseQuote = apiInstance.getQuotesByThemeQuotesThemesThemeGet(theme, skip, limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling QuotesApi#getQuotesByThemeQuotesThemesThemeGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling QuotesApi#getQuotesByThemeQuotesThemesThemeGet")
    e.printStackTrace()
}
```

### Parameters
| **theme** | [**QuoteTheme**](.md)|  | [enum: belief, teamwork, curiosity, kindness, resilience, vulnerability, growth, humor, wisdom, leadership, love, forgiveness, philosophy, romance, cultural-pride, cultural-differences, antagonism, celebration, identity, isolation, power, sacrifice, standards, confidence, conflict, honesty, integrity] |
| **skip** | **kotlin.Int**| Number of items to skip (offset) | [optional] [default to 0] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.Int**| Maximum number of items to return (max: 100) | [optional] [default to 20] |

### Return type

[**PaginatedResponseQuote**](PaginatedResponseQuote.md)

### Authorization


Configure HTTPBearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="getRandomQuoteQuotesRandomGet"></a>
# **getRandomQuoteQuotesRandomGet**
> Quote getRandomQuoteQuotesRandomGet(characterId, theme, inspirational)

Get a random quote

Get a random Ted Lasso quote, optionally filtered.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = QuotesApi()
val characterId : kotlin.String = characterId_example // kotlin.String | Filter by character
val theme : QuoteTheme =  // QuoteTheme | Filter by theme
val inspirational : kotlin.Boolean = true // kotlin.Boolean | Filter inspirational quotes
try {
    val result : Quote = apiInstance.getRandomQuoteQuotesRandomGet(characterId, theme, inspirational)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling QuotesApi#getRandomQuoteQuotesRandomGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling QuotesApi#getRandomQuoteQuotesRandomGet")
    e.printStackTrace()
}
```

### Parameters
| **characterId** | **kotlin.String**| Filter by character | [optional] |
| **theme** | [**QuoteTheme**](.md)| Filter by theme | [optional] [enum: belief, teamwork, curiosity, kindness, resilience, vulnerability, growth, humor, wisdom, leadership, love, forgiveness, philosophy, romance, cultural-pride, cultural-differences, antagonism, celebration, identity, isolation, power, sacrifice, standards, confidence, conflict, honesty, integrity] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **inspirational** | **kotlin.Boolean**| Filter inspirational quotes | [optional] |

### Return type

[**Quote**](Quote.md)

### Authorization


Configure HTTPBearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="listQuotesQuotesGet"></a>
# **listQuotesQuotesGet**
> PaginatedResponseQuote listQuotesQuotesGet(characterId, theme, momentType, inspirational, funny, skip, limit)

List all quotes

Get a paginated list of all memorable Ted Lasso quotes with optional filtering.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = QuotesApi()
val characterId : kotlin.String = characterId_example // kotlin.String | Filter by character
val theme : QuoteTheme =  // QuoteTheme | Filter by theme
val momentType : QuoteMoment =  // QuoteMoment | Filter by moment type
val inspirational : kotlin.Boolean = true // kotlin.Boolean | Filter inspirational quotes
val funny : kotlin.Boolean = true // kotlin.Boolean | Filter funny quotes
val skip : kotlin.Int = 56 // kotlin.Int | Number of items to skip (offset)
val limit : kotlin.Int = 56 // kotlin.Int | Maximum number of items to return (max: 100)
try {
    val result : PaginatedResponseQuote = apiInstance.listQuotesQuotesGet(characterId, theme, momentType, inspirational, funny, skip, limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling QuotesApi#listQuotesQuotesGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling QuotesApi#listQuotesQuotesGet")
    e.printStackTrace()
}
```

### Parameters
| **characterId** | **kotlin.String**| Filter by character | [optional] |
| **theme** | [**QuoteTheme**](.md)| Filter by theme | [optional] [enum: belief, teamwork, curiosity, kindness, resilience, vulnerability, growth, humor, wisdom, leadership, love, forgiveness, philosophy, romance, cultural-pride, cultural-differences, antagonism, celebration, identity, isolation, power, sacrifice, standards, confidence, conflict, honesty, integrity] |
| **momentType** | [**QuoteMoment**](.md)| Filter by moment type | [optional] [enum: halftime_speech, press_conference, locker_room, training, biscuits_with_boss, pub, one_on_one, celebration, crisis, casual, confrontation] |
| **inspirational** | **kotlin.Boolean**| Filter inspirational quotes | [optional] |
| **funny** | **kotlin.Boolean**| Filter funny quotes | [optional] |
| **skip** | **kotlin.Int**| Number of items to skip (offset) | [optional] [default to 0] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.Int**| Maximum number of items to return (max: 100) | [optional] [default to 20] |

### Return type

[**PaginatedResponseQuote**](PaginatedResponseQuote.md)

### Authorization


Configure HTTPBearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="updateQuoteQuotesQuoteIdPatch"></a>
# **updateQuoteQuotesQuoteIdPatch**
> Quote updateQuoteQuotesQuoteIdPatch(quoteId, quoteUpdate)

Update a quote

Update specific fields of an existing quote.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = QuotesApi()
val quoteId : kotlin.String = quoteId_example // kotlin.String | 
val quoteUpdate : QuoteUpdate =  // QuoteUpdate | 
try {
    val result : Quote = apiInstance.updateQuoteQuotesQuoteIdPatch(quoteId, quoteUpdate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling QuotesApi#updateQuoteQuotesQuoteIdPatch")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling QuotesApi#updateQuoteQuotesQuoteIdPatch")
    e.printStackTrace()
}
```

### Parameters
| **quoteId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **quoteUpdate** | [**QuoteUpdate**](QuoteUpdate.md)|  | |

### Return type

[**Quote**](Quote.md)

### Authorization


Configure HTTPBearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

