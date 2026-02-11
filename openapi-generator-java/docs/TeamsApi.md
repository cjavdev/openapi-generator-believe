# TeamsApi

All URIs are relative to *https://believe.cjav.dev*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createTeamTeamsPost**](TeamsApi.md#createTeamTeamsPost) | **POST** /teams | Create a new team |
| [**deleteTeamLogoTeamsTeamIdLogoFileIdDelete**](TeamsApi.md#deleteTeamLogoTeamsTeamIdLogoFileIdDelete) | **DELETE** /teams/{team_id}/logo/{file_id} | Delete team logo |
| [**deleteTeamTeamsTeamIdDelete**](TeamsApi.md#deleteTeamTeamsTeamIdDelete) | **DELETE** /teams/{team_id} | Delete a team |
| [**downloadTeamLogoTeamsTeamIdLogoFileIdGet**](TeamsApi.md#downloadTeamLogoTeamsTeamIdLogoFileIdGet) | **GET** /teams/{team_id}/logo/{file_id} | Download team logo |
| [**getTeamCultureTeamsTeamIdCultureGet**](TeamsApi.md#getTeamCultureTeamsTeamIdCultureGet) | **GET** /teams/{team_id}/culture | Get team culture details |
| [**getTeamRivalsTeamsTeamIdRivalsGet**](TeamsApi.md#getTeamRivalsTeamsTeamIdRivalsGet) | **GET** /teams/{team_id}/rivals | Get team&#39;s rivals |
| [**getTeamTeamsTeamIdGet**](TeamsApi.md#getTeamTeamsTeamIdGet) | **GET** /teams/{team_id} | Get a team by ID |
| [**listTeamLogosTeamsTeamIdLogosGet**](TeamsApi.md#listTeamLogosTeamsTeamIdLogosGet) | **GET** /teams/{team_id}/logos | List team logos |
| [**listTeamsTeamsGet**](TeamsApi.md#listTeamsTeamsGet) | **GET** /teams | List all teams |
| [**updateTeamTeamsTeamIdPatch**](TeamsApi.md#updateTeamTeamsTeamIdPatch) | **PATCH** /teams/{team_id} | Update a team |
| [**uploadTeamLogoTeamsTeamIdLogoPost**](TeamsApi.md#uploadTeamLogoTeamsTeamIdLogoPost) | **POST** /teams/{team_id}/logo | Upload team logo |


<a id="createTeamTeamsPost"></a>
# **createTeamTeamsPost**
> Team createTeamTeamsPost(teamCreate)

Create a new team

Add a new team to the league.

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.TeamsApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://believe.cjav.dev");
    
    // Configure HTTP bearer authorization: HTTPBearer
    HttpBearerAuth HTTPBearer = (HttpBearerAuth) defaultClient.getAuthentication("HTTPBearer");
    HTTPBearer.setBearerToken("BEARER TOKEN");

    TeamsApi apiInstance = new TeamsApi(defaultClient);
    TeamCreate teamCreate = new TeamCreate(); // TeamCreate | 
    try {
      Team result = apiInstance.createTeamTeamsPost(teamCreate);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling TeamsApi#createTeamTeamsPost");
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
| **teamCreate** | [**TeamCreate**](TeamCreate.md)|  | |

### Return type

[**Team**](Team.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Team created successfully |  -  |
| **409** | Team already exists |  -  |
| **422** | Validation Error |  -  |

<a id="deleteTeamLogoTeamsTeamIdLogoFileIdDelete"></a>
# **deleteTeamLogoTeamsTeamIdLogoFileIdDelete**
> deleteTeamLogoTeamsTeamIdLogoFileIdDelete(teamId, fileId)

Delete team logo

Delete a team&#39;s logo.

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.TeamsApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://believe.cjav.dev");
    
    // Configure HTTP bearer authorization: HTTPBearer
    HttpBearerAuth HTTPBearer = (HttpBearerAuth) defaultClient.getAuthentication("HTTPBearer");
    HTTPBearer.setBearerToken("BEARER TOKEN");

    TeamsApi apiInstance = new TeamsApi(defaultClient);
    String teamId = "teamId_example"; // String | 
    UUID fileId = UUID.randomUUID(); // UUID | 
    try {
      apiInstance.deleteTeamLogoTeamsTeamIdLogoFileIdDelete(teamId, fileId);
    } catch (ApiException e) {
      System.err.println("Exception when calling TeamsApi#deleteTeamLogoTeamsTeamIdLogoFileIdDelete");
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
| **teamId** | **String**|  | |
| **fileId** | **UUID**|  | |

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
| **204** | Logo deleted |  -  |
| **404** | Team or file not found |  -  |
| **422** | Validation Error |  -  |

<a id="deleteTeamTeamsTeamIdDelete"></a>
# **deleteTeamTeamsTeamIdDelete**
> deleteTeamTeamsTeamIdDelete(teamId)

Delete a team

Remove a team from the database (relegation to oblivion).

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.TeamsApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://believe.cjav.dev");
    
    // Configure HTTP bearer authorization: HTTPBearer
    HttpBearerAuth HTTPBearer = (HttpBearerAuth) defaultClient.getAuthentication("HTTPBearer");
    HTTPBearer.setBearerToken("BEARER TOKEN");

    TeamsApi apiInstance = new TeamsApi(defaultClient);
    String teamId = "teamId_example"; // String | 
    try {
      apiInstance.deleteTeamTeamsTeamIdDelete(teamId);
    } catch (ApiException e) {
      System.err.println("Exception when calling TeamsApi#deleteTeamTeamsTeamIdDelete");
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
| **teamId** | **String**|  | |

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
| **204** | Team deleted successfully |  -  |
| **404** | Team not found |  -  |
| **422** | Validation Error |  -  |

<a id="downloadTeamLogoTeamsTeamIdLogoFileIdGet"></a>
# **downloadTeamLogoTeamsTeamIdLogoFileIdGet**
> Object downloadTeamLogoTeamsTeamIdLogoFileIdGet(teamId, fileId)

Download team logo

Download a team&#39;s logo by file ID.

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.TeamsApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://believe.cjav.dev");
    
    // Configure HTTP bearer authorization: HTTPBearer
    HttpBearerAuth HTTPBearer = (HttpBearerAuth) defaultClient.getAuthentication("HTTPBearer");
    HTTPBearer.setBearerToken("BEARER TOKEN");

    TeamsApi apiInstance = new TeamsApi(defaultClient);
    String teamId = "teamId_example"; // String | 
    UUID fileId = UUID.randomUUID(); // UUID | 
    try {
      Object result = apiInstance.downloadTeamLogoTeamsTeamIdLogoFileIdGet(teamId, fileId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling TeamsApi#downloadTeamLogoTeamsTeamIdLogoFileIdGet");
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
| **teamId** | **String**|  | |
| **fileId** | **UUID**|  | |

### Return type

**Object**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, image/*

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Logo file content |  -  |
| **404** | Team or file not found |  -  |
| **422** | Validation Error |  -  |

<a id="getTeamCultureTeamsTeamIdCultureGet"></a>
# **getTeamCultureTeamsTeamIdCultureGet**
> Map&lt;String, Object&gt; getTeamCultureTeamsTeamIdCultureGet(teamId)

Get team culture details

Get detailed culture and values information for a team.

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.TeamsApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://believe.cjav.dev");
    
    // Configure HTTP bearer authorization: HTTPBearer
    HttpBearerAuth HTTPBearer = (HttpBearerAuth) defaultClient.getAuthentication("HTTPBearer");
    HTTPBearer.setBearerToken("BEARER TOKEN");

    TeamsApi apiInstance = new TeamsApi(defaultClient);
    String teamId = "teamId_example"; // String | 
    try {
      Map<String, Object> result = apiInstance.getTeamCultureTeamsTeamIdCultureGet(teamId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling TeamsApi#getTeamCultureTeamsTeamIdCultureGet");
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
| **teamId** | **String**|  | |

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
| **200** | Team culture details |  -  |
| **404** | Team not found |  -  |
| **422** | Validation Error |  -  |

<a id="getTeamRivalsTeamsTeamIdRivalsGet"></a>
# **getTeamRivalsTeamsTeamIdRivalsGet**
> List&lt;Team&gt; getTeamRivalsTeamsTeamIdRivalsGet(teamId)

Get team&#39;s rivals

Get all rival teams for a specific team.

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.TeamsApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://believe.cjav.dev");
    
    // Configure HTTP bearer authorization: HTTPBearer
    HttpBearerAuth HTTPBearer = (HttpBearerAuth) defaultClient.getAuthentication("HTTPBearer");
    HTTPBearer.setBearerToken("BEARER TOKEN");

    TeamsApi apiInstance = new TeamsApi(defaultClient);
    String teamId = "teamId_example"; // String | 
    try {
      List<Team> result = apiInstance.getTeamRivalsTeamsTeamIdRivalsGet(teamId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling TeamsApi#getTeamRivalsTeamsTeamIdRivalsGet");
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
| **teamId** | **String**|  | |

### Return type

[**List&lt;Team&gt;**](Team.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of rival teams |  -  |
| **404** | Team not found |  -  |
| **422** | Validation Error |  -  |

<a id="getTeamTeamsTeamIdGet"></a>
# **getTeamTeamsTeamIdGet**
> Team getTeamTeamsTeamIdGet(teamId)

Get a team by ID

Retrieve detailed information about a specific team.

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.TeamsApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://believe.cjav.dev");
    
    // Configure HTTP bearer authorization: HTTPBearer
    HttpBearerAuth HTTPBearer = (HttpBearerAuth) defaultClient.getAuthentication("HTTPBearer");
    HTTPBearer.setBearerToken("BEARER TOKEN");

    TeamsApi apiInstance = new TeamsApi(defaultClient);
    String teamId = "teamId_example"; // String | 
    try {
      Team result = apiInstance.getTeamTeamsTeamIdGet(teamId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling TeamsApi#getTeamTeamsTeamIdGet");
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
| **teamId** | **String**|  | |

### Return type

[**Team**](Team.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Team details |  -  |
| **404** | Team not found |  -  |
| **422** | Validation Error |  -  |

<a id="listTeamLogosTeamsTeamIdLogosGet"></a>
# **listTeamLogosTeamsTeamIdLogosGet**
> List&lt;FileUploadResponse&gt; listTeamLogosTeamsTeamIdLogosGet(teamId)

List team logos

List all uploaded logos for a team.

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.TeamsApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://believe.cjav.dev");
    
    // Configure HTTP bearer authorization: HTTPBearer
    HttpBearerAuth HTTPBearer = (HttpBearerAuth) defaultClient.getAuthentication("HTTPBearer");
    HTTPBearer.setBearerToken("BEARER TOKEN");

    TeamsApi apiInstance = new TeamsApi(defaultClient);
    String teamId = "teamId_example"; // String | 
    try {
      List<FileUploadResponse> result = apiInstance.listTeamLogosTeamsTeamIdLogosGet(teamId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling TeamsApi#listTeamLogosTeamsTeamIdLogosGet");
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
| **teamId** | **String**|  | |

### Return type

[**List&lt;FileUploadResponse&gt;**](FileUploadResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Successful Response |  -  |
| **422** | Validation Error |  -  |

<a id="listTeamsTeamsGet"></a>
# **listTeamsTeamsGet**
> PaginatedResponseTeam listTeamsTeamsGet(league, minCultureScore, skip, limit)

List all teams

Get a paginated list of all teams with optional filtering by league or culture score.

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.TeamsApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://believe.cjav.dev");
    
    // Configure HTTP bearer authorization: HTTPBearer
    HttpBearerAuth HTTPBearer = (HttpBearerAuth) defaultClient.getAuthentication("HTTPBearer");
    HTTPBearer.setBearerToken("BEARER TOKEN");

    TeamsApi apiInstance = new TeamsApi(defaultClient);
    League league = League.fromValue("Premier League"); // League | Filter by league
    Integer minCultureScore = 56; // Integer | Minimum culture score
    Integer skip = 0; // Integer | Number of items to skip (offset)
    Integer limit = 20; // Integer | Maximum number of items to return (max: 100)
    try {
      PaginatedResponseTeam result = apiInstance.listTeamsTeamsGet(league, minCultureScore, skip, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling TeamsApi#listTeamsTeamsGet");
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
| **league** | [**League**](.md)| Filter by league | [optional] [enum: Premier League, Championship, League One, League Two, La Liga, Serie A, Bundesliga, Ligue 1] |
| **minCultureScore** | **Integer**| Minimum culture score | [optional] |
| **skip** | **Integer**| Number of items to skip (offset) | [optional] [default to 0] |
| **limit** | **Integer**| Maximum number of items to return (max: 100) | [optional] [default to 20] |

### Return type

[**PaginatedResponseTeam**](PaginatedResponseTeam.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Paginated list of teams |  -  |
| **422** | Validation Error |  -  |

<a id="updateTeamTeamsTeamIdPatch"></a>
# **updateTeamTeamsTeamIdPatch**
> Team updateTeamTeamsTeamIdPatch(teamId, teamUpdate)

Update a team

Update specific fields of an existing team.

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.TeamsApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://believe.cjav.dev");
    
    // Configure HTTP bearer authorization: HTTPBearer
    HttpBearerAuth HTTPBearer = (HttpBearerAuth) defaultClient.getAuthentication("HTTPBearer");
    HTTPBearer.setBearerToken("BEARER TOKEN");

    TeamsApi apiInstance = new TeamsApi(defaultClient);
    String teamId = "teamId_example"; // String | 
    TeamUpdate teamUpdate = new TeamUpdate(); // TeamUpdate | 
    try {
      Team result = apiInstance.updateTeamTeamsTeamIdPatch(teamId, teamUpdate);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling TeamsApi#updateTeamTeamsTeamIdPatch");
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
| **teamId** | **String**|  | |
| **teamUpdate** | [**TeamUpdate**](TeamUpdate.md)|  | |

### Return type

[**Team**](Team.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Team updated successfully |  -  |
| **404** | Team not found |  -  |
| **422** | Validation Error |  -  |

<a id="uploadTeamLogoTeamsTeamIdLogoPost"></a>
# **uploadTeamLogoTeamsTeamIdLogoPost**
> FileUploadResponse uploadTeamLogoTeamsTeamIdLogoPost(teamId, _file)

Upload team logo

Upload a logo image for a team. Accepts image files (jpg, png, gif, webp).

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.TeamsApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://believe.cjav.dev");
    
    // Configure HTTP bearer authorization: HTTPBearer
    HttpBearerAuth HTTPBearer = (HttpBearerAuth) defaultClient.getAuthentication("HTTPBearer");
    HTTPBearer.setBearerToken("BEARER TOKEN");

    TeamsApi apiInstance = new TeamsApi(defaultClient);
    String teamId = "teamId_example"; // String | 
    File _file = new File("/path/to/file"); // File | Logo image file
    try {
      FileUploadResponse result = apiInstance.uploadTeamLogoTeamsTeamIdLogoPost(teamId, _file);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling TeamsApi#uploadTeamLogoTeamsTeamIdLogoPost");
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
| **teamId** | **String**|  | |
| **_file** | **File**| Logo image file | |

### Return type

[**FileUploadResponse**](FileUploadResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Logo uploaded successfully |  -  |
| **404** | Team not found |  -  |
| **415** | Unsupported file type |  -  |
| **422** | Validation Error |  -  |

