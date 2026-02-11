# Org.OpenAPITools.Api.EpisodesApi

All URIs are relative to *https://believe.cjav.dev*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**CreateEpisodeEpisodesPost**](EpisodesApi.md#createepisodeepisodespost) | **POST** /episodes | Create a new episode |
| [**DeleteEpisodeEpisodesEpisodeIdDelete**](EpisodesApi.md#deleteepisodeepisodesepisodeiddelete) | **DELETE** /episodes/{episode_id} | Delete an episode |
| [**GetEpisodeEpisodesEpisodeIdGet**](EpisodesApi.md#getepisodeepisodesepisodeidget) | **GET** /episodes/{episode_id} | Get an episode by ID |
| [**GetEpisodeWisdomEpisodesEpisodeIdWisdomGet**](EpisodesApi.md#getepisodewisdomepisodesepisodeidwisdomget) | **GET** /episodes/{episode_id}/wisdom | Get episode wisdom |
| [**GetSeasonEpisodesEpisodesSeasonsSeasonNumberGet**](EpisodesApi.md#getseasonepisodesepisodesseasonsseasonnumberget) | **GET** /episodes/seasons/{season_number} | Get all episodes from a season |
| [**ListEpisodesEpisodesGet**](EpisodesApi.md#listepisodesepisodesget) | **GET** /episodes | List all episodes |
| [**UpdateEpisodeEpisodesEpisodeIdPatch**](EpisodesApi.md#updateepisodeepisodesepisodeidpatch) | **PATCH** /episodes/{episode_id} | Update an episode |

<a id="createepisodeepisodespost"></a>
# **CreateEpisodeEpisodesPost**
> Episode CreateEpisodeEpisodesPost (EpisodeCreate episodeCreate)

Create a new episode

Add a new episode to the series.


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **episodeCreate** | [**EpisodeCreate**](EpisodeCreate.md) |  |  |

### Return type

[**Episode**](Episode.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Episode created successfully |  -  |
| **409** | Episode already exists |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="deleteepisodeepisodesepisodeiddelete"></a>
# **DeleteEpisodeEpisodesEpisodeIdDelete**
> void DeleteEpisodeEpisodesEpisodeIdDelete (string episodeId)

Delete an episode

Remove an episode from the database.


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **episodeId** | **string** |  |  |

### Return type

void (empty response body)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | Episode deleted successfully |  -  |
| **404** | Episode not found |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="getepisodeepisodesepisodeidget"></a>
# **GetEpisodeEpisodesEpisodeIdGet**
> Episode GetEpisodeEpisodesEpisodeIdGet (string episodeId)

Get an episode by ID

Retrieve detailed information about a specific episode.


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **episodeId** | **string** |  |  |

### Return type

[**Episode**](Episode.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Episode details |  -  |
| **404** | Episode not found |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="getepisodewisdomepisodesepisodeidwisdomget"></a>
# **GetEpisodeWisdomEpisodesEpisodeIdWisdomGet**
> Dictionary&lt;string, Object&gt; GetEpisodeWisdomEpisodesEpisodeIdWisdomGet (string episodeId)

Get episode wisdom

Get Ted's wisdom and memorable moments from a specific episode.


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **episodeId** | **string** |  |  |

### Return type

**Dictionary<string, Object>**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Episode wisdom details |  -  |
| **404** | Episode not found |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="getseasonepisodesepisodesseasonsseasonnumberget"></a>
# **GetSeasonEpisodesEpisodesSeasonsSeasonNumberGet**
> PaginatedResponseEpisode GetSeasonEpisodesEpisodesSeasonsSeasonNumberGet (int seasonNumber, int skip = null, int limit = null)

Get all episodes from a season

Get a paginated list of episodes from a specific season.


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **seasonNumber** | **int** |  |  |
| **skip** | **int** | Number of items to skip (offset) | [optional] [default to 0] |
| **limit** | **int** | Maximum number of items to return (max: 100) | [optional] [default to 20] |

### Return type

[**PaginatedResponseEpisode**](PaginatedResponseEpisode.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Paginated list of episodes from the season |  -  |
| **404** | Season not found |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="listepisodesepisodesget"></a>
# **ListEpisodesEpisodesGet**
> PaginatedResponseEpisode ListEpisodesEpisodesGet (int season = null, string characterFocus = null, int skip = null, int limit = null)

List all episodes

Get a paginated list of all Ted Lasso episodes with optional filtering by season.


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **season** | **int** | Filter by season | [optional]  |
| **characterFocus** | **string** | Filter by character focus (character ID) | [optional]  |
| **skip** | **int** | Number of items to skip (offset) | [optional] [default to 0] |
| **limit** | **int** | Maximum number of items to return (max: 100) | [optional] [default to 20] |

### Return type

[**PaginatedResponseEpisode**](PaginatedResponseEpisode.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Paginated list of episodes |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="updateepisodeepisodesepisodeidpatch"></a>
# **UpdateEpisodeEpisodesEpisodeIdPatch**
> Episode UpdateEpisodeEpisodesEpisodeIdPatch (string episodeId, EpisodeUpdate episodeUpdate)

Update an episode

Update specific fields of an existing episode.


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **episodeId** | **string** |  |  |
| **episodeUpdate** | [**EpisodeUpdate**](EpisodeUpdate.md) |  |  |

### Return type

[**Episode**](Episode.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Episode updated successfully |  -  |
| **404** | Episode not found |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

