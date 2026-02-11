# MatchesApi

All URIs are relative to *https://believe.cjav.dev*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createMatchMatchesPost**](MatchesApi.md#creatematchmatchespost) | **POST** /matches | Create a new match |
| [**deleteMatchMatchesMatchIdDelete**](MatchesApi.md#deletematchmatchesmatchiddelete) | **DELETE** /matches/{match_id} | Delete a match |
| [**getMatchLessonMatchesMatchIdLessonGet**](MatchesApi.md#getmatchlessonmatchesmatchidlessonget) | **GET** /matches/{match_id}/lesson | Get match lesson |
| [**getMatchMatchesMatchIdGet**](MatchesApi.md#getmatchmatchesmatchidget) | **GET** /matches/{match_id} | Get a match by ID |
| [**getTurningPointsMatchesMatchIdTurningPointsGet**](MatchesApi.md#getturningpointsmatchesmatchidturningpointsget) | **GET** /matches/{match_id}/turning-points | Get match turning points |
| [**listMatchesMatchesGet**](MatchesApi.md#listmatchesmatchesget) | **GET** /matches | List all matches |
| [**updateMatchMatchesMatchIdPatch**](MatchesApi.md#updatematchmatchesmatchidpatch) | **PATCH** /matches/{match_id} | Update a match |



## createMatchMatchesPost

> Match createMatchMatchesPost(matchCreate)

Create a new match

Schedule a new match.

### Example

```ts
import {
  Configuration,
  MatchesApi,
} from '';
import type { CreateMatchMatchesPostRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new MatchesApi(config);

  const body = {
    // MatchCreate
    matchCreate: ...,
  } satisfies CreateMatchMatchesPostRequest;

  try {
    const data = await api.createMatchMatchesPost(body);
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
| **matchCreate** | [MatchCreate](MatchCreate.md) |  | |

### Return type

[**Match**](Match.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Match created successfully |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deleteMatchMatchesMatchIdDelete

> deleteMatchMatchesMatchIdDelete(matchId)

Delete a match

Remove a match from the database.

### Example

```ts
import {
  Configuration,
  MatchesApi,
} from '';
import type { DeleteMatchMatchesMatchIdDeleteRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new MatchesApi(config);

  const body = {
    // string
    matchId: matchId_example,
  } satisfies DeleteMatchMatchesMatchIdDeleteRequest;

  try {
    const data = await api.deleteMatchMatchesMatchIdDelete(body);
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

`void` (Empty response body)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | Match deleted successfully |  -  |
| **404** | Match not found |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getMatchLessonMatchesMatchIdLessonGet

> { [key: string]: any; } getMatchLessonMatchesMatchIdLessonGet(matchId)

Get match lesson

Get the life lesson learned from a specific match.

### Example

```ts
import {
  Configuration,
  MatchesApi,
} from '';
import type { GetMatchLessonMatchesMatchIdLessonGetRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new MatchesApi(config);

  const body = {
    // string
    matchId: matchId_example,
  } satisfies GetMatchLessonMatchesMatchIdLessonGetRequest;

  try {
    const data = await api.getMatchLessonMatchesMatchIdLessonGet(body);
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

**{ [key: string]: any; }**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Match lesson details |  -  |
| **404** | Match not found |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getMatchMatchesMatchIdGet

> Match getMatchMatchesMatchIdGet(matchId)

Get a match by ID

Retrieve detailed information about a specific match.

### Example

```ts
import {
  Configuration,
  MatchesApi,
} from '';
import type { GetMatchMatchesMatchIdGetRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new MatchesApi(config);

  const body = {
    // string
    matchId: matchId_example,
  } satisfies GetMatchMatchesMatchIdGetRequest;

  try {
    const data = await api.getMatchMatchesMatchIdGet(body);
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

[**Match**](Match.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Match details |  -  |
| **404** | Match not found |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getTurningPointsMatchesMatchIdTurningPointsGet

> Array&lt;{ [key: string]: any; }&gt; getTurningPointsMatchesMatchIdTurningPointsGet(matchId)

Get match turning points

Get all turning points from a specific match.

### Example

```ts
import {
  Configuration,
  MatchesApi,
} from '';
import type { GetTurningPointsMatchesMatchIdTurningPointsGetRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new MatchesApi(config);

  const body = {
    // string
    matchId: matchId_example,
  } satisfies GetTurningPointsMatchesMatchIdTurningPointsGetRequest;

  try {
    const data = await api.getTurningPointsMatchesMatchIdTurningPointsGet(body);
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

**Array<{ [key: string]: any; }>**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of turning points |  -  |
| **404** | Match not found |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## listMatchesMatchesGet

> PaginatedResponseMatch listMatchesMatchesGet(teamId, result, matchType, skip, limit)

List all matches

Get a paginated list of all matches with optional filtering.

### Example

```ts
import {
  Configuration,
  MatchesApi,
} from '';
import type { ListMatchesMatchesGetRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new MatchesApi(config);

  const body = {
    // string | Filter by team (home or away) (optional)
    teamId: teamId_example,
    // MatchResult | Filter by result (optional)
    result: ...,
    // MatchType | Filter by match type (optional)
    matchType: ...,
    // number | Number of items to skip (offset) (optional)
    skip: 56,
    // number | Maximum number of items to return (max: 100) (optional)
    limit: 56,
  } satisfies ListMatchesMatchesGetRequest;

  try {
    const data = await api.listMatchesMatchesGet(body);
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
| **teamId** | `string` | Filter by team (home or away) | [Optional] [Defaults to `undefined`] |
| **result** | `MatchResult` | Filter by result | [Optional] [Defaults to `undefined`] [Enum: win, loss, draw, pending] |
| **matchType** | `MatchType` | Filter by match type | [Optional] [Defaults to `undefined`] [Enum: league, cup, friendly, playoff, final] |
| **skip** | `number` | Number of items to skip (offset) | [Optional] [Defaults to `0`] |
| **limit** | `number` | Maximum number of items to return (max: 100) | [Optional] [Defaults to `20`] |

### Return type

[**PaginatedResponseMatch**](PaginatedResponseMatch.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Paginated list of matches |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## updateMatchMatchesMatchIdPatch

> Match updateMatchMatchesMatchIdPatch(matchId, matchUpdate)

Update a match

Update specific fields of an existing match (e.g., update score).

### Example

```ts
import {
  Configuration,
  MatchesApi,
} from '';
import type { UpdateMatchMatchesMatchIdPatchRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new MatchesApi(config);

  const body = {
    // string
    matchId: matchId_example,
    // MatchUpdate
    matchUpdate: ...,
  } satisfies UpdateMatchMatchesMatchIdPatchRequest;

  try {
    const data = await api.updateMatchMatchesMatchIdPatch(body);
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
| **matchUpdate** | [MatchUpdate](MatchUpdate.md) |  | |

### Return type

[**Match**](Match.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Match updated successfully |  -  |
| **404** | Match not found |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

