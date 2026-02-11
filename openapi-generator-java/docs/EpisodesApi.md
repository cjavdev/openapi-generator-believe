# EpisodesApi

All URIs are relative to *https://believe.cjav.dev*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createEpisodeEpisodesPost**](EpisodesApi.md#createEpisodeEpisodesPost) | **POST** /episodes | Create a new episode |
| [**deleteEpisodeEpisodesEpisodeIdDelete**](EpisodesApi.md#deleteEpisodeEpisodesEpisodeIdDelete) | **DELETE** /episodes/{episode_id} | Delete an episode |
| [**getEpisodeEpisodesEpisodeIdGet**](EpisodesApi.md#getEpisodeEpisodesEpisodeIdGet) | **GET** /episodes/{episode_id} | Get an episode by ID |
| [**getEpisodeWisdomEpisodesEpisodeIdWisdomGet**](EpisodesApi.md#getEpisodeWisdomEpisodesEpisodeIdWisdomGet) | **GET** /episodes/{episode_id}/wisdom | Get episode wisdom |
| [**getSeasonEpisodesEpisodesSeasonsSeasonNumberGet**](EpisodesApi.md#getSeasonEpisodesEpisodesSeasonsSeasonNumberGet) | **GET** /episodes/seasons/{season_number} | Get all episodes from a season |
| [**listEpisodesEpisodesGet**](EpisodesApi.md#listEpisodesEpisodesGet) | **GET** /episodes | List all episodes |
| [**updateEpisodeEpisodesEpisodeIdPatch**](EpisodesApi.md#updateEpisodeEpisodesEpisodeIdPatch) | **PATCH** /episodes/{episode_id} | Update an episode |


<a id="createEpisodeEpisodesPost"></a>
# **createEpisodeEpisodesPost**
> Episode createEpisodeEpisodesPost(episodeCreate)

Create a new episode

Add a new episode to the series.

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.EpisodesApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://believe.cjav.dev");
    
    // Configure HTTP bearer authorization: HTTPBearer
    HttpBearerAuth HTTPBearer = (HttpBearerAuth) defaultClient.getAuthentication("HTTPBearer");
    HTTPBearer.setBearerToken("BEARER TOKEN");

    EpisodesApi apiInstance = new EpisodesApi(defaultClient);
    EpisodeCreate episodeCreate = new EpisodeCreate(); // EpisodeCreate | 
    try {
      Episode result = apiInstance.createEpisodeEpisodesPost(episodeCreate);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling EpisodesApi#createEpisodeEpisodesPost");
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
| **episodeCreate** | [**EpisodeCreate**](EpisodeCreate.md)|  | |

### Return type

[**Episode**](Episode.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Episode created successfully |  -  |
| **409** | Episode already exists |  -  |
| **422** | Validation Error |  -  |

<a id="deleteEpisodeEpisodesEpisodeIdDelete"></a>
# **deleteEpisodeEpisodesEpisodeIdDelete**
> deleteEpisodeEpisodesEpisodeIdDelete(episodeId)

Delete an episode

Remove an episode from the database.

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.EpisodesApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://believe.cjav.dev");
    
    // Configure HTTP bearer authorization: HTTPBearer
    HttpBearerAuth HTTPBearer = (HttpBearerAuth) defaultClient.getAuthentication("HTTPBearer");
    HTTPBearer.setBearerToken("BEARER TOKEN");

    EpisodesApi apiInstance = new EpisodesApi(defaultClient);
    String episodeId = "episodeId_example"; // String | 
    try {
      apiInstance.deleteEpisodeEpisodesEpisodeIdDelete(episodeId);
    } catch (ApiException e) {
      System.err.println("Exception when calling EpisodesApi#deleteEpisodeEpisodesEpisodeIdDelete");
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
| **episodeId** | **String**|  | |

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
| **204** | Episode deleted successfully |  -  |
| **404** | Episode not found |  -  |
| **422** | Validation Error |  -  |

<a id="getEpisodeEpisodesEpisodeIdGet"></a>
# **getEpisodeEpisodesEpisodeIdGet**
> Episode getEpisodeEpisodesEpisodeIdGet(episodeId)

Get an episode by ID

Retrieve detailed information about a specific episode.

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.EpisodesApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://believe.cjav.dev");
    
    // Configure HTTP bearer authorization: HTTPBearer
    HttpBearerAuth HTTPBearer = (HttpBearerAuth) defaultClient.getAuthentication("HTTPBearer");
    HTTPBearer.setBearerToken("BEARER TOKEN");

    EpisodesApi apiInstance = new EpisodesApi(defaultClient);
    String episodeId = "episodeId_example"; // String | 
    try {
      Episode result = apiInstance.getEpisodeEpisodesEpisodeIdGet(episodeId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling EpisodesApi#getEpisodeEpisodesEpisodeIdGet");
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
| **episodeId** | **String**|  | |

### Return type

[**Episode**](Episode.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Episode details |  -  |
| **404** | Episode not found |  -  |
| **422** | Validation Error |  -  |

<a id="getEpisodeWisdomEpisodesEpisodeIdWisdomGet"></a>
# **getEpisodeWisdomEpisodesEpisodeIdWisdomGet**
> Map&lt;String, Object&gt; getEpisodeWisdomEpisodesEpisodeIdWisdomGet(episodeId)

Get episode wisdom

Get Ted&#39;s wisdom and memorable moments from a specific episode.

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.EpisodesApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://believe.cjav.dev");
    
    // Configure HTTP bearer authorization: HTTPBearer
    HttpBearerAuth HTTPBearer = (HttpBearerAuth) defaultClient.getAuthentication("HTTPBearer");
    HTTPBearer.setBearerToken("BEARER TOKEN");

    EpisodesApi apiInstance = new EpisodesApi(defaultClient);
    String episodeId = "episodeId_example"; // String | 
    try {
      Map<String, Object> result = apiInstance.getEpisodeWisdomEpisodesEpisodeIdWisdomGet(episodeId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling EpisodesApi#getEpisodeWisdomEpisodesEpisodeIdWisdomGet");
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
| **episodeId** | **String**|  | |

### Return type

**Map&lt;String, Object&gt;**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Episode wisdom details |  -  |
| **404** | Episode not found |  -  |
| **422** | Validation Error |  -  |

<a id="getSeasonEpisodesEpisodesSeasonsSeasonNumberGet"></a>
# **getSeasonEpisodesEpisodesSeasonsSeasonNumberGet**
> PaginatedResponseEpisode getSeasonEpisodesEpisodesSeasonsSeasonNumberGet(seasonNumber, skip, limit)

Get all episodes from a season

Get a paginated list of episodes from a specific season.

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.EpisodesApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://believe.cjav.dev");
    
    // Configure HTTP bearer authorization: HTTPBearer
    HttpBearerAuth HTTPBearer = (HttpBearerAuth) defaultClient.getAuthentication("HTTPBearer");
    HTTPBearer.setBearerToken("BEARER TOKEN");

    EpisodesApi apiInstance = new EpisodesApi(defaultClient);
    Integer seasonNumber = 56; // Integer | 
    Integer skip = 0; // Integer | Number of items to skip (offset)
    Integer limit = 20; // Integer | Maximum number of items to return (max: 100)
    try {
      PaginatedResponseEpisode result = apiInstance.getSeasonEpisodesEpisodesSeasonsSeasonNumberGet(seasonNumber, skip, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling EpisodesApi#getSeasonEpisodesEpisodesSeasonsSeasonNumberGet");
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
| **seasonNumber** | **Integer**|  | |
| **skip** | **Integer**| Number of items to skip (offset) | [optional] [default to 0] |
| **limit** | **Integer**| Maximum number of items to return (max: 100) | [optional] [default to 20] |

### Return type

[**PaginatedResponseEpisode**](PaginatedResponseEpisode.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Paginated list of episodes from the season |  -  |
| **404** | Season not found |  -  |
| **422** | Validation Error |  -  |

<a id="listEpisodesEpisodesGet"></a>
# **listEpisodesEpisodesGet**
> PaginatedResponseEpisode listEpisodesEpisodesGet(season, characterFocus, skip, limit)

List all episodes

Get a paginated list of all Ted Lasso episodes with optional filtering by season.

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.EpisodesApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://believe.cjav.dev");
    
    // Configure HTTP bearer authorization: HTTPBearer
    HttpBearerAuth HTTPBearer = (HttpBearerAuth) defaultClient.getAuthentication("HTTPBearer");
    HTTPBearer.setBearerToken("BEARER TOKEN");

    EpisodesApi apiInstance = new EpisodesApi(defaultClient);
    Integer season = 56; // Integer | Filter by season
    String characterFocus = "characterFocus_example"; // String | Filter by character focus (character ID)
    Integer skip = 0; // Integer | Number of items to skip (offset)
    Integer limit = 20; // Integer | Maximum number of items to return (max: 100)
    try {
      PaginatedResponseEpisode result = apiInstance.listEpisodesEpisodesGet(season, characterFocus, skip, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling EpisodesApi#listEpisodesEpisodesGet");
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
| **season** | **Integer**| Filter by season | [optional] |
| **characterFocus** | **String**| Filter by character focus (character ID) | [optional] |
| **skip** | **Integer**| Number of items to skip (offset) | [optional] [default to 0] |
| **limit** | **Integer**| Maximum number of items to return (max: 100) | [optional] [default to 20] |

### Return type

[**PaginatedResponseEpisode**](PaginatedResponseEpisode.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Paginated list of episodes |  -  |
| **422** | Validation Error |  -  |

<a id="updateEpisodeEpisodesEpisodeIdPatch"></a>
# **updateEpisodeEpisodesEpisodeIdPatch**
> Episode updateEpisodeEpisodesEpisodeIdPatch(episodeId, episodeUpdate)

Update an episode

Update specific fields of an existing episode.

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.EpisodesApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://believe.cjav.dev");
    
    // Configure HTTP bearer authorization: HTTPBearer
    HttpBearerAuth HTTPBearer = (HttpBearerAuth) defaultClient.getAuthentication("HTTPBearer");
    HTTPBearer.setBearerToken("BEARER TOKEN");

    EpisodesApi apiInstance = new EpisodesApi(defaultClient);
    String episodeId = "episodeId_example"; // String | 
    EpisodeUpdate episodeUpdate = new EpisodeUpdate(); // EpisodeUpdate | 
    try {
      Episode result = apiInstance.updateEpisodeEpisodesEpisodeIdPatch(episodeId, episodeUpdate);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling EpisodesApi#updateEpisodeEpisodesEpisodeIdPatch");
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
| **episodeId** | **String**|  | |
| **episodeUpdate** | [**EpisodeUpdate**](EpisodeUpdate.md)|  | |

### Return type

[**Episode**](Episode.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Episode updated successfully |  -  |
| **404** | Episode not found |  -  |
| **422** | Validation Error |  -  |

