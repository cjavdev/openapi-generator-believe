# EpisodesApi

All URIs are relative to *https://believe.cjav.dev*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
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
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = EpisodesApi()
val episodeCreate : EpisodeCreate =  // EpisodeCreate | 
try {
    val result : Episode = apiInstance.createEpisodeEpisodesPost(episodeCreate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EpisodesApi#createEpisodeEpisodesPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EpisodesApi#createEpisodeEpisodesPost")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **episodeCreate** | [**EpisodeCreate**](EpisodeCreate.md)|  | |

### Return type

[**Episode**](Episode.md)

### Authorization


Configure HTTPBearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="deleteEpisodeEpisodesEpisodeIdDelete"></a>
# **deleteEpisodeEpisodesEpisodeIdDelete**
> deleteEpisodeEpisodesEpisodeIdDelete(episodeId)

Delete an episode

Remove an episode from the database.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = EpisodesApi()
val episodeId : kotlin.String = episodeId_example // kotlin.String | 
try {
    apiInstance.deleteEpisodeEpisodesEpisodeIdDelete(episodeId)
} catch (e: ClientException) {
    println("4xx response calling EpisodesApi#deleteEpisodeEpisodesEpisodeIdDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EpisodesApi#deleteEpisodeEpisodesEpisodeIdDelete")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **episodeId** | **kotlin.String**|  | |

### Return type

null (empty response body)

### Authorization


Configure HTTPBearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="getEpisodeEpisodesEpisodeIdGet"></a>
# **getEpisodeEpisodesEpisodeIdGet**
> Episode getEpisodeEpisodesEpisodeIdGet(episodeId)

Get an episode by ID

Retrieve detailed information about a specific episode.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = EpisodesApi()
val episodeId : kotlin.String = episodeId_example // kotlin.String | 
try {
    val result : Episode = apiInstance.getEpisodeEpisodesEpisodeIdGet(episodeId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EpisodesApi#getEpisodeEpisodesEpisodeIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EpisodesApi#getEpisodeEpisodesEpisodeIdGet")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **episodeId** | **kotlin.String**|  | |

### Return type

[**Episode**](Episode.md)

### Authorization


Configure HTTPBearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="getEpisodeWisdomEpisodesEpisodeIdWisdomGet"></a>
# **getEpisodeWisdomEpisodesEpisodeIdWisdomGet**
> kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt; getEpisodeWisdomEpisodesEpisodeIdWisdomGet(episodeId)

Get episode wisdom

Get Ted&#39;s wisdom and memorable moments from a specific episode.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = EpisodesApi()
val episodeId : kotlin.String = episodeId_example // kotlin.String | 
try {
    val result : kotlin.collections.Map<kotlin.String, kotlin.Any> = apiInstance.getEpisodeWisdomEpisodesEpisodeIdWisdomGet(episodeId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EpisodesApi#getEpisodeWisdomEpisodesEpisodeIdWisdomGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EpisodesApi#getEpisodeWisdomEpisodesEpisodeIdWisdomGet")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **episodeId** | **kotlin.String**|  | |

### Return type

[**kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt;**](kotlin.Any.md)

### Authorization


Configure HTTPBearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="getSeasonEpisodesEpisodesSeasonsSeasonNumberGet"></a>
# **getSeasonEpisodesEpisodesSeasonsSeasonNumberGet**
> PaginatedResponseEpisode getSeasonEpisodesEpisodesSeasonsSeasonNumberGet(seasonNumber, skip, limit)

Get all episodes from a season

Get a paginated list of episodes from a specific season.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = EpisodesApi()
val seasonNumber : kotlin.Int = 56 // kotlin.Int | 
val skip : kotlin.Int = 56 // kotlin.Int | Number of items to skip (offset)
val limit : kotlin.Int = 56 // kotlin.Int | Maximum number of items to return (max: 100)
try {
    val result : PaginatedResponseEpisode = apiInstance.getSeasonEpisodesEpisodesSeasonsSeasonNumberGet(seasonNumber, skip, limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EpisodesApi#getSeasonEpisodesEpisodesSeasonsSeasonNumberGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EpisodesApi#getSeasonEpisodesEpisodesSeasonsSeasonNumberGet")
    e.printStackTrace()
}
```

### Parameters
| **seasonNumber** | **kotlin.Int**|  | |
| **skip** | **kotlin.Int**| Number of items to skip (offset) | [optional] [default to 0] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.Int**| Maximum number of items to return (max: 100) | [optional] [default to 20] |

### Return type

[**PaginatedResponseEpisode**](PaginatedResponseEpisode.md)

### Authorization


Configure HTTPBearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="listEpisodesEpisodesGet"></a>
# **listEpisodesEpisodesGet**
> PaginatedResponseEpisode listEpisodesEpisodesGet(season, characterFocus, skip, limit)

List all episodes

Get a paginated list of all Ted Lasso episodes with optional filtering by season.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = EpisodesApi()
val season : kotlin.Int = 56 // kotlin.Int | Filter by season
val characterFocus : kotlin.String = characterFocus_example // kotlin.String | Filter by character focus (character ID)
val skip : kotlin.Int = 56 // kotlin.Int | Number of items to skip (offset)
val limit : kotlin.Int = 56 // kotlin.Int | Maximum number of items to return (max: 100)
try {
    val result : PaginatedResponseEpisode = apiInstance.listEpisodesEpisodesGet(season, characterFocus, skip, limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EpisodesApi#listEpisodesEpisodesGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EpisodesApi#listEpisodesEpisodesGet")
    e.printStackTrace()
}
```

### Parameters
| **season** | **kotlin.Int**| Filter by season | [optional] |
| **characterFocus** | **kotlin.String**| Filter by character focus (character ID) | [optional] |
| **skip** | **kotlin.Int**| Number of items to skip (offset) | [optional] [default to 0] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.Int**| Maximum number of items to return (max: 100) | [optional] [default to 20] |

### Return type

[**PaginatedResponseEpisode**](PaginatedResponseEpisode.md)

### Authorization


Configure HTTPBearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="updateEpisodeEpisodesEpisodeIdPatch"></a>
# **updateEpisodeEpisodesEpisodeIdPatch**
> Episode updateEpisodeEpisodesEpisodeIdPatch(episodeId, episodeUpdate)

Update an episode

Update specific fields of an existing episode.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = EpisodesApi()
val episodeId : kotlin.String = episodeId_example // kotlin.String | 
val episodeUpdate : EpisodeUpdate =  // EpisodeUpdate | 
try {
    val result : Episode = apiInstance.updateEpisodeEpisodesEpisodeIdPatch(episodeId, episodeUpdate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EpisodesApi#updateEpisodeEpisodesEpisodeIdPatch")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EpisodesApi#updateEpisodeEpisodesEpisodeIdPatch")
    e.printStackTrace()
}
```

### Parameters
| **episodeId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **episodeUpdate** | [**EpisodeUpdate**](EpisodeUpdate.md)|  | |

### Return type

[**Episode**](Episode.md)

### Authorization


Configure HTTPBearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

