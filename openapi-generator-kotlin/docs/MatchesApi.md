# MatchesApi

All URIs are relative to *https://believe.cjav.dev*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
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
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MatchesApi()
val matchCreate : MatchCreate =  // MatchCreate | 
try {
    val result : Match = apiInstance.createMatchMatchesPost(matchCreate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MatchesApi#createMatchMatchesPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MatchesApi#createMatchMatchesPost")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **matchCreate** | [**MatchCreate**](MatchCreate.md)|  | |

### Return type

[**Match**](Match.md)

### Authorization


Configure HTTPBearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="deleteMatchMatchesMatchIdDelete"></a>
# **deleteMatchMatchesMatchIdDelete**
> deleteMatchMatchesMatchIdDelete(matchId)

Delete a match

Remove a match from the database.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MatchesApi()
val matchId : kotlin.String = matchId_example // kotlin.String | 
try {
    apiInstance.deleteMatchMatchesMatchIdDelete(matchId)
} catch (e: ClientException) {
    println("4xx response calling MatchesApi#deleteMatchMatchesMatchIdDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MatchesApi#deleteMatchMatchesMatchIdDelete")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **matchId** | **kotlin.String**|  | |

### Return type

null (empty response body)

### Authorization


Configure HTTPBearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="getMatchLessonMatchesMatchIdLessonGet"></a>
# **getMatchLessonMatchesMatchIdLessonGet**
> kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt; getMatchLessonMatchesMatchIdLessonGet(matchId)

Get match lesson

Get the life lesson learned from a specific match.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MatchesApi()
val matchId : kotlin.String = matchId_example // kotlin.String | 
try {
    val result : kotlin.collections.Map<kotlin.String, kotlin.Any> = apiInstance.getMatchLessonMatchesMatchIdLessonGet(matchId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MatchesApi#getMatchLessonMatchesMatchIdLessonGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MatchesApi#getMatchLessonMatchesMatchIdLessonGet")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **matchId** | **kotlin.String**|  | |

### Return type

[**kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt;**](kotlin.Any.md)

### Authorization


Configure HTTPBearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="getMatchMatchesMatchIdGet"></a>
# **getMatchMatchesMatchIdGet**
> Match getMatchMatchesMatchIdGet(matchId)

Get a match by ID

Retrieve detailed information about a specific match.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MatchesApi()
val matchId : kotlin.String = matchId_example // kotlin.String | 
try {
    val result : Match = apiInstance.getMatchMatchesMatchIdGet(matchId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MatchesApi#getMatchMatchesMatchIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MatchesApi#getMatchMatchesMatchIdGet")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **matchId** | **kotlin.String**|  | |

### Return type

[**Match**](Match.md)

### Authorization


Configure HTTPBearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="getTurningPointsMatchesMatchIdTurningPointsGet"></a>
# **getTurningPointsMatchesMatchIdTurningPointsGet**
> kotlin.collections.List&lt;kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt;&gt; getTurningPointsMatchesMatchIdTurningPointsGet(matchId)

Get match turning points

Get all turning points from a specific match.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MatchesApi()
val matchId : kotlin.String = matchId_example // kotlin.String | 
try {
    val result : kotlin.collections.List<kotlin.collections.Map<kotlin.String, kotlin.Any>> = apiInstance.getTurningPointsMatchesMatchIdTurningPointsGet(matchId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MatchesApi#getTurningPointsMatchesMatchIdTurningPointsGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MatchesApi#getTurningPointsMatchesMatchIdTurningPointsGet")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **matchId** | **kotlin.String**|  | |

### Return type

**kotlin.collections.List&lt;kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt;&gt;**

### Authorization


Configure HTTPBearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="listMatchesMatchesGet"></a>
# **listMatchesMatchesGet**
> PaginatedResponseMatch listMatchesMatchesGet(teamId, result, matchType, skip, limit)

List all matches

Get a paginated list of all matches with optional filtering.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MatchesApi()
val teamId : kotlin.String = teamId_example // kotlin.String | Filter by team (home or away)
val result : MatchResult =  // MatchResult | Filter by result
val matchType : MatchType =  // MatchType | Filter by match type
val skip : kotlin.Int = 56 // kotlin.Int | Number of items to skip (offset)
val limit : kotlin.Int = 56 // kotlin.Int | Maximum number of items to return (max: 100)
try {
    val result : PaginatedResponseMatch = apiInstance.listMatchesMatchesGet(teamId, result, matchType, skip, limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MatchesApi#listMatchesMatchesGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MatchesApi#listMatchesMatchesGet")
    e.printStackTrace()
}
```

### Parameters
| **teamId** | **kotlin.String**| Filter by team (home or away) | [optional] |
| **result** | [**MatchResult**](.md)| Filter by result | [optional] [enum: win, loss, draw, pending] |
| **matchType** | [**MatchType**](.md)| Filter by match type | [optional] [enum: league, cup, friendly, playoff, final] |
| **skip** | **kotlin.Int**| Number of items to skip (offset) | [optional] [default to 0] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.Int**| Maximum number of items to return (max: 100) | [optional] [default to 20] |

### Return type

[**PaginatedResponseMatch**](PaginatedResponseMatch.md)

### Authorization


Configure HTTPBearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="updateMatchMatchesMatchIdPatch"></a>
# **updateMatchMatchesMatchIdPatch**
> Match updateMatchMatchesMatchIdPatch(matchId, matchUpdate)

Update a match

Update specific fields of an existing match (e.g., update score).

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MatchesApi()
val matchId : kotlin.String = matchId_example // kotlin.String | 
val matchUpdate : MatchUpdate =  // MatchUpdate | 
try {
    val result : Match = apiInstance.updateMatchMatchesMatchIdPatch(matchId, matchUpdate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MatchesApi#updateMatchMatchesMatchIdPatch")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MatchesApi#updateMatchMatchesMatchIdPatch")
    e.printStackTrace()
}
```

### Parameters
| **matchId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **matchUpdate** | [**MatchUpdate**](MatchUpdate.md)|  | |

### Return type

[**Match**](Match.md)

### Authorization


Configure HTTPBearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

