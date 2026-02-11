# Org.OpenAPITools.Api.TeamsApi

All URIs are relative to *https://believe.cjav.dev*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**CreateTeamTeamsPost**](TeamsApi.md#createteamteamspost) | **POST** /teams | Create a new team |
| [**DeleteTeamLogoTeamsTeamIdLogoFileIdDelete**](TeamsApi.md#deleteteamlogoteamsteamidlogofileiddelete) | **DELETE** /teams/{team_id}/logo/{file_id} | Delete team logo |
| [**DeleteTeamTeamsTeamIdDelete**](TeamsApi.md#deleteteamteamsteamiddelete) | **DELETE** /teams/{team_id} | Delete a team |
| [**DownloadTeamLogoTeamsTeamIdLogoFileIdGet**](TeamsApi.md#downloadteamlogoteamsteamidlogofileidget) | **GET** /teams/{team_id}/logo/{file_id} | Download team logo |
| [**GetTeamCultureTeamsTeamIdCultureGet**](TeamsApi.md#getteamcultureteamsteamidcultureget) | **GET** /teams/{team_id}/culture | Get team culture details |
| [**GetTeamRivalsTeamsTeamIdRivalsGet**](TeamsApi.md#getteamrivalsteamsteamidrivalsget) | **GET** /teams/{team_id}/rivals | Get team&#39;s rivals |
| [**GetTeamTeamsTeamIdGet**](TeamsApi.md#getteamteamsteamidget) | **GET** /teams/{team_id} | Get a team by ID |
| [**ListTeamLogosTeamsTeamIdLogosGet**](TeamsApi.md#listteamlogosteamsteamidlogosget) | **GET** /teams/{team_id}/logos | List team logos |
| [**ListTeamsTeamsGet**](TeamsApi.md#listteamsteamsget) | **GET** /teams | List all teams |
| [**UpdateTeamTeamsTeamIdPatch**](TeamsApi.md#updateteamteamsteamidpatch) | **PATCH** /teams/{team_id} | Update a team |
| [**UploadTeamLogoTeamsTeamIdLogoPost**](TeamsApi.md#uploadteamlogoteamsteamidlogopost) | **POST** /teams/{team_id}/logo | Upload team logo |

<a id="createteamteamspost"></a>
# **CreateTeamTeamsPost**
> Team CreateTeamTeamsPost (TeamCreate teamCreate)

Create a new team

Add a new team to the league.


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **teamCreate** | [**TeamCreate**](TeamCreate.md) |  |  |

### Return type

[**Team**](Team.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Team created successfully |  -  |
| **409** | Team already exists |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="deleteteamlogoteamsteamidlogofileiddelete"></a>
# **DeleteTeamLogoTeamsTeamIdLogoFileIdDelete**
> void DeleteTeamLogoTeamsTeamIdLogoFileIdDelete (string teamId, Guid fileId)

Delete team logo

Delete a team's logo.


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **teamId** | **string** |  |  |
| **fileId** | **Guid** |  |  |

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
| **204** | Logo deleted |  -  |
| **404** | Team or file not found |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="deleteteamteamsteamiddelete"></a>
# **DeleteTeamTeamsTeamIdDelete**
> void DeleteTeamTeamsTeamIdDelete (string teamId)

Delete a team

Remove a team from the database (relegation to oblivion).


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **teamId** | **string** |  |  |

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
| **204** | Team deleted successfully |  -  |
| **404** | Team not found |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="downloadteamlogoteamsteamidlogofileidget"></a>
# **DownloadTeamLogoTeamsTeamIdLogoFileIdGet**
> Object DownloadTeamLogoTeamsTeamIdLogoFileIdGet (string teamId, Guid fileId)

Download team logo

Download a team's logo by file ID.


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **teamId** | **string** |  |  |
| **fileId** | **Guid** |  |  |

### Return type

**Object**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, image/*


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Logo file content |  -  |
| **404** | Team or file not found |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="getteamcultureteamsteamidcultureget"></a>
# **GetTeamCultureTeamsTeamIdCultureGet**
> Dictionary&lt;string, Object&gt; GetTeamCultureTeamsTeamIdCultureGet (string teamId)

Get team culture details

Get detailed culture and values information for a team.


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **teamId** | **string** |  |  |

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
| **200** | Team culture details |  -  |
| **404** | Team not found |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="getteamrivalsteamsteamidrivalsget"></a>
# **GetTeamRivalsTeamsTeamIdRivalsGet**
> List&lt;Team&gt; GetTeamRivalsTeamsTeamIdRivalsGet (string teamId)

Get team's rivals

Get all rival teams for a specific team.


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **teamId** | **string** |  |  |

### Return type

[**List&lt;Team&gt;**](Team.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | List of rival teams |  -  |
| **404** | Team not found |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="getteamteamsteamidget"></a>
# **GetTeamTeamsTeamIdGet**
> Team GetTeamTeamsTeamIdGet (string teamId)

Get a team by ID

Retrieve detailed information about a specific team.


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **teamId** | **string** |  |  |

### Return type

[**Team**](Team.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Team details |  -  |
| **404** | Team not found |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="listteamlogosteamsteamidlogosget"></a>
# **ListTeamLogosTeamsTeamIdLogosGet**
> List&lt;FileUploadResponse&gt; ListTeamLogosTeamsTeamIdLogosGet (string teamId)

List team logos

List all uploaded logos for a team.


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **teamId** | **string** |  |  |

### Return type

[**List&lt;FileUploadResponse&gt;**](FileUploadResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Successful Response |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="listteamsteamsget"></a>
# **ListTeamsTeamsGet**
> PaginatedResponseTeam ListTeamsTeamsGet (League league = null, int minCultureScore = null, int skip = null, int limit = null)

List all teams

Get a paginated list of all teams with optional filtering by league or culture score.


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **league** | **League** | Filter by league | [optional]  |
| **minCultureScore** | **int** | Minimum culture score | [optional]  |
| **skip** | **int** | Number of items to skip (offset) | [optional] [default to 0] |
| **limit** | **int** | Maximum number of items to return (max: 100) | [optional] [default to 20] |

### Return type

[**PaginatedResponseTeam**](PaginatedResponseTeam.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Paginated list of teams |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="updateteamteamsteamidpatch"></a>
# **UpdateTeamTeamsTeamIdPatch**
> Team UpdateTeamTeamsTeamIdPatch (string teamId, TeamUpdate teamUpdate)

Update a team

Update specific fields of an existing team.


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **teamId** | **string** |  |  |
| **teamUpdate** | [**TeamUpdate**](TeamUpdate.md) |  |  |

### Return type

[**Team**](Team.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Team updated successfully |  -  |
| **404** | Team not found |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="uploadteamlogoteamsteamidlogopost"></a>
# **UploadTeamLogoTeamsTeamIdLogoPost**
> FileUploadResponse UploadTeamLogoTeamsTeamIdLogoPost (string teamId, System.IO.Stream file)

Upload team logo

Upload a logo image for a team. Accepts image files (jpg, png, gif, webp).


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **teamId** | **string** |  |  |
| **file** | **System.IO.Stream****System.IO.Stream** | Logo image file |  |

### Return type

[**FileUploadResponse**](FileUploadResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Logo uploaded successfully |  -  |
| **404** | Team not found |  -  |
| **415** | Unsupported file type |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

