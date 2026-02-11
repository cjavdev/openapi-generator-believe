# InteractiveApi

All URIs are relative to *https://believe.cjav.dev*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**believeEngineBelievePost**](InteractiveApi.md#believeEngineBelievePost) | **POST** /believe | The Believe Engine |
| [**getBiscuitBiscuitsBiscuitIdGet**](InteractiveApi.md#getBiscuitBiscuitsBiscuitIdGet) | **GET** /biscuits/{biscuit_id} | Get a Specific Biscuit |
| [**getBiscuitsBiscuitsGet**](InteractiveApi.md#getBiscuitsBiscuitsGet) | **GET** /biscuits | Biscuits as a Service |
| [**getCoachingPrincipleCoachingPrinciplesPrincipleIdGet**](InteractiveApi.md#getCoachingPrincipleCoachingPrinciplesPrincipleIdGet) | **GET** /coaching/principles/{principle_id} | Get a Specific Coaching Principle |
| [**getCoachingPrinciplesCoachingPrinciplesGet**](InteractiveApi.md#getCoachingPrinciplesCoachingPrinciplesGet) | **GET** /coaching/principles | Get Coaching Principles |
| [**getFreshBiscuitBiscuitsFreshGet**](InteractiveApi.md#getFreshBiscuitBiscuitsFreshGet) | **GET** /biscuits/fresh | Get a Fresh Biscuit |
| [**getRandomPrincipleCoachingPrinciplesRandomGet**](InteractiveApi.md#getRandomPrincipleCoachingPrinciplesRandomGet) | **GET** /coaching/principles/random | Get a Random Coaching Principle |
| [**pressConferencePressPost**](InteractiveApi.md#pressConferencePressPost) | **POST** /press | Press Conference Simulator |
| [**reframeThoughtReframePost**](InteractiveApi.md#reframeThoughtReframePost) | **POST** /reframe | Reframe Negative Thoughts |
| [**resolveConflictConflictsResolvePost**](InteractiveApi.md#resolveConflictConflictsResolvePost) | **POST** /conflicts/resolve | Resolve Conflicts |


<a id="believeEngineBelievePost"></a>
# **believeEngineBelievePost**
> BelieveResponse believeEngineBelievePost(believeRequest)

The Believe Engine

Submit your situation and receive Ted Lasso-style motivational guidance.

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.InteractiveApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://believe.cjav.dev");
    
    // Configure HTTP bearer authorization: HTTPBearer
    HttpBearerAuth HTTPBearer = (HttpBearerAuth) defaultClient.getAuthentication("HTTPBearer");
    HTTPBearer.setBearerToken("BEARER TOKEN");

    InteractiveApi apiInstance = new InteractiveApi(defaultClient);
    BelieveRequest believeRequest = new BelieveRequest(); // BelieveRequest | 
    try {
      BelieveResponse result = apiInstance.believeEngineBelievePost(believeRequest);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling InteractiveApi#believeEngineBelievePost");
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
| **believeRequest** | [**BelieveRequest**](BelieveRequest.md)|  | |

### Return type

[**BelieveResponse**](BelieveResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Motivational response generated |  -  |
| **418** | You&#39;re already a believer! |  -  |
| **422** | Validation Error |  -  |
| **429** | Too much negativity detected |  -  |

<a id="getBiscuitBiscuitsBiscuitIdGet"></a>
# **getBiscuitBiscuitsBiscuitIdGet**
> Biscuit getBiscuitBiscuitsBiscuitIdGet(biscuitId)

Get a Specific Biscuit

Get a specific type of biscuit by ID.

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.InteractiveApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://believe.cjav.dev");
    
    // Configure HTTP bearer authorization: HTTPBearer
    HttpBearerAuth HTTPBearer = (HttpBearerAuth) defaultClient.getAuthentication("HTTPBearer");
    HTTPBearer.setBearerToken("BEARER TOKEN");

    InteractiveApi apiInstance = new InteractiveApi(defaultClient);
    String biscuitId = "biscuitId_example"; // String | 
    try {
      Biscuit result = apiInstance.getBiscuitBiscuitsBiscuitIdGet(biscuitId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling InteractiveApi#getBiscuitBiscuitsBiscuitIdGet");
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
| **biscuitId** | **String**|  | |

### Return type

[**Biscuit**](Biscuit.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Biscuit details |  -  |
| **404** | Biscuit not found |  -  |
| **422** | Validation Error |  -  |

<a id="getBiscuitsBiscuitsGet"></a>
# **getBiscuitsBiscuitsGet**
> PaginatedResponseBiscuit getBiscuitsBiscuitsGet(skip, limit)

Biscuits as a Service

Get a paginated list of Ted&#39;s famous homemade biscuits! Each comes with a heartwarming message.

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.InteractiveApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://believe.cjav.dev");
    
    // Configure HTTP bearer authorization: HTTPBearer
    HttpBearerAuth HTTPBearer = (HttpBearerAuth) defaultClient.getAuthentication("HTTPBearer");
    HTTPBearer.setBearerToken("BEARER TOKEN");

    InteractiveApi apiInstance = new InteractiveApi(defaultClient);
    Integer skip = 0; // Integer | Number of items to skip (offset)
    Integer limit = 20; // Integer | Maximum number of items to return (max: 100)
    try {
      PaginatedResponseBiscuit result = apiInstance.getBiscuitsBiscuitsGet(skip, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling InteractiveApi#getBiscuitsBiscuitsGet");
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
| **skip** | **Integer**| Number of items to skip (offset) | [optional] [default to 0] |
| **limit** | **Integer**| Maximum number of items to return (max: 100) | [optional] [default to 20] |

### Return type

[**PaginatedResponseBiscuit**](PaginatedResponseBiscuit.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Paginated list of fresh biscuits from Ted&#39;s kitchen |  -  |
| **422** | Validation Error |  -  |

<a id="getCoachingPrincipleCoachingPrinciplesPrincipleIdGet"></a>
# **getCoachingPrincipleCoachingPrinciplesPrincipleIdGet**
> CoachingPrinciple getCoachingPrincipleCoachingPrinciplesPrincipleIdGet(principleId)

Get a Specific Coaching Principle

Get details about a specific coaching principle.

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.InteractiveApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://believe.cjav.dev");
    
    // Configure HTTP bearer authorization: HTTPBearer
    HttpBearerAuth HTTPBearer = (HttpBearerAuth) defaultClient.getAuthentication("HTTPBearer");
    HTTPBearer.setBearerToken("BEARER TOKEN");

    InteractiveApi apiInstance = new InteractiveApi(defaultClient);
    String principleId = "principleId_example"; // String | 
    try {
      CoachingPrinciple result = apiInstance.getCoachingPrincipleCoachingPrinciplesPrincipleIdGet(principleId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling InteractiveApi#getCoachingPrincipleCoachingPrinciplesPrincipleIdGet");
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
| **principleId** | **String**|  | |

### Return type

[**CoachingPrinciple**](CoachingPrinciple.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Coaching principle details |  -  |
| **404** | Principle not found |  -  |
| **422** | Validation Error |  -  |

<a id="getCoachingPrinciplesCoachingPrinciplesGet"></a>
# **getCoachingPrinciplesCoachingPrinciplesGet**
> PaginatedResponseCoachingPrinciple getCoachingPrinciplesCoachingPrinciplesGet(skip, limit)

Get Coaching Principles

Get a paginated list of Ted Lasso&#39;s core coaching principles and philosophy.

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.InteractiveApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://believe.cjav.dev");
    
    // Configure HTTP bearer authorization: HTTPBearer
    HttpBearerAuth HTTPBearer = (HttpBearerAuth) defaultClient.getAuthentication("HTTPBearer");
    HTTPBearer.setBearerToken("BEARER TOKEN");

    InteractiveApi apiInstance = new InteractiveApi(defaultClient);
    Integer skip = 0; // Integer | Number of items to skip (offset)
    Integer limit = 20; // Integer | Maximum number of items to return (max: 100)
    try {
      PaginatedResponseCoachingPrinciple result = apiInstance.getCoachingPrinciplesCoachingPrinciplesGet(skip, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling InteractiveApi#getCoachingPrinciplesCoachingPrinciplesGet");
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
| **skip** | **Integer**| Number of items to skip (offset) | [optional] [default to 0] |
| **limit** | **Integer**| Maximum number of items to return (max: 100) | [optional] [default to 20] |

### Return type

[**PaginatedResponseCoachingPrinciple**](PaginatedResponseCoachingPrinciple.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Paginated list of coaching principles |  -  |
| **422** | Validation Error |  -  |

<a id="getFreshBiscuitBiscuitsFreshGet"></a>
# **getFreshBiscuitBiscuitsFreshGet**
> Biscuit getFreshBiscuitBiscuitsFreshGet()

Get a Fresh Biscuit

Get a single fresh biscuit with a personalized message from Ted.

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.InteractiveApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://believe.cjav.dev");
    
    // Configure HTTP bearer authorization: HTTPBearer
    HttpBearerAuth HTTPBearer = (HttpBearerAuth) defaultClient.getAuthentication("HTTPBearer");
    HTTPBearer.setBearerToken("BEARER TOKEN");

    InteractiveApi apiInstance = new InteractiveApi(defaultClient);
    try {
      Biscuit result = apiInstance.getFreshBiscuitBiscuitsFreshGet();
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling InteractiveApi#getFreshBiscuitBiscuitsFreshGet");
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

[**Biscuit**](Biscuit.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | A fresh biscuit from Ted&#39;s kitchen |  -  |

<a id="getRandomPrincipleCoachingPrinciplesRandomGet"></a>
# **getRandomPrincipleCoachingPrinciplesRandomGet**
> CoachingPrinciple getRandomPrincipleCoachingPrinciplesRandomGet()

Get a Random Coaching Principle

Get a random coaching principle to inspire your day.

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.InteractiveApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://believe.cjav.dev");
    
    // Configure HTTP bearer authorization: HTTPBearer
    HttpBearerAuth HTTPBearer = (HttpBearerAuth) defaultClient.getAuthentication("HTTPBearer");
    HTTPBearer.setBearerToken("BEARER TOKEN");

    InteractiveApi apiInstance = new InteractiveApi(defaultClient);
    try {
      CoachingPrinciple result = apiInstance.getRandomPrincipleCoachingPrinciplesRandomGet();
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling InteractiveApi#getRandomPrincipleCoachingPrinciplesRandomGet");
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

[**CoachingPrinciple**](CoachingPrinciple.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | A random coaching principle |  -  |

<a id="pressConferencePressPost"></a>
# **pressConferencePressPost**
> PressConferenceResponse pressConferencePressPost(pressConferenceRequest)

Press Conference Simulator

Get Ted&#39;s response to press conference questions.

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.InteractiveApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://believe.cjav.dev");
    
    // Configure HTTP bearer authorization: HTTPBearer
    HttpBearerAuth HTTPBearer = (HttpBearerAuth) defaultClient.getAuthentication("HTTPBearer");
    HTTPBearer.setBearerToken("BEARER TOKEN");

    InteractiveApi apiInstance = new InteractiveApi(defaultClient);
    PressConferenceRequest pressConferenceRequest = new PressConferenceRequest(); // PressConferenceRequest | 
    try {
      PressConferenceResponse result = apiInstance.pressConferencePressPost(pressConferenceRequest);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling InteractiveApi#pressConferencePressPost");
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
| **pressConferenceRequest** | [**PressConferenceRequest**](PressConferenceRequest.md)|  | |

### Return type

[**PressConferenceResponse**](PressConferenceResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Press conference response |  -  |
| **422** | Validation Error |  -  |

<a id="reframeThoughtReframePost"></a>
# **reframeThoughtReframePost**
> ReframeResponse reframeThoughtReframePost(reframeRequest)

Reframe Negative Thoughts

Transform negative thoughts into positive perspectives with Ted&#39;s help.

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.InteractiveApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://believe.cjav.dev");
    
    // Configure HTTP bearer authorization: HTTPBearer
    HttpBearerAuth HTTPBearer = (HttpBearerAuth) defaultClient.getAuthentication("HTTPBearer");
    HTTPBearer.setBearerToken("BEARER TOKEN");

    InteractiveApi apiInstance = new InteractiveApi(defaultClient);
    ReframeRequest reframeRequest = new ReframeRequest(); // ReframeRequest | 
    try {
      ReframeResponse result = apiInstance.reframeThoughtReframePost(reframeRequest);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling InteractiveApi#reframeThoughtReframePost");
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
| **reframeRequest** | [**ReframeRequest**](ReframeRequest.md)|  | |

### Return type

[**ReframeResponse**](ReframeResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Reframed perspective |  -  |
| **422** | Validation Error |  -  |
| **429** | Too much negativity |  -  |

<a id="resolveConflictConflictsResolvePost"></a>
# **resolveConflictConflictsResolvePost**
> ConflictResolution resolveConflictConflictsResolvePost(conflictRequest)

Resolve Conflicts

Get Ted Lasso-style advice for resolving conflicts.

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.InteractiveApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://believe.cjav.dev");
    
    // Configure HTTP bearer authorization: HTTPBearer
    HttpBearerAuth HTTPBearer = (HttpBearerAuth) defaultClient.getAuthentication("HTTPBearer");
    HTTPBearer.setBearerToken("BEARER TOKEN");

    InteractiveApi apiInstance = new InteractiveApi(defaultClient);
    ConflictRequest conflictRequest = new ConflictRequest(); // ConflictRequest | 
    try {
      ConflictResolution result = apiInstance.resolveConflictConflictsResolvePost(conflictRequest);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling InteractiveApi#resolveConflictConflictsResolvePost");
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
| **conflictRequest** | [**ConflictRequest**](ConflictRequest.md)|  | |

### Return type

[**ConflictResolution**](ConflictResolution.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Conflict resolution guidance |  -  |
| **403** | Too judgmental |  -  |
| **422** | Validation Error |  -  |

