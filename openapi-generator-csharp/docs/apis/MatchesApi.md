# Org.OpenAPITools.Api.MatchesApi

All URIs are relative to *https://believe.cjav.dev*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**CreateMatchMatchesPost**](MatchesApi.md#creatematchmatchespost) | **POST** /matches | Create a new match |
| [**DeleteMatchMatchesMatchIdDelete**](MatchesApi.md#deletematchmatchesmatchiddelete) | **DELETE** /matches/{match_id} | Delete a match |
| [**GetMatchLessonMatchesMatchIdLessonGet**](MatchesApi.md#getmatchlessonmatchesmatchidlessonget) | **GET** /matches/{match_id}/lesson | Get match lesson |
| [**GetMatchMatchesMatchIdGet**](MatchesApi.md#getmatchmatchesmatchidget) | **GET** /matches/{match_id} | Get a match by ID |
| [**GetTurningPointsMatchesMatchIdTurningPointsGet**](MatchesApi.md#getturningpointsmatchesmatchidturningpointsget) | **GET** /matches/{match_id}/turning-points | Get match turning points |
| [**ListMatchesMatchesGet**](MatchesApi.md#listmatchesmatchesget) | **GET** /matches | List all matches |
| [**UpdateMatchMatchesMatchIdPatch**](MatchesApi.md#updatematchmatchesmatchidpatch) | **PATCH** /matches/{match_id} | Update a match |

<a id="creatematchmatchespost"></a>
# **CreateMatchMatchesPost**
> Match CreateMatchMatchesPost (MatchCreate matchCreate)

Create a new match

Schedule a new match.


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **matchCreate** | [**MatchCreate**](MatchCreate.md) |  |  |

### Return type

[**Match**](Match.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Match created successfully |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="deletematchmatchesmatchiddelete"></a>
# **DeleteMatchMatchesMatchIdDelete**
> void DeleteMatchMatchesMatchIdDelete (string matchId)

Delete a match

Remove a match from the database.


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **matchId** | **string** |  |  |

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
| **204** | Match deleted successfully |  -  |
| **404** | Match not found |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="getmatchlessonmatchesmatchidlessonget"></a>
# **GetMatchLessonMatchesMatchIdLessonGet**
> Dictionary&lt;string, Object&gt; GetMatchLessonMatchesMatchIdLessonGet (string matchId)

Get match lesson

Get the life lesson learned from a specific match.


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **matchId** | **string** |  |  |

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
| **200** | Match lesson details |  -  |
| **404** | Match not found |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="getmatchmatchesmatchidget"></a>
# **GetMatchMatchesMatchIdGet**
> Match GetMatchMatchesMatchIdGet (string matchId)

Get a match by ID

Retrieve detailed information about a specific match.


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **matchId** | **string** |  |  |

### Return type

[**Match**](Match.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Match details |  -  |
| **404** | Match not found |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="getturningpointsmatchesmatchidturningpointsget"></a>
# **GetTurningPointsMatchesMatchIdTurningPointsGet**
> List&lt;Dictionary&lt;string, Object&gt;&gt; GetTurningPointsMatchesMatchIdTurningPointsGet (string matchId)

Get match turning points

Get all turning points from a specific match.


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **matchId** | **string** |  |  |

### Return type

**List<Dictionary<string, Object>>**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of turning points |  -  |
| **404** | Match not found |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="listmatchesmatchesget"></a>
# **ListMatchesMatchesGet**
> PaginatedResponseMatch ListMatchesMatchesGet (string teamId = null, MatchResult result = null, MatchType matchType = null, int skip = null, int limit = null)

List all matches

Get a paginated list of all matches with optional filtering.


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **teamId** | **string** | Filter by team (home or away) | [optional]  |
| **result** | **MatchResult** | Filter by result | [optional]  |
| **matchType** | **MatchType** | Filter by match type | [optional]  |
| **skip** | **int** | Number of items to skip (offset) | [optional] [default to 0] |
| **limit** | **int** | Maximum number of items to return (max: 100) | [optional] [default to 20] |

### Return type

[**PaginatedResponseMatch**](PaginatedResponseMatch.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Paginated list of matches |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="updatematchmatchesmatchidpatch"></a>
# **UpdateMatchMatchesMatchIdPatch**
> Match UpdateMatchMatchesMatchIdPatch (string matchId, MatchUpdate matchUpdate)

Update a match

Update specific fields of an existing match (e.g., update score).


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **matchId** | **string** |  |  |
| **matchUpdate** | [**MatchUpdate**](MatchUpdate.md) |  |  |

### Return type

[**Match**](Match.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Match updated successfully |  -  |
| **404** | Match not found |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

