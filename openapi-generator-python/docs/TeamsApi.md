# openapi_client.TeamsApi

All URIs are relative to *https://believe.cjav.dev*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_team_teams_post**](TeamsApi.md#create_team_teams_post) | **POST** /teams | Create a new team
[**delete_team_logo_teams_team_id_logo_file_id_delete**](TeamsApi.md#delete_team_logo_teams_team_id_logo_file_id_delete) | **DELETE** /teams/{team_id}/logo/{file_id} | Delete team logo
[**delete_team_teams_team_id_delete**](TeamsApi.md#delete_team_teams_team_id_delete) | **DELETE** /teams/{team_id} | Delete a team
[**download_team_logo_teams_team_id_logo_file_id_get**](TeamsApi.md#download_team_logo_teams_team_id_logo_file_id_get) | **GET** /teams/{team_id}/logo/{file_id} | Download team logo
[**get_team_culture_teams_team_id_culture_get**](TeamsApi.md#get_team_culture_teams_team_id_culture_get) | **GET** /teams/{team_id}/culture | Get team culture details
[**get_team_rivals_teams_team_id_rivals_get**](TeamsApi.md#get_team_rivals_teams_team_id_rivals_get) | **GET** /teams/{team_id}/rivals | Get team&#39;s rivals
[**get_team_teams_team_id_get**](TeamsApi.md#get_team_teams_team_id_get) | **GET** /teams/{team_id} | Get a team by ID
[**list_team_logos_teams_team_id_logos_get**](TeamsApi.md#list_team_logos_teams_team_id_logos_get) | **GET** /teams/{team_id}/logos | List team logos
[**list_teams_teams_get**](TeamsApi.md#list_teams_teams_get) | **GET** /teams | List all teams
[**update_team_teams_team_id_patch**](TeamsApi.md#update_team_teams_team_id_patch) | **PATCH** /teams/{team_id} | Update a team
[**upload_team_logo_teams_team_id_logo_post**](TeamsApi.md#upload_team_logo_teams_team_id_logo_post) | **POST** /teams/{team_id}/logo | Upload team logo


# **create_team_teams_post**
> Team create_team_teams_post(team_create)

Create a new team

Add a new team to the league.

### Example

* Bearer Authentication (HTTPBearer):

```python
import openapi_client
from openapi_client.models.team import Team
from openapi_client.models.team_create import TeamCreate
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://believe.cjav.dev
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://believe.cjav.dev"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization: HTTPBearer
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.TeamsApi(api_client)
    team_create = openapi_client.TeamCreate() # TeamCreate | 

    try:
        # Create a new team
        api_response = api_instance.create_team_teams_post(team_create)
        print("The response of TeamsApi->create_team_teams_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TeamsApi->create_team_teams_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_create** | [**TeamCreate**](TeamCreate.md)|  | 

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
**201** | Team created successfully |  -  |
**409** | Team already exists |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_team_logo_teams_team_id_logo_file_id_delete**
> delete_team_logo_teams_team_id_logo_file_id_delete(team_id, file_id)

Delete team logo

Delete a team's logo.

### Example

* Bearer Authentication (HTTPBearer):

```python
import openapi_client
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://believe.cjav.dev
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://believe.cjav.dev"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization: HTTPBearer
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.TeamsApi(api_client)
    team_id = 'team_id_example' # str | 
    file_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Delete team logo
        api_instance.delete_team_logo_teams_team_id_logo_file_id_delete(team_id, file_id)
    except Exception as e:
        print("Exception when calling TeamsApi->delete_team_logo_teams_team_id_logo_file_id_delete: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **str**|  | 
 **file_id** | **UUID**|  | 

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
**204** | Logo deleted |  -  |
**404** | Team or file not found |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_team_teams_team_id_delete**
> delete_team_teams_team_id_delete(team_id)

Delete a team

Remove a team from the database (relegation to oblivion).

### Example

* Bearer Authentication (HTTPBearer):

```python
import openapi_client
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://believe.cjav.dev
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://believe.cjav.dev"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization: HTTPBearer
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.TeamsApi(api_client)
    team_id = 'team_id_example' # str | 

    try:
        # Delete a team
        api_instance.delete_team_teams_team_id_delete(team_id)
    except Exception as e:
        print("Exception when calling TeamsApi->delete_team_teams_team_id_delete: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **str**|  | 

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
**204** | Team deleted successfully |  -  |
**404** | Team not found |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **download_team_logo_teams_team_id_logo_file_id_get**
> object download_team_logo_teams_team_id_logo_file_id_get(team_id, file_id)

Download team logo

Download a team's logo by file ID.

### Example

* Bearer Authentication (HTTPBearer):

```python
import openapi_client
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://believe.cjav.dev
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://believe.cjav.dev"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization: HTTPBearer
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.TeamsApi(api_client)
    team_id = 'team_id_example' # str | 
    file_id = UUID('38400000-8cf0-11bd-b23e-10b96e4ef00d') # UUID | 

    try:
        # Download team logo
        api_response = api_instance.download_team_logo_teams_team_id_logo_file_id_get(team_id, file_id)
        print("The response of TeamsApi->download_team_logo_teams_team_id_logo_file_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TeamsApi->download_team_logo_teams_team_id_logo_file_id_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **str**|  | 
 **file_id** | **UUID**|  | 

### Return type

**object**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, image/*

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Logo file content |  -  |
**404** | Team or file not found |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_team_culture_teams_team_id_culture_get**
> Dict[str, object] get_team_culture_teams_team_id_culture_get(team_id)

Get team culture details

Get detailed culture and values information for a team.

### Example

* Bearer Authentication (HTTPBearer):

```python
import openapi_client
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://believe.cjav.dev
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://believe.cjav.dev"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization: HTTPBearer
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.TeamsApi(api_client)
    team_id = 'team_id_example' # str | 

    try:
        # Get team culture details
        api_response = api_instance.get_team_culture_teams_team_id_culture_get(team_id)
        print("The response of TeamsApi->get_team_culture_teams_team_id_culture_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TeamsApi->get_team_culture_teams_team_id_culture_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **str**|  | 

### Return type

**Dict[str, object]**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Team culture details |  -  |
**404** | Team not found |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_team_rivals_teams_team_id_rivals_get**
> List[Team] get_team_rivals_teams_team_id_rivals_get(team_id)

Get team's rivals

Get all rival teams for a specific team.

### Example

* Bearer Authentication (HTTPBearer):

```python
import openapi_client
from openapi_client.models.team import Team
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://believe.cjav.dev
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://believe.cjav.dev"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization: HTTPBearer
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.TeamsApi(api_client)
    team_id = 'team_id_example' # str | 

    try:
        # Get team's rivals
        api_response = api_instance.get_team_rivals_teams_team_id_rivals_get(team_id)
        print("The response of TeamsApi->get_team_rivals_teams_team_id_rivals_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TeamsApi->get_team_rivals_teams_team_id_rivals_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **str**|  | 

### Return type

[**List[Team]**](Team.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | List of rival teams |  -  |
**404** | Team not found |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_team_teams_team_id_get**
> Team get_team_teams_team_id_get(team_id)

Get a team by ID

Retrieve detailed information about a specific team.

### Example

* Bearer Authentication (HTTPBearer):

```python
import openapi_client
from openapi_client.models.team import Team
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://believe.cjav.dev
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://believe.cjav.dev"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization: HTTPBearer
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.TeamsApi(api_client)
    team_id = 'team_id_example' # str | 

    try:
        # Get a team by ID
        api_response = api_instance.get_team_teams_team_id_get(team_id)
        print("The response of TeamsApi->get_team_teams_team_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TeamsApi->get_team_teams_team_id_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **str**|  | 

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
**200** | Team details |  -  |
**404** | Team not found |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_team_logos_teams_team_id_logos_get**
> List[FileUploadResponse] list_team_logos_teams_team_id_logos_get(team_id)

List team logos

List all uploaded logos for a team.

### Example

* Bearer Authentication (HTTPBearer):

```python
import openapi_client
from openapi_client.models.file_upload_response import FileUploadResponse
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://believe.cjav.dev
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://believe.cjav.dev"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization: HTTPBearer
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.TeamsApi(api_client)
    team_id = 'team_id_example' # str | 

    try:
        # List team logos
        api_response = api_instance.list_team_logos_teams_team_id_logos_get(team_id)
        print("The response of TeamsApi->list_team_logos_teams_team_id_logos_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TeamsApi->list_team_logos_teams_team_id_logos_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **str**|  | 

### Return type

[**List[FileUploadResponse]**](FileUploadResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_teams_teams_get**
> PaginatedResponseTeam list_teams_teams_get(league=league, min_culture_score=min_culture_score, skip=skip, limit=limit)

List all teams

Get a paginated list of all teams with optional filtering by league or culture score.

### Example

* Bearer Authentication (HTTPBearer):

```python
import openapi_client
from openapi_client.models.paginated_response_team import PaginatedResponseTeam
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://believe.cjav.dev
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://believe.cjav.dev"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization: HTTPBearer
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.TeamsApi(api_client)
    league = openapi_client.League() # League | Filter by league (optional)
    min_culture_score = 56 # int | Minimum culture score (optional)
    skip = 0 # int | Number of items to skip (offset) (optional) (default to 0)
    limit = 20 # int | Maximum number of items to return (max: 100) (optional) (default to 20)

    try:
        # List all teams
        api_response = api_instance.list_teams_teams_get(league=league, min_culture_score=min_culture_score, skip=skip, limit=limit)
        print("The response of TeamsApi->list_teams_teams_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TeamsApi->list_teams_teams_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **league** | [**League**](.md)| Filter by league | [optional] 
 **min_culture_score** | **int**| Minimum culture score | [optional] 
 **skip** | **int**| Number of items to skip (offset) | [optional] [default to 0]
 **limit** | **int**| Maximum number of items to return (max: 100) | [optional] [default to 20]

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
**200** | Paginated list of teams |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_team_teams_team_id_patch**
> Team update_team_teams_team_id_patch(team_id, team_update)

Update a team

Update specific fields of an existing team.

### Example

* Bearer Authentication (HTTPBearer):

```python
import openapi_client
from openapi_client.models.team import Team
from openapi_client.models.team_update import TeamUpdate
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://believe.cjav.dev
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://believe.cjav.dev"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization: HTTPBearer
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.TeamsApi(api_client)
    team_id = 'team_id_example' # str | 
    team_update = openapi_client.TeamUpdate() # TeamUpdate | 

    try:
        # Update a team
        api_response = api_instance.update_team_teams_team_id_patch(team_id, team_update)
        print("The response of TeamsApi->update_team_teams_team_id_patch:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TeamsApi->update_team_teams_team_id_patch: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **str**|  | 
 **team_update** | [**TeamUpdate**](TeamUpdate.md)|  | 

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
**200** | Team updated successfully |  -  |
**404** | Team not found |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **upload_team_logo_teams_team_id_logo_post**
> FileUploadResponse upload_team_logo_teams_team_id_logo_post(team_id, file)

Upload team logo

Upload a logo image for a team. Accepts image files (jpg, png, gif, webp).

### Example

* Bearer Authentication (HTTPBearer):

```python
import openapi_client
from openapi_client.models.file_upload_response import FileUploadResponse
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://believe.cjav.dev
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://believe.cjav.dev"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization: HTTPBearer
configuration = openapi_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.TeamsApi(api_client)
    team_id = 'team_id_example' # str | 
    file = None # bytearray | Logo image file

    try:
        # Upload team logo
        api_response = api_instance.upload_team_logo_teams_team_id_logo_post(team_id, file)
        print("The response of TeamsApi->upload_team_logo_teams_team_id_logo_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TeamsApi->upload_team_logo_teams_team_id_logo_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **str**|  | 
 **file** | **bytearray**| Logo image file | 

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
**201** | Logo uploaded successfully |  -  |
**404** | Team not found |  -  |
**415** | Unsupported file type |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

