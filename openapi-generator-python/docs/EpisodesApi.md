# openapi_client.EpisodesApi

All URIs are relative to *https://believe.cjav.dev*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_episode_episodes_post**](EpisodesApi.md#create_episode_episodes_post) | **POST** /episodes | Create a new episode
[**delete_episode_episodes_episode_id_delete**](EpisodesApi.md#delete_episode_episodes_episode_id_delete) | **DELETE** /episodes/{episode_id} | Delete an episode
[**get_episode_episodes_episode_id_get**](EpisodesApi.md#get_episode_episodes_episode_id_get) | **GET** /episodes/{episode_id} | Get an episode by ID
[**get_episode_wisdom_episodes_episode_id_wisdom_get**](EpisodesApi.md#get_episode_wisdom_episodes_episode_id_wisdom_get) | **GET** /episodes/{episode_id}/wisdom | Get episode wisdom
[**get_season_episodes_episodes_seasons_season_number_get**](EpisodesApi.md#get_season_episodes_episodes_seasons_season_number_get) | **GET** /episodes/seasons/{season_number} | Get all episodes from a season
[**list_episodes_episodes_get**](EpisodesApi.md#list_episodes_episodes_get) | **GET** /episodes | List all episodes
[**update_episode_episodes_episode_id_patch**](EpisodesApi.md#update_episode_episodes_episode_id_patch) | **PATCH** /episodes/{episode_id} | Update an episode


# **create_episode_episodes_post**
> Episode create_episode_episodes_post(episode_create)

Create a new episode

Add a new episode to the series.

### Example

* Bearer Authentication (HTTPBearer):

```python
import openapi_client
from openapi_client.models.episode import Episode
from openapi_client.models.episode_create import EpisodeCreate
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
    api_instance = openapi_client.EpisodesApi(api_client)
    episode_create = openapi_client.EpisodeCreate() # EpisodeCreate | 

    try:
        # Create a new episode
        api_response = api_instance.create_episode_episodes_post(episode_create)
        print("The response of EpisodesApi->create_episode_episodes_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EpisodesApi->create_episode_episodes_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **episode_create** | [**EpisodeCreate**](EpisodeCreate.md)|  | 

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
**201** | Episode created successfully |  -  |
**409** | Episode already exists |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_episode_episodes_episode_id_delete**
> delete_episode_episodes_episode_id_delete(episode_id)

Delete an episode

Remove an episode from the database.

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
    api_instance = openapi_client.EpisodesApi(api_client)
    episode_id = 'episode_id_example' # str | 

    try:
        # Delete an episode
        api_instance.delete_episode_episodes_episode_id_delete(episode_id)
    except Exception as e:
        print("Exception when calling EpisodesApi->delete_episode_episodes_episode_id_delete: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **episode_id** | **str**|  | 

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
**204** | Episode deleted successfully |  -  |
**404** | Episode not found |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_episode_episodes_episode_id_get**
> Episode get_episode_episodes_episode_id_get(episode_id)

Get an episode by ID

Retrieve detailed information about a specific episode.

### Example

* Bearer Authentication (HTTPBearer):

```python
import openapi_client
from openapi_client.models.episode import Episode
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
    api_instance = openapi_client.EpisodesApi(api_client)
    episode_id = 'episode_id_example' # str | 

    try:
        # Get an episode by ID
        api_response = api_instance.get_episode_episodes_episode_id_get(episode_id)
        print("The response of EpisodesApi->get_episode_episodes_episode_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EpisodesApi->get_episode_episodes_episode_id_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **episode_id** | **str**|  | 

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
**200** | Episode details |  -  |
**404** | Episode not found |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_episode_wisdom_episodes_episode_id_wisdom_get**
> Dict[str, object] get_episode_wisdom_episodes_episode_id_wisdom_get(episode_id)

Get episode wisdom

Get Ted's wisdom and memorable moments from a specific episode.

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
    api_instance = openapi_client.EpisodesApi(api_client)
    episode_id = 'episode_id_example' # str | 

    try:
        # Get episode wisdom
        api_response = api_instance.get_episode_wisdom_episodes_episode_id_wisdom_get(episode_id)
        print("The response of EpisodesApi->get_episode_wisdom_episodes_episode_id_wisdom_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EpisodesApi->get_episode_wisdom_episodes_episode_id_wisdom_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **episode_id** | **str**|  | 

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
**200** | Episode wisdom details |  -  |
**404** | Episode not found |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_season_episodes_episodes_seasons_season_number_get**
> PaginatedResponseEpisode get_season_episodes_episodes_seasons_season_number_get(season_number, skip=skip, limit=limit)

Get all episodes from a season

Get a paginated list of episodes from a specific season.

### Example

* Bearer Authentication (HTTPBearer):

```python
import openapi_client
from openapi_client.models.paginated_response_episode import PaginatedResponseEpisode
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
    api_instance = openapi_client.EpisodesApi(api_client)
    season_number = 56 # int | 
    skip = 0 # int | Number of items to skip (offset) (optional) (default to 0)
    limit = 20 # int | Maximum number of items to return (max: 100) (optional) (default to 20)

    try:
        # Get all episodes from a season
        api_response = api_instance.get_season_episodes_episodes_seasons_season_number_get(season_number, skip=skip, limit=limit)
        print("The response of EpisodesApi->get_season_episodes_episodes_seasons_season_number_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EpisodesApi->get_season_episodes_episodes_seasons_season_number_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **season_number** | **int**|  | 
 **skip** | **int**| Number of items to skip (offset) | [optional] [default to 0]
 **limit** | **int**| Maximum number of items to return (max: 100) | [optional] [default to 20]

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
**200** | Paginated list of episodes from the season |  -  |
**404** | Season not found |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_episodes_episodes_get**
> PaginatedResponseEpisode list_episodes_episodes_get(season=season, character_focus=character_focus, skip=skip, limit=limit)

List all episodes

Get a paginated list of all Ted Lasso episodes with optional filtering by season.

### Example

* Bearer Authentication (HTTPBearer):

```python
import openapi_client
from openapi_client.models.paginated_response_episode import PaginatedResponseEpisode
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
    api_instance = openapi_client.EpisodesApi(api_client)
    season = 56 # int | Filter by season (optional)
    character_focus = 'character_focus_example' # str | Filter by character focus (character ID) (optional)
    skip = 0 # int | Number of items to skip (offset) (optional) (default to 0)
    limit = 20 # int | Maximum number of items to return (max: 100) (optional) (default to 20)

    try:
        # List all episodes
        api_response = api_instance.list_episodes_episodes_get(season=season, character_focus=character_focus, skip=skip, limit=limit)
        print("The response of EpisodesApi->list_episodes_episodes_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EpisodesApi->list_episodes_episodes_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **season** | **int**| Filter by season | [optional] 
 **character_focus** | **str**| Filter by character focus (character ID) | [optional] 
 **skip** | **int**| Number of items to skip (offset) | [optional] [default to 0]
 **limit** | **int**| Maximum number of items to return (max: 100) | [optional] [default to 20]

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
**200** | Paginated list of episodes |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_episode_episodes_episode_id_patch**
> Episode update_episode_episodes_episode_id_patch(episode_id, episode_update)

Update an episode

Update specific fields of an existing episode.

### Example

* Bearer Authentication (HTTPBearer):

```python
import openapi_client
from openapi_client.models.episode import Episode
from openapi_client.models.episode_update import EpisodeUpdate
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
    api_instance = openapi_client.EpisodesApi(api_client)
    episode_id = 'episode_id_example' # str | 
    episode_update = openapi_client.EpisodeUpdate() # EpisodeUpdate | 

    try:
        # Update an episode
        api_response = api_instance.update_episode_episodes_episode_id_patch(episode_id, episode_update)
        print("The response of EpisodesApi->update_episode_episodes_episode_id_patch:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EpisodesApi->update_episode_episodes_episode_id_patch: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **episode_id** | **str**|  | 
 **episode_update** | [**EpisodeUpdate**](EpisodeUpdate.md)|  | 

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
**200** | Episode updated successfully |  -  |
**404** | Episode not found |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

