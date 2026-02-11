# StreamingApi

All URIs are relative to *https://believe.cjav.dev*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**getPepTalkPepTalkGet**](StreamingApi.md#getpeptalkpeptalkget) | **GET** /pep-talk | Get a Pep Talk |
| [**streamMatchCommentaryMatchesMatchIdCommentaryStreamPost**](StreamingApi.md#streammatchcommentarymatchesmatchidcommentarystreampost) | **POST** /matches/{match_id}/commentary/stream | Stream Match Commentary |
| [**testStreamStreamTestGet**](StreamingApi.md#teststreamstreamtestget) | **GET** /stream/test | Test SSE Connection |



## getPepTalkPepTalkGet

> PepTalkResponse getPepTalkPepTalkGet(stream)

Get a Pep Talk

Get a motivational pep talk from Ted Lasso himself. By default returns the complete pep talk. Add &#x60;?stream&#x3D;true&#x60; to get Server-Sent Events (SSE) streaming the pep talk chunk by chunk.

### Example

```ts
import {
  Configuration,
  StreamingApi,
} from '';
import type { GetPepTalkPepTalkGetRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new StreamingApi(config);

  const body = {
    // boolean | If true, returns SSE stream instead of full response (optional)
    stream: true,
  } satisfies GetPepTalkPepTalkGetRequest;

  try {
    const data = await api.getPepTalkPepTalkGet(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **stream** | `boolean` | If true, returns SSE stream instead of full response | [Optional] [Defaults to `false`] |

### Return type

[**PepTalkResponse**](PepTalkResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `text/event-stream`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Pep talk response (JSON or SSE stream) |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## streamMatchCommentaryMatchesMatchIdCommentaryStreamPost

> any streamMatchCommentaryMatchesMatchIdCommentaryStreamPost(matchId)

Stream Match Commentary

Stream live match commentary for a specific match. Uses Server-Sent Events (SSE) to stream commentary events in real-time.

### Example

```ts
import {
  Configuration,
  StreamingApi,
} from '';
import type { StreamMatchCommentaryMatchesMatchIdCommentaryStreamPostRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new StreamingApi(config);

  const body = {
    // string
    matchId: matchId_example,
  } satisfies StreamMatchCommentaryMatchesMatchIdCommentaryStreamPostRequest;

  try {
    const data = await api.streamMatchCommentaryMatchesMatchIdCommentaryStreamPost(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **matchId** | `string` |  | [Defaults to `undefined`] |

### Return type

**any**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `text/event-stream`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | SSE stream of match commentary events |  -  |
| **404** | Match not found |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## testStreamStreamTestGet

> any testStreamStreamTestGet()

Test SSE Connection

A simple SSE test endpoint that streams numbers 1-5.

### Example

```ts
import {
  Configuration,
  StreamingApi,
} from '';
import type { TestStreamStreamTestGetRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new StreamingApi(config);

  try {
    const data = await api.testStreamStreamTestGet();
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters

This endpoint does not need any parameter.

### Return type

**any**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `text/event-stream`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | SSE stream of test messages |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

