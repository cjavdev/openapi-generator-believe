# EpisodesApi

All URIs are relative to *https://believe.cjav.dev*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createEpisodeEpisodesPost**](EpisodesApi.md#createepisodeepisodespost) | **POST** /episodes | Create a new episode |
| [**deleteEpisodeEpisodesEpisodeIdDelete**](EpisodesApi.md#deleteepisodeepisodesepisodeiddelete) | **DELETE** /episodes/{episode_id} | Delete an episode |
| [**getEpisodeEpisodesEpisodeIdGet**](EpisodesApi.md#getepisodeepisodesepisodeidget) | **GET** /episodes/{episode_id} | Get an episode by ID |
| [**getEpisodeWisdomEpisodesEpisodeIdWisdomGet**](EpisodesApi.md#getepisodewisdomepisodesepisodeidwisdomget) | **GET** /episodes/{episode_id}/wisdom | Get episode wisdom |
| [**getSeasonEpisodesEpisodesSeasonsSeasonNumberGet**](EpisodesApi.md#getseasonepisodesepisodesseasonsseasonnumberget) | **GET** /episodes/seasons/{season_number} | Get all episodes from a season |
| [**listEpisodesEpisodesGet**](EpisodesApi.md#listepisodesepisodesget) | **GET** /episodes | List all episodes |
| [**updateEpisodeEpisodesEpisodeIdPatch**](EpisodesApi.md#updateepisodeepisodesepisodeidpatch) | **PATCH** /episodes/{episode_id} | Update an episode |



## createEpisodeEpisodesPost

> Episode createEpisodeEpisodesPost(episodeCreate)

Create a new episode

Add a new episode to the series.

### Example

```ts
import {
  Configuration,
  EpisodesApi,
} from '';
import type { CreateEpisodeEpisodesPostRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new EpisodesApi(config);

  const body = {
    // EpisodeCreate
    episodeCreate: ...,
  } satisfies CreateEpisodeEpisodesPostRequest;

  try {
    const data = await api.createEpisodeEpisodesPost(body);
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
| **episodeCreate** | [EpisodeCreate](EpisodeCreate.md) |  | |

### Return type

[**Episode**](Episode.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Episode created successfully |  -  |
| **409** | Episode already exists |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deleteEpisodeEpisodesEpisodeIdDelete

> deleteEpisodeEpisodesEpisodeIdDelete(episodeId)

Delete an episode

Remove an episode from the database.

### Example

```ts
import {
  Configuration,
  EpisodesApi,
} from '';
import type { DeleteEpisodeEpisodesEpisodeIdDeleteRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new EpisodesApi(config);

  const body = {
    // string
    episodeId: episodeId_example,
  } satisfies DeleteEpisodeEpisodesEpisodeIdDeleteRequest;

  try {
    const data = await api.deleteEpisodeEpisodesEpisodeIdDelete(body);
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
| **episodeId** | `string` |  | [Defaults to `undefined`] |

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
| **204** | Episode deleted successfully |  -  |
| **404** | Episode not found |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getEpisodeEpisodesEpisodeIdGet

> Episode getEpisodeEpisodesEpisodeIdGet(episodeId)

Get an episode by ID

Retrieve detailed information about a specific episode.

### Example

```ts
import {
  Configuration,
  EpisodesApi,
} from '';
import type { GetEpisodeEpisodesEpisodeIdGetRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new EpisodesApi(config);

  const body = {
    // string
    episodeId: episodeId_example,
  } satisfies GetEpisodeEpisodesEpisodeIdGetRequest;

  try {
    const data = await api.getEpisodeEpisodesEpisodeIdGet(body);
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
| **episodeId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**Episode**](Episode.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Episode details |  -  |
| **404** | Episode not found |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getEpisodeWisdomEpisodesEpisodeIdWisdomGet

> { [key: string]: any; } getEpisodeWisdomEpisodesEpisodeIdWisdomGet(episodeId)

Get episode wisdom

Get Ted\&#39;s wisdom and memorable moments from a specific episode.

### Example

```ts
import {
  Configuration,
  EpisodesApi,
} from '';
import type { GetEpisodeWisdomEpisodesEpisodeIdWisdomGetRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new EpisodesApi(config);

  const body = {
    // string
    episodeId: episodeId_example,
  } satisfies GetEpisodeWisdomEpisodesEpisodeIdWisdomGetRequest;

  try {
    const data = await api.getEpisodeWisdomEpisodesEpisodeIdWisdomGet(body);
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
| **episodeId** | `string` |  | [Defaults to `undefined`] |

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
| **200** | Episode wisdom details |  -  |
| **404** | Episode not found |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getSeasonEpisodesEpisodesSeasonsSeasonNumberGet

> PaginatedResponseEpisode getSeasonEpisodesEpisodesSeasonsSeasonNumberGet(seasonNumber, skip, limit)

Get all episodes from a season

Get a paginated list of episodes from a specific season.

### Example

```ts
import {
  Configuration,
  EpisodesApi,
} from '';
import type { GetSeasonEpisodesEpisodesSeasonsSeasonNumberGetRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new EpisodesApi(config);

  const body = {
    // number
    seasonNumber: 56,
    // number | Number of items to skip (offset) (optional)
    skip: 56,
    // number | Maximum number of items to return (max: 100) (optional)
    limit: 56,
  } satisfies GetSeasonEpisodesEpisodesSeasonsSeasonNumberGetRequest;

  try {
    const data = await api.getSeasonEpisodesEpisodesSeasonsSeasonNumberGet(body);
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
| **seasonNumber** | `number` |  | [Defaults to `undefined`] |
| **skip** | `number` | Number of items to skip (offset) | [Optional] [Defaults to `0`] |
| **limit** | `number` | Maximum number of items to return (max: 100) | [Optional] [Defaults to `20`] |

### Return type

[**PaginatedResponseEpisode**](PaginatedResponseEpisode.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Paginated list of episodes from the season |  -  |
| **404** | Season not found |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## listEpisodesEpisodesGet

> PaginatedResponseEpisode listEpisodesEpisodesGet(season, characterFocus, skip, limit)

List all episodes

Get a paginated list of all Ted Lasso episodes with optional filtering by season.

### Example

```ts
import {
  Configuration,
  EpisodesApi,
} from '';
import type { ListEpisodesEpisodesGetRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new EpisodesApi(config);

  const body = {
    // number | Filter by season (optional)
    season: 56,
    // string | Filter by character focus (character ID) (optional)
    characterFocus: characterFocus_example,
    // number | Number of items to skip (offset) (optional)
    skip: 56,
    // number | Maximum number of items to return (max: 100) (optional)
    limit: 56,
  } satisfies ListEpisodesEpisodesGetRequest;

  try {
    const data = await api.listEpisodesEpisodesGet(body);
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
| **season** | `number` | Filter by season | [Optional] [Defaults to `undefined`] |
| **characterFocus** | `string` | Filter by character focus (character ID) | [Optional] [Defaults to `undefined`] |
| **skip** | `number` | Number of items to skip (offset) | [Optional] [Defaults to `0`] |
| **limit** | `number` | Maximum number of items to return (max: 100) | [Optional] [Defaults to `20`] |

### Return type

[**PaginatedResponseEpisode**](PaginatedResponseEpisode.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Paginated list of episodes |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## updateEpisodeEpisodesEpisodeIdPatch

> Episode updateEpisodeEpisodesEpisodeIdPatch(episodeId, episodeUpdate)

Update an episode

Update specific fields of an existing episode.

### Example

```ts
import {
  Configuration,
  EpisodesApi,
} from '';
import type { UpdateEpisodeEpisodesEpisodeIdPatchRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new EpisodesApi(config);

  const body = {
    // string
    episodeId: episodeId_example,
    // EpisodeUpdate
    episodeUpdate: ...,
  } satisfies UpdateEpisodeEpisodesEpisodeIdPatchRequest;

  try {
    const data = await api.updateEpisodeEpisodesEpisodeIdPatch(body);
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
| **episodeId** | `string` |  | [Defaults to `undefined`] |
| **episodeUpdate** | [EpisodeUpdate](EpisodeUpdate.md) |  | |

### Return type

[**Episode**](Episode.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Episode updated successfully |  -  |
| **404** | Episode not found |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

