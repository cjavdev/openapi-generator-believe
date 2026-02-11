# MatchesApi

All URIs are relative to *https://believe.cjav.dev*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createMatchMatchesPost**](MatchesApi.md#createMatchMatchesPost) | **POST** /matches | Create a new match |
| [**deleteMatchMatchesMatchIdDelete**](MatchesApi.md#deleteMatchMatchesMatchIdDelete) | **DELETE** /matches/{match_id} | Delete a match |
| [**getMatchLessonMatchesMatchIdLessonGet**](MatchesApi.md#getMatchLessonMatchesMatchIdLessonGet) | **GET** /matches/{match_id}/lesson | Get match lesson |
| [**getMatchMatchesMatchIdGet**](MatchesApi.md#getMatchMatchesMatchIdGet) | **GET** /matches/{match_id} | Get a match by ID |
| [**getTurningPointsMatchesMatchIdTurningPointsGet**](MatchesApi.md#getTurningPointsMatchesMatchIdTurningPointsGet) | **GET** /matches/{match_id}/turning-points | Get match turning points |
| [**listMatchesMatchesGet**](MatchesApi.md#listMatchesMatchesGet) | **GET** /matches | List all matches |
| [**updateMatchMatchesMatchIdPatch**](MatchesApi.md#updateMatchMatchesMatchIdPatch) | **PATCH** /matches/{match_id} | Update a match |


<a id="createMatchMatchesPost"></a>
# **createMatchMatchesPost**
> Match createMatchMatchesPost(matchCreate)

Create a new match

Schedule a new match.

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.MatchesApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://believe.cjav.dev");
    
    // Configure HTTP bearer authorization: HTTPBearer
    HttpBearerAuth HTTPBearer = (HttpBearerAuth) defaultClient.getAuthentication("HTTPBearer");
    HTTPBearer.setBearerToken("BEARER TOKEN");

    MatchesApi apiInstance = new MatchesApi(defaultClient);
    MatchCreate matchCreate = new MatchCreate(); // MatchCreate | 
    try {
      Match result = apiInstance.createMatchMatchesPost(matchCreate);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling MatchesApi#createMatchMatchesPost");
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
| **matchCreate** | [**MatchCreate**](MatchCreate.md)|  | |

### Return type

[**Match**](Match.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Match created successfully |  -  |
| **422** | Validation Error |  -  |

<a id="deleteMatchMatchesMatchIdDelete"></a>
# **deleteMatchMatchesMatchIdDelete**
> deleteMatchMatchesMatchIdDelete(matchId)

Delete a match

Remove a match from the database.

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.MatchesApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://believe.cjav.dev");
    
    // Configure HTTP bearer authorization: HTTPBearer
    HttpBearerAuth HTTPBearer = (HttpBearerAuth) defaultClient.getAuthentication("HTTPBearer");
    HTTPBearer.setBearerToken("BEARER TOKEN");

    MatchesApi apiInstance = new MatchesApi(defaultClient);
    String matchId = "matchId_example"; // String | 
    try {
      apiInstance.deleteMatchMatchesMatchIdDelete(matchId);
    } catch (ApiException e) {
      System.err.println("Exception when calling MatchesApi#deleteMatchMatchesMatchIdDelete");
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
| **matchId** | **String**|  | |

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
| **204** | Match deleted successfully |  -  |
| **404** | Match not found |  -  |
| **422** | Validation Error |  -  |

<a id="getMatchLessonMatchesMatchIdLessonGet"></a>
# **getMatchLessonMatchesMatchIdLessonGet**
> Map&lt;String, Object&gt; getMatchLessonMatchesMatchIdLessonGet(matchId)

Get match lesson

Get the life lesson learned from a specific match.

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.MatchesApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://believe.cjav.dev");
    
    // Configure HTTP bearer authorization: HTTPBearer
    HttpBearerAuth HTTPBearer = (HttpBearerAuth) defaultClient.getAuthentication("HTTPBearer");
    HTTPBearer.setBearerToken("BEARER TOKEN");

    MatchesApi apiInstance = new MatchesApi(defaultClient);
    String matchId = "matchId_example"; // String | 
    try {
      Map<String, Object> result = apiInstance.getMatchLessonMatchesMatchIdLessonGet(matchId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling MatchesApi#getMatchLessonMatchesMatchIdLessonGet");
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
| **matchId** | **String**|  | |

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
| **200** | Match lesson details |  -  |
| **404** | Match not found |  -  |
| **422** | Validation Error |  -  |

<a id="getMatchMatchesMatchIdGet"></a>
# **getMatchMatchesMatchIdGet**
> Match getMatchMatchesMatchIdGet(matchId)

Get a match by ID

Retrieve detailed information about a specific match.

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.MatchesApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://believe.cjav.dev");
    
    // Configure HTTP bearer authorization: HTTPBearer
    HttpBearerAuth HTTPBearer = (HttpBearerAuth) defaultClient.getAuthentication("HTTPBearer");
    HTTPBearer.setBearerToken("BEARER TOKEN");

    MatchesApi apiInstance = new MatchesApi(defaultClient);
    String matchId = "matchId_example"; // String | 
    try {
      Match result = apiInstance.getMatchMatchesMatchIdGet(matchId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling MatchesApi#getMatchMatchesMatchIdGet");
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
| **matchId** | **String**|  | |

### Return type

[**Match**](Match.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Match details |  -  |
| **404** | Match not found |  -  |
| **422** | Validation Error |  -  |

<a id="getTurningPointsMatchesMatchIdTurningPointsGet"></a>
# **getTurningPointsMatchesMatchIdTurningPointsGet**
> List&lt;Map&lt;String, Object&gt;&gt; getTurningPointsMatchesMatchIdTurningPointsGet(matchId)

Get match turning points

Get all turning points from a specific match.

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.MatchesApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://believe.cjav.dev");
    
    // Configure HTTP bearer authorization: HTTPBearer
    HttpBearerAuth HTTPBearer = (HttpBearerAuth) defaultClient.getAuthentication("HTTPBearer");
    HTTPBearer.setBearerToken("BEARER TOKEN");

    MatchesApi apiInstance = new MatchesApi(defaultClient);
    String matchId = "matchId_example"; // String | 
    try {
      List<Map<String, Object>> result = apiInstance.getTurningPointsMatchesMatchIdTurningPointsGet(matchId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling MatchesApi#getTurningPointsMatchesMatchIdTurningPointsGet");
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
| **matchId** | **String**|  | |

### Return type

[**List&lt;Map&lt;String, Object&gt;&gt;**](Map.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of turning points |  -  |
| **404** | Match not found |  -  |
| **422** | Validation Error |  -  |

<a id="listMatchesMatchesGet"></a>
# **listMatchesMatchesGet**
> PaginatedResponseMatch listMatchesMatchesGet(teamId, result, matchType, skip, limit)

List all matches

Get a paginated list of all matches with optional filtering.

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.MatchesApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://believe.cjav.dev");
    
    // Configure HTTP bearer authorization: HTTPBearer
    HttpBearerAuth HTTPBearer = (HttpBearerAuth) defaultClient.getAuthentication("HTTPBearer");
    HTTPBearer.setBearerToken("BEARER TOKEN");

    MatchesApi apiInstance = new MatchesApi(defaultClient);
    String teamId = "teamId_example"; // String | Filter by team (home or away)
    MatchResult result = MatchResult.fromValue("win"); // MatchResult | Filter by result
    MatchType matchType = MatchType.fromValue("league"); // MatchType | Filter by match type
    Integer skip = 0; // Integer | Number of items to skip (offset)
    Integer limit = 20; // Integer | Maximum number of items to return (max: 100)
    try {
      PaginatedResponseMatch result = apiInstance.listMatchesMatchesGet(teamId, result, matchType, skip, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling MatchesApi#listMatchesMatchesGet");
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
| **teamId** | **String**| Filter by team (home or away) | [optional] |
| **result** | [**MatchResult**](.md)| Filter by result | [optional] [enum: win, loss, draw, pending] |
| **matchType** | [**MatchType**](.md)| Filter by match type | [optional] [enum: league, cup, friendly, playoff, final] |
| **skip** | **Integer**| Number of items to skip (offset) | [optional] [default to 0] |
| **limit** | **Integer**| Maximum number of items to return (max: 100) | [optional] [default to 20] |

### Return type

[**PaginatedResponseMatch**](PaginatedResponseMatch.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Paginated list of matches |  -  |
| **422** | Validation Error |  -  |

<a id="updateMatchMatchesMatchIdPatch"></a>
# **updateMatchMatchesMatchIdPatch**
> Match updateMatchMatchesMatchIdPatch(matchId, matchUpdate)

Update a match

Update specific fields of an existing match (e.g., update score).

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.MatchesApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://believe.cjav.dev");
    
    // Configure HTTP bearer authorization: HTTPBearer
    HttpBearerAuth HTTPBearer = (HttpBearerAuth) defaultClient.getAuthentication("HTTPBearer");
    HTTPBearer.setBearerToken("BEARER TOKEN");

    MatchesApi apiInstance = new MatchesApi(defaultClient);
    String matchId = "matchId_example"; // String | 
    MatchUpdate matchUpdate = new MatchUpdate(); // MatchUpdate | 
    try {
      Match result = apiInstance.updateMatchMatchesMatchIdPatch(matchId, matchUpdate);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling MatchesApi#updateMatchMatchesMatchIdPatch");
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
| **matchId** | **String**|  | |
| **matchUpdate** | [**MatchUpdate**](MatchUpdate.md)|  | |

### Return type

[**Match**](Match.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Match updated successfully |  -  |
| **404** | Match not found |  -  |
| **422** | Validation Error |  -  |

