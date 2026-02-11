# QuotesApi

All URIs are relative to *https://believe.cjav.dev*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
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
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.QuotesApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://believe.cjav.dev");
    
    // Configure HTTP bearer authorization: HTTPBearer
    HttpBearerAuth HTTPBearer = (HttpBearerAuth) defaultClient.getAuthentication("HTTPBearer");
    HTTPBearer.setBearerToken("BEARER TOKEN");

    QuotesApi apiInstance = new QuotesApi(defaultClient);
    QuoteCreate quoteCreate = new QuoteCreate(); // QuoteCreate | 
    try {
      Quote result = apiInstance.createQuoteQuotesPost(quoteCreate);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling QuotesApi#createQuoteQuotesPost");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **quoteCreate** | [**QuoteCreate**](QuoteCreate.md)|  | |

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

<a id="deleteQuoteQuotesQuoteIdDelete"></a>
# **deleteQuoteQuotesQuoteIdDelete**
> deleteQuoteQuotesQuoteIdDelete(quoteId)

Delete a quote

Remove a quote from the collection.

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.QuotesApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://believe.cjav.dev");
    
    // Configure HTTP bearer authorization: HTTPBearer
    HttpBearerAuth HTTPBearer = (HttpBearerAuth) defaultClient.getAuthentication("HTTPBearer");
    HTTPBearer.setBearerToken("BEARER TOKEN");

    QuotesApi apiInstance = new QuotesApi(defaultClient);
    String quoteId = "quoteId_example"; // String | 
    try {
      apiInstance.deleteQuoteQuotesQuoteIdDelete(quoteId);
    } catch (ApiException e) {
      System.err.println("Exception when calling QuotesApi#deleteQuoteQuotesQuoteIdDelete");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **quoteId** | **String**|  | |

### Return type

null (empty response body)

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

<a id="getCharacterQuotesQuotesCharactersCharacterIdGet"></a>
# **getCharacterQuotesQuotesCharactersCharacterIdGet**
> PaginatedResponseQuote getCharacterQuotesQuotesCharactersCharacterIdGet(characterId, skip, limit)

Get all quotes by a character

Get a paginated list of quotes from a specific character.

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.QuotesApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://believe.cjav.dev");
    
    // Configure HTTP bearer authorization: HTTPBearer
    HttpBearerAuth HTTPBearer = (HttpBearerAuth) defaultClient.getAuthentication("HTTPBearer");
    HTTPBearer.setBearerToken("BEARER TOKEN");

    QuotesApi apiInstance = new QuotesApi(defaultClient);
    String characterId = "characterId_example"; // String | 
    Integer skip = 0; // Integer | Number of items to skip (offset)
    Integer limit = 20; // Integer | Maximum number of items to return (max: 100)
    try {
      PaginatedResponseQuote result = apiInstance.getCharacterQuotesQuotesCharactersCharacterIdGet(characterId, skip, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling QuotesApi#getCharacterQuotesQuotesCharactersCharacterIdGet");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **characterId** | **String**|  | |
| **skip** | **Integer**| Number of items to skip (offset) | [optional] [default to 0] |
| **limit** | **Integer**| Maximum number of items to return (max: 100) | [optional] [default to 20] |

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

<a id="getQuoteQuotesQuoteIdGet"></a>
# **getQuoteQuotesQuoteIdGet**
> Quote getQuoteQuotesQuoteIdGet(quoteId)

Get a quote by ID

Retrieve a specific quote by its ID.

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.QuotesApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://believe.cjav.dev");
    
    // Configure HTTP bearer authorization: HTTPBearer
    HttpBearerAuth HTTPBearer = (HttpBearerAuth) defaultClient.getAuthentication("HTTPBearer");
    HTTPBearer.setBearerToken("BEARER TOKEN");

    QuotesApi apiInstance = new QuotesApi(defaultClient);
    String quoteId = "quoteId_example"; // String | 
    try {
      Quote result = apiInstance.getQuoteQuotesQuoteIdGet(quoteId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling QuotesApi#getQuoteQuotesQuoteIdGet");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **quoteId** | **String**|  | |

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

<a id="getQuotesByThemeQuotesThemesThemeGet"></a>
# **getQuotesByThemeQuotesThemesThemeGet**
> PaginatedResponseQuote getQuotesByThemeQuotesThemesThemeGet(theme, skip, limit)

Get quotes by theme

Get a paginated list of quotes related to a specific theme.

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.QuotesApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://believe.cjav.dev");
    
    // Configure HTTP bearer authorization: HTTPBearer
    HttpBearerAuth HTTPBearer = (HttpBearerAuth) defaultClient.getAuthentication("HTTPBearer");
    HTTPBearer.setBearerToken("BEARER TOKEN");

    QuotesApi apiInstance = new QuotesApi(defaultClient);
    QuoteTheme theme = QuoteTheme.fromValue("belief"); // QuoteTheme | 
    Integer skip = 0; // Integer | Number of items to skip (offset)
    Integer limit = 20; // Integer | Maximum number of items to return (max: 100)
    try {
      PaginatedResponseQuote result = apiInstance.getQuotesByThemeQuotesThemesThemeGet(theme, skip, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling QuotesApi#getQuotesByThemeQuotesThemesThemeGet");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **theme** | [**QuoteTheme**](.md)|  | [enum: belief, teamwork, curiosity, kindness, resilience, vulnerability, growth, humor, wisdom, leadership, love, forgiveness, philosophy, romance, cultural-pride, cultural-differences, antagonism, celebration, identity, isolation, power, sacrifice, standards, confidence, conflict, honesty, integrity] |
| **skip** | **Integer**| Number of items to skip (offset) | [optional] [default to 0] |
| **limit** | **Integer**| Maximum number of items to return (max: 100) | [optional] [default to 20] |

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

<a id="getRandomQuoteQuotesRandomGet"></a>
# **getRandomQuoteQuotesRandomGet**
> Quote getRandomQuoteQuotesRandomGet(characterId, theme, inspirational)

Get a random quote

Get a random Ted Lasso quote, optionally filtered.

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.QuotesApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://believe.cjav.dev");
    
    // Configure HTTP bearer authorization: HTTPBearer
    HttpBearerAuth HTTPBearer = (HttpBearerAuth) defaultClient.getAuthentication("HTTPBearer");
    HTTPBearer.setBearerToken("BEARER TOKEN");

    QuotesApi apiInstance = new QuotesApi(defaultClient);
    String characterId = "characterId_example"; // String | Filter by character
    QuoteTheme theme = QuoteTheme.fromValue("belief"); // QuoteTheme | Filter by theme
    Boolean inspirational = true; // Boolean | Filter inspirational quotes
    try {
      Quote result = apiInstance.getRandomQuoteQuotesRandomGet(characterId, theme, inspirational);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling QuotesApi#getRandomQuoteQuotesRandomGet");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **characterId** | **String**| Filter by character | [optional] |
| **theme** | [**QuoteTheme**](.md)| Filter by theme | [optional] [enum: belief, teamwork, curiosity, kindness, resilience, vulnerability, growth, humor, wisdom, leadership, love, forgiveness, philosophy, romance, cultural-pride, cultural-differences, antagonism, celebration, identity, isolation, power, sacrifice, standards, confidence, conflict, honesty, integrity] |
| **inspirational** | **Boolean**| Filter inspirational quotes | [optional] |

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

<a id="listQuotesQuotesGet"></a>
# **listQuotesQuotesGet**
> PaginatedResponseQuote listQuotesQuotesGet(characterId, theme, momentType, inspirational, funny, skip, limit)

List all quotes

Get a paginated list of all memorable Ted Lasso quotes with optional filtering.

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.QuotesApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://believe.cjav.dev");
    
    // Configure HTTP bearer authorization: HTTPBearer
    HttpBearerAuth HTTPBearer = (HttpBearerAuth) defaultClient.getAuthentication("HTTPBearer");
    HTTPBearer.setBearerToken("BEARER TOKEN");

    QuotesApi apiInstance = new QuotesApi(defaultClient);
    String characterId = "characterId_example"; // String | Filter by character
    QuoteTheme theme = QuoteTheme.fromValue("belief"); // QuoteTheme | Filter by theme
    QuoteMoment momentType = QuoteMoment.fromValue("halftime_speech"); // QuoteMoment | Filter by moment type
    Boolean inspirational = true; // Boolean | Filter inspirational quotes
    Boolean funny = true; // Boolean | Filter funny quotes
    Integer skip = 0; // Integer | Number of items to skip (offset)
    Integer limit = 20; // Integer | Maximum number of items to return (max: 100)
    try {
      PaginatedResponseQuote result = apiInstance.listQuotesQuotesGet(characterId, theme, momentType, inspirational, funny, skip, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling QuotesApi#listQuotesQuotesGet");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **characterId** | **String**| Filter by character | [optional] |
| **theme** | [**QuoteTheme**](.md)| Filter by theme | [optional] [enum: belief, teamwork, curiosity, kindness, resilience, vulnerability, growth, humor, wisdom, leadership, love, forgiveness, philosophy, romance, cultural-pride, cultural-differences, antagonism, celebration, identity, isolation, power, sacrifice, standards, confidence, conflict, honesty, integrity] |
| **momentType** | [**QuoteMoment**](.md)| Filter by moment type | [optional] [enum: halftime_speech, press_conference, locker_room, training, biscuits_with_boss, pub, one_on_one, celebration, crisis, casual, confrontation] |
| **inspirational** | **Boolean**| Filter inspirational quotes | [optional] |
| **funny** | **Boolean**| Filter funny quotes | [optional] |
| **skip** | **Integer**| Number of items to skip (offset) | [optional] [default to 0] |
| **limit** | **Integer**| Maximum number of items to return (max: 100) | [optional] [default to 20] |

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

<a id="updateQuoteQuotesQuoteIdPatch"></a>
# **updateQuoteQuotesQuoteIdPatch**
> Quote updateQuoteQuotesQuoteIdPatch(quoteId, quoteUpdate)

Update a quote

Update specific fields of an existing quote.

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.QuotesApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://believe.cjav.dev");
    
    // Configure HTTP bearer authorization: HTTPBearer
    HttpBearerAuth HTTPBearer = (HttpBearerAuth) defaultClient.getAuthentication("HTTPBearer");
    HTTPBearer.setBearerToken("BEARER TOKEN");

    QuotesApi apiInstance = new QuotesApi(defaultClient);
    String quoteId = "quoteId_example"; // String | 
    QuoteUpdate quoteUpdate = new QuoteUpdate(); // QuoteUpdate | 
    try {
      Quote result = apiInstance.updateQuoteQuotesQuoteIdPatch(quoteId, quoteUpdate);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling QuotesApi#updateQuoteQuotesQuoteIdPatch");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **quoteId** | **String**|  | |
| **quoteUpdate** | [**QuoteUpdate**](QuoteUpdate.md)|  | |

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

