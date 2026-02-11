# TeamsApi

All URIs are relative to *https://believe.cjav.dev*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
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
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = TeamsApi()
val teamCreate : TeamCreate =  // TeamCreate | 
try {
    val result : Team = apiInstance.createTeamTeamsPost(teamCreate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TeamsApi#createTeamTeamsPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TeamsApi#createTeamTeamsPost")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **teamCreate** | [**TeamCreate**](TeamCreate.md)|  | |

### Return type

[**Team**](Team.md)

### Authorization


Configure HTTPBearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="deleteTeamLogoTeamsTeamIdLogoFileIdDelete"></a>
# **deleteTeamLogoTeamsTeamIdLogoFileIdDelete**
> deleteTeamLogoTeamsTeamIdLogoFileIdDelete(teamId, fileId)

Delete team logo

Delete a team&#39;s logo.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = TeamsApi()
val teamId : kotlin.String = teamId_example // kotlin.String | 
val fileId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    apiInstance.deleteTeamLogoTeamsTeamIdLogoFileIdDelete(teamId, fileId)
} catch (e: ClientException) {
    println("4xx response calling TeamsApi#deleteTeamLogoTeamsTeamIdLogoFileIdDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TeamsApi#deleteTeamLogoTeamsTeamIdLogoFileIdDelete")
    e.printStackTrace()
}
```

### Parameters
| **teamId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **fileId** | **java.util.UUID**|  | |

### Return type

null (empty response body)

### Authorization


Configure HTTPBearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="deleteTeamTeamsTeamIdDelete"></a>
# **deleteTeamTeamsTeamIdDelete**
> deleteTeamTeamsTeamIdDelete(teamId)

Delete a team

Remove a team from the database (relegation to oblivion).

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = TeamsApi()
val teamId : kotlin.String = teamId_example // kotlin.String | 
try {
    apiInstance.deleteTeamTeamsTeamIdDelete(teamId)
} catch (e: ClientException) {
    println("4xx response calling TeamsApi#deleteTeamTeamsTeamIdDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TeamsApi#deleteTeamTeamsTeamIdDelete")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **teamId** | **kotlin.String**|  | |

### Return type

null (empty response body)

### Authorization


Configure HTTPBearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="downloadTeamLogoTeamsTeamIdLogoFileIdGet"></a>
# **downloadTeamLogoTeamsTeamIdLogoFileIdGet**
> kotlin.Any downloadTeamLogoTeamsTeamIdLogoFileIdGet(teamId, fileId)

Download team logo

Download a team&#39;s logo by file ID.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = TeamsApi()
val teamId : kotlin.String = teamId_example // kotlin.String | 
val fileId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : kotlin.Any = apiInstance.downloadTeamLogoTeamsTeamIdLogoFileIdGet(teamId, fileId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TeamsApi#downloadTeamLogoTeamsTeamIdLogoFileIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TeamsApi#downloadTeamLogoTeamsTeamIdLogoFileIdGet")
    e.printStackTrace()
}
```

### Parameters
| **teamId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **fileId** | **java.util.UUID**|  | |

### Return type

[**kotlin.Any**](kotlin.Any.md)

### Authorization


Configure HTTPBearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="getTeamCultureTeamsTeamIdCultureGet"></a>
# **getTeamCultureTeamsTeamIdCultureGet**
> kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt; getTeamCultureTeamsTeamIdCultureGet(teamId)

Get team culture details

Get detailed culture and values information for a team.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = TeamsApi()
val teamId : kotlin.String = teamId_example // kotlin.String | 
try {
    val result : kotlin.collections.Map<kotlin.String, kotlin.Any> = apiInstance.getTeamCultureTeamsTeamIdCultureGet(teamId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TeamsApi#getTeamCultureTeamsTeamIdCultureGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TeamsApi#getTeamCultureTeamsTeamIdCultureGet")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **teamId** | **kotlin.String**|  | |

### Return type

[**kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt;**](kotlin.Any.md)

### Authorization


Configure HTTPBearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="getTeamRivalsTeamsTeamIdRivalsGet"></a>
# **getTeamRivalsTeamsTeamIdRivalsGet**
> kotlin.collections.List&lt;Team&gt; getTeamRivalsTeamsTeamIdRivalsGet(teamId)

Get team&#39;s rivals

Get all rival teams for a specific team.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = TeamsApi()
val teamId : kotlin.String = teamId_example // kotlin.String | 
try {
    val result : kotlin.collections.List<Team> = apiInstance.getTeamRivalsTeamsTeamIdRivalsGet(teamId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TeamsApi#getTeamRivalsTeamsTeamIdRivalsGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TeamsApi#getTeamRivalsTeamsTeamIdRivalsGet")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **teamId** | **kotlin.String**|  | |

### Return type

[**kotlin.collections.List&lt;Team&gt;**](Team.md)

### Authorization


Configure HTTPBearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="getTeamTeamsTeamIdGet"></a>
# **getTeamTeamsTeamIdGet**
> Team getTeamTeamsTeamIdGet(teamId)

Get a team by ID

Retrieve detailed information about a specific team.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = TeamsApi()
val teamId : kotlin.String = teamId_example // kotlin.String | 
try {
    val result : Team = apiInstance.getTeamTeamsTeamIdGet(teamId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TeamsApi#getTeamTeamsTeamIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TeamsApi#getTeamTeamsTeamIdGet")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **teamId** | **kotlin.String**|  | |

### Return type

[**Team**](Team.md)

### Authorization


Configure HTTPBearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="listTeamLogosTeamsTeamIdLogosGet"></a>
# **listTeamLogosTeamsTeamIdLogosGet**
> kotlin.collections.List&lt;FileUploadResponse&gt; listTeamLogosTeamsTeamIdLogosGet(teamId)

List team logos

List all uploaded logos for a team.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = TeamsApi()
val teamId : kotlin.String = teamId_example // kotlin.String | 
try {
    val result : kotlin.collections.List<FileUploadResponse> = apiInstance.listTeamLogosTeamsTeamIdLogosGet(teamId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TeamsApi#listTeamLogosTeamsTeamIdLogosGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TeamsApi#listTeamLogosTeamsTeamIdLogosGet")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **teamId** | **kotlin.String**|  | |

### Return type

[**kotlin.collections.List&lt;FileUploadResponse&gt;**](FileUploadResponse.md)

### Authorization


Configure HTTPBearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="listTeamsTeamsGet"></a>
# **listTeamsTeamsGet**
> PaginatedResponseTeam listTeamsTeamsGet(league, minCultureScore, skip, limit)

List all teams

Get a paginated list of all teams with optional filtering by league or culture score.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = TeamsApi()
val league : League =  // League | Filter by league
val minCultureScore : kotlin.Int = 56 // kotlin.Int | Minimum culture score
val skip : kotlin.Int = 56 // kotlin.Int | Number of items to skip (offset)
val limit : kotlin.Int = 56 // kotlin.Int | Maximum number of items to return (max: 100)
try {
    val result : PaginatedResponseTeam = apiInstance.listTeamsTeamsGet(league, minCultureScore, skip, limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TeamsApi#listTeamsTeamsGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TeamsApi#listTeamsTeamsGet")
    e.printStackTrace()
}
```

### Parameters
| **league** | [**League**](.md)| Filter by league | [optional] [enum: Premier League, Championship, League One, League Two, La Liga, Serie A, Bundesliga, Ligue 1] |
| **minCultureScore** | **kotlin.Int**| Minimum culture score | [optional] |
| **skip** | **kotlin.Int**| Number of items to skip (offset) | [optional] [default to 0] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.Int**| Maximum number of items to return (max: 100) | [optional] [default to 20] |

### Return type

[**PaginatedResponseTeam**](PaginatedResponseTeam.md)

### Authorization


Configure HTTPBearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="updateTeamTeamsTeamIdPatch"></a>
# **updateTeamTeamsTeamIdPatch**
> Team updateTeamTeamsTeamIdPatch(teamId, teamUpdate)

Update a team

Update specific fields of an existing team.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = TeamsApi()
val teamId : kotlin.String = teamId_example // kotlin.String | 
val teamUpdate : TeamUpdate =  // TeamUpdate | 
try {
    val result : Team = apiInstance.updateTeamTeamsTeamIdPatch(teamId, teamUpdate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TeamsApi#updateTeamTeamsTeamIdPatch")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TeamsApi#updateTeamTeamsTeamIdPatch")
    e.printStackTrace()
}
```

### Parameters
| **teamId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **teamUpdate** | [**TeamUpdate**](TeamUpdate.md)|  | |

### Return type

[**Team**](Team.md)

### Authorization


Configure HTTPBearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="uploadTeamLogoTeamsTeamIdLogoPost"></a>
# **uploadTeamLogoTeamsTeamIdLogoPost**
> FileUploadResponse uploadTeamLogoTeamsTeamIdLogoPost(teamId, file)

Upload team logo

Upload a logo image for a team. Accepts image files (jpg, png, gif, webp).

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = TeamsApi()
val teamId : kotlin.String = teamId_example // kotlin.String | 
val file : java.io.File = BINARY_DATA_HERE // java.io.File | Logo image file
try {
    val result : FileUploadResponse = apiInstance.uploadTeamLogoTeamsTeamIdLogoPost(teamId, file)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TeamsApi#uploadTeamLogoTeamsTeamIdLogoPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TeamsApi#uploadTeamLogoTeamsTeamIdLogoPost")
    e.printStackTrace()
}
```

### Parameters
| **teamId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **file** | **java.io.File**| Logo image file | |

### Return type

[**FileUploadResponse**](FileUploadResponse.md)

### Authorization


Configure HTTPBearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json

