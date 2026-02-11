# TeamsApi

All URIs are relative to *https://believe.cjav.dev*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createTeamTeamsPost**](TeamsApi.md#createteamteamspost) | **POST** /teams | Create a new team |
| [**deleteTeamLogoTeamsTeamIdLogoFileIdDelete**](TeamsApi.md#deleteteamlogoteamsteamidlogofileiddelete) | **DELETE** /teams/{team_id}/logo/{file_id} | Delete team logo |
| [**deleteTeamTeamsTeamIdDelete**](TeamsApi.md#deleteteamteamsteamiddelete) | **DELETE** /teams/{team_id} | Delete a team |
| [**downloadTeamLogoTeamsTeamIdLogoFileIdGet**](TeamsApi.md#downloadteamlogoteamsteamidlogofileidget) | **GET** /teams/{team_id}/logo/{file_id} | Download team logo |
| [**getTeamCultureTeamsTeamIdCultureGet**](TeamsApi.md#getteamcultureteamsteamidcultureget) | **GET** /teams/{team_id}/culture | Get team culture details |
| [**getTeamRivalsTeamsTeamIdRivalsGet**](TeamsApi.md#getteamrivalsteamsteamidrivalsget) | **GET** /teams/{team_id}/rivals | Get team\&#39;s rivals |
| [**getTeamTeamsTeamIdGet**](TeamsApi.md#getteamteamsteamidget) | **GET** /teams/{team_id} | Get a team by ID |
| [**listTeamLogosTeamsTeamIdLogosGet**](TeamsApi.md#listteamlogosteamsteamidlogosget) | **GET** /teams/{team_id}/logos | List team logos |
| [**listTeamsTeamsGet**](TeamsApi.md#listteamsteamsget) | **GET** /teams | List all teams |
| [**updateTeamTeamsTeamIdPatch**](TeamsApi.md#updateteamteamsteamidpatch) | **PATCH** /teams/{team_id} | Update a team |
| [**uploadTeamLogoTeamsTeamIdLogoPost**](TeamsApi.md#uploadteamlogoteamsteamidlogopost) | **POST** /teams/{team_id}/logo | Upload team logo |



## createTeamTeamsPost

> Team createTeamTeamsPost(teamCreate)

Create a new team

Add a new team to the league.

### Example

```ts
import {
  Configuration,
  TeamsApi,
} from '';
import type { CreateTeamTeamsPostRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new TeamsApi(config);

  const body = {
    // TeamCreate
    teamCreate: ...,
  } satisfies CreateTeamTeamsPostRequest;

  try {
    const data = await api.createTeamTeamsPost(body);
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
| **teamCreate** | [TeamCreate](TeamCreate.md) |  | |

### Return type

[**Team**](Team.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Team created successfully |  -  |
| **409** | Team already exists |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deleteTeamLogoTeamsTeamIdLogoFileIdDelete

> deleteTeamLogoTeamsTeamIdLogoFileIdDelete(teamId, fileId)

Delete team logo

Delete a team\&#39;s logo.

### Example

```ts
import {
  Configuration,
  TeamsApi,
} from '';
import type { DeleteTeamLogoTeamsTeamIdLogoFileIdDeleteRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new TeamsApi(config);

  const body = {
    // string
    teamId: teamId_example,
    // string
    fileId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
  } satisfies DeleteTeamLogoTeamsTeamIdLogoFileIdDeleteRequest;

  try {
    const data = await api.deleteTeamLogoTeamsTeamIdLogoFileIdDelete(body);
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
| **teamId** | `string` |  | [Defaults to `undefined`] |
| **fileId** | `string` |  | [Defaults to `undefined`] |

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
| **204** | Logo deleted |  -  |
| **404** | Team or file not found |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deleteTeamTeamsTeamIdDelete

> deleteTeamTeamsTeamIdDelete(teamId)

Delete a team

Remove a team from the database (relegation to oblivion).

### Example

```ts
import {
  Configuration,
  TeamsApi,
} from '';
import type { DeleteTeamTeamsTeamIdDeleteRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new TeamsApi(config);

  const body = {
    // string
    teamId: teamId_example,
  } satisfies DeleteTeamTeamsTeamIdDeleteRequest;

  try {
    const data = await api.deleteTeamTeamsTeamIdDelete(body);
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
| **teamId** | `string` |  | [Defaults to `undefined`] |

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
| **204** | Team deleted successfully |  -  |
| **404** | Team not found |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## downloadTeamLogoTeamsTeamIdLogoFileIdGet

> any downloadTeamLogoTeamsTeamIdLogoFileIdGet(teamId, fileId)

Download team logo

Download a team\&#39;s logo by file ID.

### Example

```ts
import {
  Configuration,
  TeamsApi,
} from '';
import type { DownloadTeamLogoTeamsTeamIdLogoFileIdGetRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new TeamsApi(config);

  const body = {
    // string
    teamId: teamId_example,
    // string
    fileId: 38400000-8cf0-11bd-b23e-10b96e4ef00d,
  } satisfies DownloadTeamLogoTeamsTeamIdLogoFileIdGetRequest;

  try {
    const data = await api.downloadTeamLogoTeamsTeamIdLogoFileIdGet(body);
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
| **teamId** | `string` |  | [Defaults to `undefined`] |
| **fileId** | `string` |  | [Defaults to `undefined`] |

### Return type

**any**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `image/*`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Logo file content |  -  |
| **404** | Team or file not found |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getTeamCultureTeamsTeamIdCultureGet

> { [key: string]: any; } getTeamCultureTeamsTeamIdCultureGet(teamId)

Get team culture details

Get detailed culture and values information for a team.

### Example

```ts
import {
  Configuration,
  TeamsApi,
} from '';
import type { GetTeamCultureTeamsTeamIdCultureGetRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new TeamsApi(config);

  const body = {
    // string
    teamId: teamId_example,
  } satisfies GetTeamCultureTeamsTeamIdCultureGetRequest;

  try {
    const data = await api.getTeamCultureTeamsTeamIdCultureGet(body);
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
| **teamId** | `string` |  | [Defaults to `undefined`] |

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
| **200** | Team culture details |  -  |
| **404** | Team not found |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getTeamRivalsTeamsTeamIdRivalsGet

> Array&lt;Team&gt; getTeamRivalsTeamsTeamIdRivalsGet(teamId)

Get team\&#39;s rivals

Get all rival teams for a specific team.

### Example

```ts
import {
  Configuration,
  TeamsApi,
} from '';
import type { GetTeamRivalsTeamsTeamIdRivalsGetRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new TeamsApi(config);

  const body = {
    // string
    teamId: teamId_example,
  } satisfies GetTeamRivalsTeamsTeamIdRivalsGetRequest;

  try {
    const data = await api.getTeamRivalsTeamsTeamIdRivalsGet(body);
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
| **teamId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**Array&lt;Team&gt;**](Team.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of rival teams |  -  |
| **404** | Team not found |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getTeamTeamsTeamIdGet

> Team getTeamTeamsTeamIdGet(teamId)

Get a team by ID

Retrieve detailed information about a specific team.

### Example

```ts
import {
  Configuration,
  TeamsApi,
} from '';
import type { GetTeamTeamsTeamIdGetRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new TeamsApi(config);

  const body = {
    // string
    teamId: teamId_example,
  } satisfies GetTeamTeamsTeamIdGetRequest;

  try {
    const data = await api.getTeamTeamsTeamIdGet(body);
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
| **teamId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**Team**](Team.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Team details |  -  |
| **404** | Team not found |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## listTeamLogosTeamsTeamIdLogosGet

> Array&lt;FileUploadResponse&gt; listTeamLogosTeamsTeamIdLogosGet(teamId)

List team logos

List all uploaded logos for a team.

### Example

```ts
import {
  Configuration,
  TeamsApi,
} from '';
import type { ListTeamLogosTeamsTeamIdLogosGetRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new TeamsApi(config);

  const body = {
    // string
    teamId: teamId_example,
  } satisfies ListTeamLogosTeamsTeamIdLogosGetRequest;

  try {
    const data = await api.listTeamLogosTeamsTeamIdLogosGet(body);
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
| **teamId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**Array&lt;FileUploadResponse&gt;**](FileUploadResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Successful Response |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## listTeamsTeamsGet

> PaginatedResponseTeam listTeamsTeamsGet(league, minCultureScore, skip, limit)

List all teams

Get a paginated list of all teams with optional filtering by league or culture score.

### Example

```ts
import {
  Configuration,
  TeamsApi,
} from '';
import type { ListTeamsTeamsGetRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new TeamsApi(config);

  const body = {
    // League | Filter by league (optional)
    league: ...,
    // number | Minimum culture score (optional)
    minCultureScore: 56,
    // number | Number of items to skip (offset) (optional)
    skip: 56,
    // number | Maximum number of items to return (max: 100) (optional)
    limit: 56,
  } satisfies ListTeamsTeamsGetRequest;

  try {
    const data = await api.listTeamsTeamsGet(body);
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
| **league** | `League` | Filter by league | [Optional] [Defaults to `undefined`] [Enum: Premier League, Championship, League One, League Two, La Liga, Serie A, Bundesliga, Ligue 1] |
| **minCultureScore** | `number` | Minimum culture score | [Optional] [Defaults to `undefined`] |
| **skip** | `number` | Number of items to skip (offset) | [Optional] [Defaults to `0`] |
| **limit** | `number` | Maximum number of items to return (max: 100) | [Optional] [Defaults to `20`] |

### Return type

[**PaginatedResponseTeam**](PaginatedResponseTeam.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Paginated list of teams |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## updateTeamTeamsTeamIdPatch

> Team updateTeamTeamsTeamIdPatch(teamId, teamUpdate)

Update a team

Update specific fields of an existing team.

### Example

```ts
import {
  Configuration,
  TeamsApi,
} from '';
import type { UpdateTeamTeamsTeamIdPatchRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new TeamsApi(config);

  const body = {
    // string
    teamId: teamId_example,
    // TeamUpdate
    teamUpdate: ...,
  } satisfies UpdateTeamTeamsTeamIdPatchRequest;

  try {
    const data = await api.updateTeamTeamsTeamIdPatch(body);
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
| **teamId** | `string` |  | [Defaults to `undefined`] |
| **teamUpdate** | [TeamUpdate](TeamUpdate.md) |  | |

### Return type

[**Team**](Team.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Team updated successfully |  -  |
| **404** | Team not found |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## uploadTeamLogoTeamsTeamIdLogoPost

> FileUploadResponse uploadTeamLogoTeamsTeamIdLogoPost(teamId, file)

Upload team logo

Upload a logo image for a team. Accepts image files (jpg, png, gif, webp).

### Example

```ts
import {
  Configuration,
  TeamsApi,
} from '';
import type { UploadTeamLogoTeamsTeamIdLogoPostRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new TeamsApi(config);

  const body = {
    // string
    teamId: teamId_example,
    // Blob | Logo image file
    file: BINARY_DATA_HERE,
  } satisfies UploadTeamLogoTeamsTeamIdLogoPostRequest;

  try {
    const data = await api.uploadTeamLogoTeamsTeamIdLogoPost(body);
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
| **teamId** | `string` |  | [Defaults to `undefined`] |
| **file** | `Blob` | Logo image file | [Defaults to `undefined`] |

### Return type

[**FileUploadResponse**](FileUploadResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: `multipart/form-data`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Logo uploaded successfully |  -  |
| **404** | Team not found |  -  |
| **415** | Unsupported file type |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

