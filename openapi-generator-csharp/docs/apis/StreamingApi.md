# Org.OpenAPITools.Api.StreamingApi

All URIs are relative to *https://believe.cjav.dev*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**GetPepTalkPepTalkGet**](StreamingApi.md#getpeptalkpeptalkget) | **GET** /pep-talk | Get a Pep Talk |
| [**StreamMatchCommentaryMatchesMatchIdCommentaryStreamPost**](StreamingApi.md#streammatchcommentarymatchesmatchidcommentarystreampost) | **POST** /matches/{match_id}/commentary/stream | Stream Match Commentary |
| [**TestStreamStreamTestGet**](StreamingApi.md#teststreamstreamtestget) | **GET** /stream/test | Test SSE Connection |

<a id="getpeptalkpeptalkget"></a>
# **GetPepTalkPepTalkGet**
> PepTalkResponse GetPepTalkPepTalkGet (bool stream = null)

Get a Pep Talk

Get a motivational pep talk from Ted Lasso himself. By default returns the complete pep talk. Add `?stream=true` to get Server-Sent Events (SSE) streaming the pep talk chunk by chunk.


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **stream** | **bool** | If true, returns SSE stream instead of full response | [optional] [default to false] |

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

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="streammatchcommentarymatchesmatchidcommentarystreampost"></a>
# **StreamMatchCommentaryMatchesMatchIdCommentaryStreamPost**
> Object StreamMatchCommentaryMatchesMatchIdCommentaryStreamPost (string matchId)

Stream Match Commentary

Stream live match commentary for a specific match. Uses Server-Sent Events (SSE) to stream commentary events in real-time.


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **matchId** | **string** |  |  |

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

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="teststreamstreamtestget"></a>
# **TestStreamStreamTestGet**
> Object TestStreamStreamTestGet ()

Test SSE Connection

A simple SSE test endpoint that streams numbers 1-5.


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

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

