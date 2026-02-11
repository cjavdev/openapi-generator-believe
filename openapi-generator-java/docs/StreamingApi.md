# StreamingApi

All URIs are relative to *https://believe.cjav.dev*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getPepTalkPepTalkGet**](StreamingApi.md#getPepTalkPepTalkGet) | **GET** /pep-talk | Get a Pep Talk |
| [**streamMatchCommentaryMatchesMatchIdCommentaryStreamPost**](StreamingApi.md#streamMatchCommentaryMatchesMatchIdCommentaryStreamPost) | **POST** /matches/{match_id}/commentary/stream | Stream Match Commentary |
| [**testStreamStreamTestGet**](StreamingApi.md#testStreamStreamTestGet) | **GET** /stream/test | Test SSE Connection |


<a id="getPepTalkPepTalkGet"></a>
# **getPepTalkPepTalkGet**
> PepTalkResponse getPepTalkPepTalkGet(stream)

Get a Pep Talk

Get a motivational pep talk from Ted Lasso himself. By default returns the complete pep talk. Add &#x60;?stream&#x3D;true&#x60; to get Server-Sent Events (SSE) streaming the pep talk chunk by chunk.

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.StreamingApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://believe.cjav.dev");
    
    // Configure HTTP bearer authorization: HTTPBearer
    HttpBearerAuth HTTPBearer = (HttpBearerAuth) defaultClient.getAuthentication("HTTPBearer");
    HTTPBearer.setBearerToken("BEARER TOKEN");

    StreamingApi apiInstance = new StreamingApi(defaultClient);
    Boolean stream = false; // Boolean | If true, returns SSE stream instead of full response
    try {
      PepTalkResponse result = apiInstance.getPepTalkPepTalkGet(stream);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling StreamingApi#getPepTalkPepTalkGet");
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
| **stream** | **Boolean**| If true, returns SSE stream instead of full response | [optional] [default to false] |

### Return type

[**PepTalkResponse**](PepTalkResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/event-stream

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Pep talk response (JSON or SSE stream) |  -  |
| **422** | Validation Error |  -  |

<a id="streamMatchCommentaryMatchesMatchIdCommentaryStreamPost"></a>
# **streamMatchCommentaryMatchesMatchIdCommentaryStreamPost**
> Object streamMatchCommentaryMatchesMatchIdCommentaryStreamPost(matchId)

Stream Match Commentary

Stream live match commentary for a specific match. Uses Server-Sent Events (SSE) to stream commentary events in real-time.

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.StreamingApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://believe.cjav.dev");
    
    // Configure HTTP bearer authorization: HTTPBearer
    HttpBearerAuth HTTPBearer = (HttpBearerAuth) defaultClient.getAuthentication("HTTPBearer");
    HTTPBearer.setBearerToken("BEARER TOKEN");

    StreamingApi apiInstance = new StreamingApi(defaultClient);
    String matchId = "matchId_example"; // String | 
    try {
      Object result = apiInstance.streamMatchCommentaryMatchesMatchIdCommentaryStreamPost(matchId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling StreamingApi#streamMatchCommentaryMatchesMatchIdCommentaryStreamPost");
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

**Object**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/event-stream

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | SSE stream of match commentary events |  -  |
| **404** | Match not found |  -  |
| **422** | Validation Error |  -  |

<a id="testStreamStreamTestGet"></a>
# **testStreamStreamTestGet**
> Object testStreamStreamTestGet()

Test SSE Connection

A simple SSE test endpoint that streams numbers 1-5.

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.StreamingApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://believe.cjav.dev");
    
    // Configure HTTP bearer authorization: HTTPBearer
    HttpBearerAuth HTTPBearer = (HttpBearerAuth) defaultClient.getAuthentication("HTTPBearer");
    HTTPBearer.setBearerToken("BEARER TOKEN");

    StreamingApi apiInstance = new StreamingApi(defaultClient);
    try {
      Object result = apiInstance.testStreamStreamTestGet();
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling StreamingApi#testStreamStreamTestGet");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

**Object**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/event-stream

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | SSE stream of test messages |  -  |

