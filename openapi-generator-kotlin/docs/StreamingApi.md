# StreamingApi

All URIs are relative to *https://believe.cjav.dev*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**getPepTalkPepTalkGet**](StreamingApi.md#getPepTalkPepTalkGet) | **GET** /pep-talk | Get a Pep Talk |
| [**streamMatchCommentaryMatchesMatchIdCommentaryStreamPost**](StreamingApi.md#streamMatchCommentaryMatchesMatchIdCommentaryStreamPost) | **POST** /matches/{match_id}/commentary/stream | Stream Match Commentary |
| [**testStreamStreamTestGet**](StreamingApi.md#testStreamStreamTestGet) | **GET** /stream/test | Test SSE Connection |


<a id="getPepTalkPepTalkGet"></a>
# **getPepTalkPepTalkGet**
> PepTalkResponse getPepTalkPepTalkGet(stream)

Get a Pep Talk

Get a motivational pep talk from Ted Lasso himself. By default returns the complete pep talk. Add &#x60;?stream&#x3D;true&#x60; to get Server-Sent Events (SSE) streaming the pep talk chunk by chunk.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = StreamingApi()
val stream : kotlin.Boolean = true // kotlin.Boolean | If true, returns SSE stream instead of full response
try {
    val result : PepTalkResponse = apiInstance.getPepTalkPepTalkGet(stream)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StreamingApi#getPepTalkPepTalkGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StreamingApi#getPepTalkPepTalkGet")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **stream** | **kotlin.Boolean**| If true, returns SSE stream instead of full response | [optional] [default to false] |

### Return type

[**PepTalkResponse**](PepTalkResponse.md)

### Authorization


Configure HTTPBearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="streamMatchCommentaryMatchesMatchIdCommentaryStreamPost"></a>
# **streamMatchCommentaryMatchesMatchIdCommentaryStreamPost**
> kotlin.Any streamMatchCommentaryMatchesMatchIdCommentaryStreamPost(matchId)

Stream Match Commentary

Stream live match commentary for a specific match. Uses Server-Sent Events (SSE) to stream commentary events in real-time.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = StreamingApi()
val matchId : kotlin.String = matchId_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.streamMatchCommentaryMatchesMatchIdCommentaryStreamPost(matchId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StreamingApi#streamMatchCommentaryMatchesMatchIdCommentaryStreamPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StreamingApi#streamMatchCommentaryMatchesMatchIdCommentaryStreamPost")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **matchId** | **kotlin.String**|  | |

### Return type

[**kotlin.Any**](kotlin.Any.md)

### Authorization


Configure HTTPBearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="testStreamStreamTestGet"></a>
# **testStreamStreamTestGet**
> kotlin.Any testStreamStreamTestGet()

Test SSE Connection

A simple SSE test endpoint that streams numbers 1-5.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = StreamingApi()
try {
    val result : kotlin.Any = apiInstance.testStreamStreamTestGet()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StreamingApi#testStreamStreamTestGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StreamingApi#testStreamStreamTestGet")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.Any**](kotlin.Any.md)

### Authorization


Configure HTTPBearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

