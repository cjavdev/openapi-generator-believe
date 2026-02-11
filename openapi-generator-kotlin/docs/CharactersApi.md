# CharactersApi

All URIs are relative to *https://believe.cjav.dev*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
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
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = CharactersApi()
val characterCreate : CharacterCreate =  // CharacterCreate | 
try {
    val result : Character = apiInstance.createCharacterCharactersPost(characterCreate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CharactersApi#createCharacterCharactersPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CharactersApi#createCharacterCharactersPost")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **characterCreate** | [**CharacterCreate**](CharacterCreate.md)|  | |

### Return type

[**Character**](Character.md)

### Authorization


Configure HTTPBearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="deleteCharacterCharactersCharacterIdDelete"></a>
# **deleteCharacterCharactersCharacterIdDelete**
> deleteCharacterCharactersCharacterIdDelete(characterId)

Delete a character

Remove a character from the database.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = CharactersApi()
val characterId : kotlin.String = characterId_example // kotlin.String | 
try {
    apiInstance.deleteCharacterCharactersCharacterIdDelete(characterId)
} catch (e: ClientException) {
    println("4xx response calling CharactersApi#deleteCharacterCharactersCharacterIdDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CharactersApi#deleteCharacterCharactersCharacterIdDelete")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **characterId** | **kotlin.String**|  | |

### Return type

null (empty response body)

### Authorization


Configure HTTPBearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="getCharacterCharactersCharacterIdGet"></a>
# **getCharacterCharactersCharacterIdGet**
> Character getCharacterCharactersCharacterIdGet(characterId)

Get a character by ID

Retrieve detailed information about a specific character.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = CharactersApi()
val characterId : kotlin.String = characterId_example // kotlin.String | 
try {
    val result : Character = apiInstance.getCharacterCharactersCharacterIdGet(characterId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CharactersApi#getCharacterCharactersCharacterIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CharactersApi#getCharacterCharactersCharacterIdGet")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **characterId** | **kotlin.String**|  | |

### Return type

[**Character**](Character.md)

### Authorization


Configure HTTPBearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="getCharacterQuotesCharactersCharacterIdQuotesGet"></a>
# **getCharacterQuotesCharactersCharacterIdQuotesGet**
> kotlin.collections.List&lt;kotlin.String?&gt; getCharacterQuotesCharactersCharacterIdQuotesGet(characterId)

Get character&#39;s signature quotes

Get all signature quotes from a specific character.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = CharactersApi()
val characterId : kotlin.String = characterId_example // kotlin.String | 
try {
    val result : kotlin.collections.List<kotlin.String?> = apiInstance.getCharacterQuotesCharactersCharacterIdQuotesGet(characterId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CharactersApi#getCharacterQuotesCharactersCharacterIdQuotesGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CharactersApi#getCharacterQuotesCharactersCharacterIdQuotesGet")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **characterId** | **kotlin.String**|  | |

### Return type

**kotlin.collections.List&lt;kotlin.String?&gt;**

### Authorization


Configure HTTPBearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="listCharactersCharactersGet"></a>
# **listCharactersCharactersGet**
> PaginatedResponseCharacter listCharactersCharactersGet(role, teamId, minOptimism, skip, limit)

List all characters

Get a paginated list of Ted Lasso characters.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = CharactersApi()
val role : CharacterRole =  // CharacterRole | Filter by role
val teamId : kotlin.String = teamId_example // kotlin.String | Filter by team ID
val minOptimism : kotlin.Int = 56 // kotlin.Int | Minimum optimism score
val skip : kotlin.Int = 56 // kotlin.Int | Number of items to skip (offset)
val limit : kotlin.Int = 56 // kotlin.Int | Maximum number of items to return (max: 100)
try {
    val result : PaginatedResponseCharacter = apiInstance.listCharactersCharactersGet(role, teamId, minOptimism, skip, limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CharactersApi#listCharactersCharactersGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CharactersApi#listCharactersCharactersGet")
    e.printStackTrace()
}
```

### Parameters
| **role** | [**CharacterRole**](.md)| Filter by role | [optional] [enum: coach, player, owner, manager, staff, journalist, family, friend, fan, other] |
| **teamId** | **kotlin.String**| Filter by team ID | [optional] |
| **minOptimism** | **kotlin.Int**| Minimum optimism score | [optional] |
| **skip** | **kotlin.Int**| Number of items to skip (offset) | [optional] [default to 0] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.Int**| Maximum number of items to return (max: 100) | [optional] [default to 20] |

### Return type

[**PaginatedResponseCharacter**](PaginatedResponseCharacter.md)

### Authorization


Configure HTTPBearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="updateCharacterCharactersCharacterIdPatch"></a>
# **updateCharacterCharactersCharacterIdPatch**
> Character updateCharacterCharactersCharacterIdPatch(characterId, characterUpdate)

Update a character

Update specific fields of an existing character.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = CharactersApi()
val characterId : kotlin.String = characterId_example // kotlin.String | 
val characterUpdate : CharacterUpdate =  // CharacterUpdate | 
try {
    val result : Character = apiInstance.updateCharacterCharactersCharacterIdPatch(characterId, characterUpdate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CharactersApi#updateCharacterCharactersCharacterIdPatch")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CharactersApi#updateCharacterCharactersCharacterIdPatch")
    e.printStackTrace()
}
```

### Parameters
| **characterId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **characterUpdate** | [**CharacterUpdate**](CharacterUpdate.md)|  | |

### Return type

[**Character**](Character.md)

### Authorization


Configure HTTPBearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

