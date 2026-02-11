# CharactersApi

All URIs are relative to *https://believe.cjav.dev*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createCharacterCharactersPost**](CharactersApi.md#createCharacterCharactersPost) | **POST** /characters | Create a new character |
| [**deleteCharacterCharactersCharacterIdDelete**](CharactersApi.md#deleteCharacterCharactersCharacterIdDelete) | **DELETE** /characters/{character_id} | Delete a character |
| [**getCharacterCharactersCharacterIdGet**](CharactersApi.md#getCharacterCharactersCharacterIdGet) | **GET** /characters/{character_id} | Get a character by ID |
| [**getCharacterQuotesCharactersCharacterIdQuotesGet**](CharactersApi.md#getCharacterQuotesCharactersCharacterIdQuotesGet) | **GET** /characters/{character_id}/quotes | Get character&#39;s signature quotes |
| [**listCharactersCharactersGet**](CharactersApi.md#listCharactersCharactersGet) | **GET** /characters | List all characters |
| [**updateCharacterCharactersCharacterIdPatch**](CharactersApi.md#updateCharacterCharactersCharacterIdPatch) | **PATCH** /characters/{character_id} | Update a character |


<a id="createCharacterCharactersPost"></a>
# **createCharacterCharactersPost**
> Character createCharacterCharactersPost(characterCreate)

Create a new character

Add a new character to the Ted Lasso universe.

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.CharactersApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://believe.cjav.dev");
    
    // Configure HTTP bearer authorization: HTTPBearer
    HttpBearerAuth HTTPBearer = (HttpBearerAuth) defaultClient.getAuthentication("HTTPBearer");
    HTTPBearer.setBearerToken("BEARER TOKEN");

    CharactersApi apiInstance = new CharactersApi(defaultClient);
    CharacterCreate characterCreate = new CharacterCreate(); // CharacterCreate | 
    try {
      Character result = apiInstance.createCharacterCharactersPost(characterCreate);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling CharactersApi#createCharacterCharactersPost");
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
| **characterCreate** | [**CharacterCreate**](CharacterCreate.md)|  | |

### Return type

[**Character**](Character.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Character created successfully |  -  |
| **409** | Character already exists |  -  |
| **422** | Validation Error |  -  |

<a id="deleteCharacterCharactersCharacterIdDelete"></a>
# **deleteCharacterCharactersCharacterIdDelete**
> deleteCharacterCharactersCharacterIdDelete(characterId)

Delete a character

Remove a character from the database.

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.CharactersApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://believe.cjav.dev");
    
    // Configure HTTP bearer authorization: HTTPBearer
    HttpBearerAuth HTTPBearer = (HttpBearerAuth) defaultClient.getAuthentication("HTTPBearer");
    HTTPBearer.setBearerToken("BEARER TOKEN");

    CharactersApi apiInstance = new CharactersApi(defaultClient);
    String characterId = "characterId_example"; // String | 
    try {
      apiInstance.deleteCharacterCharactersCharacterIdDelete(characterId);
    } catch (ApiException e) {
      System.err.println("Exception when calling CharactersApi#deleteCharacterCharactersCharacterIdDelete");
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
| **204** | Character deleted successfully |  -  |
| **404** | Character not found |  -  |
| **422** | Validation Error |  -  |

<a id="getCharacterCharactersCharacterIdGet"></a>
# **getCharacterCharactersCharacterIdGet**
> Character getCharacterCharactersCharacterIdGet(characterId)

Get a character by ID

Retrieve detailed information about a specific character.

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.CharactersApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://believe.cjav.dev");
    
    // Configure HTTP bearer authorization: HTTPBearer
    HttpBearerAuth HTTPBearer = (HttpBearerAuth) defaultClient.getAuthentication("HTTPBearer");
    HTTPBearer.setBearerToken("BEARER TOKEN");

    CharactersApi apiInstance = new CharactersApi(defaultClient);
    String characterId = "characterId_example"; // String | 
    try {
      Character result = apiInstance.getCharacterCharactersCharacterIdGet(characterId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling CharactersApi#getCharacterCharactersCharacterIdGet");
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

### Return type

[**Character**](Character.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Character details |  -  |
| **404** | Character not found |  -  |
| **422** | Validation Error |  -  |

<a id="getCharacterQuotesCharactersCharacterIdQuotesGet"></a>
# **getCharacterQuotesCharactersCharacterIdQuotesGet**
> List&lt;String&gt; getCharacterQuotesCharactersCharacterIdQuotesGet(characterId)

Get character&#39;s signature quotes

Get all signature quotes from a specific character.

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.CharactersApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://believe.cjav.dev");
    
    // Configure HTTP bearer authorization: HTTPBearer
    HttpBearerAuth HTTPBearer = (HttpBearerAuth) defaultClient.getAuthentication("HTTPBearer");
    HTTPBearer.setBearerToken("BEARER TOKEN");

    CharactersApi apiInstance = new CharactersApi(defaultClient);
    String characterId = "characterId_example"; // String | 
    try {
      List<String> result = apiInstance.getCharacterQuotesCharactersCharacterIdQuotesGet(characterId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling CharactersApi#getCharacterQuotesCharactersCharacterIdQuotesGet");
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

### Return type

**List&lt;String&gt;**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of signature quotes |  -  |
| **404** | Character not found |  -  |
| **422** | Validation Error |  -  |

<a id="listCharactersCharactersGet"></a>
# **listCharactersCharactersGet**
> PaginatedResponseCharacter listCharactersCharactersGet(role, teamId, minOptimism, skip, limit)

List all characters

Get a paginated list of Ted Lasso characters.

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.CharactersApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://believe.cjav.dev");
    
    // Configure HTTP bearer authorization: HTTPBearer
    HttpBearerAuth HTTPBearer = (HttpBearerAuth) defaultClient.getAuthentication("HTTPBearer");
    HTTPBearer.setBearerToken("BEARER TOKEN");

    CharactersApi apiInstance = new CharactersApi(defaultClient);
    CharacterRole role = CharacterRole.fromValue("coach"); // CharacterRole | Filter by role
    String teamId = "teamId_example"; // String | Filter by team ID
    Integer minOptimism = 56; // Integer | Minimum optimism score
    Integer skip = 0; // Integer | Number of items to skip (offset)
    Integer limit = 20; // Integer | Maximum number of items to return (max: 100)
    try {
      PaginatedResponseCharacter result = apiInstance.listCharactersCharactersGet(role, teamId, minOptimism, skip, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling CharactersApi#listCharactersCharactersGet");
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
| **role** | [**CharacterRole**](.md)| Filter by role | [optional] [enum: coach, player, owner, manager, staff, journalist, family, friend, fan, other] |
| **teamId** | **String**| Filter by team ID | [optional] |
| **minOptimism** | **Integer**| Minimum optimism score | [optional] |
| **skip** | **Integer**| Number of items to skip (offset) | [optional] [default to 0] |
| **limit** | **Integer**| Maximum number of items to return (max: 100) | [optional] [default to 20] |

### Return type

[**PaginatedResponseCharacter**](PaginatedResponseCharacter.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Paginated list of characters |  -  |
| **422** | Validation Error |  -  |

<a id="updateCharacterCharactersCharacterIdPatch"></a>
# **updateCharacterCharactersCharacterIdPatch**
> Character updateCharacterCharactersCharacterIdPatch(characterId, characterUpdate)

Update a character

Update specific fields of an existing character.

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.CharactersApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://believe.cjav.dev");
    
    // Configure HTTP bearer authorization: HTTPBearer
    HttpBearerAuth HTTPBearer = (HttpBearerAuth) defaultClient.getAuthentication("HTTPBearer");
    HTTPBearer.setBearerToken("BEARER TOKEN");

    CharactersApi apiInstance = new CharactersApi(defaultClient);
    String characterId = "characterId_example"; // String | 
    CharacterUpdate characterUpdate = new CharacterUpdate(); // CharacterUpdate | 
    try {
      Character result = apiInstance.updateCharacterCharactersCharacterIdPatch(characterId, characterUpdate);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling CharactersApi#updateCharacterCharactersCharacterIdPatch");
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
| **characterUpdate** | [**CharacterUpdate**](CharacterUpdate.md)|  | |

### Return type

[**Character**](Character.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Character updated successfully |  -  |
| **404** | Character not found |  -  |
| **422** | Validation Error |  -  |

