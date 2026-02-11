# openapi_client.MatchesApi

All URIs are relative to *https://believe.cjav.dev*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_match_matches_post**](MatchesApi.md#create_match_matches_post) | **POST** /matches | Create a new match
[**delete_match_matches_match_id_delete**](MatchesApi.md#delete_match_matches_match_id_delete) | **DELETE** /matches/{match_id} | Delete a match
[**get_match_lesson_matches_match_id_lesson_get**](MatchesApi.md#get_match_lesson_matches_match_id_lesson_get) | **GET** /matches/{match_id}/lesson | Get match lesson
[**get_match_matches_match_id_get**](MatchesApi.md#get_match_matches_match_id_get) | **GET** /matches/{match_id} | Get a match by ID
[**get_turning_points_matches_match_id_turning_points_get**](MatchesApi.md#get_turning_points_matches_match_id_turning_points_get) | **GET** /matches/{match_id}/turning-points | Get match turning points
[**list_matches_matches_get**](MatchesApi.md#list_matches_matches_get) | **GET** /matches | List all matches
[**update_match_matches_match_id_patch**](MatchesApi.md#update_match_matches_match_id_patch) | **PATCH** /matches/{match_id} | Update a match


# **create_match_matches_post**
> Match create_match_matches_post(match_create)

Create a new match

Schedule a new match.

### Example

* Bearer Authentication (HTTPBearer):

```python
import openapi_client
from openapi_client.models.match import Match
from openapi_client.models.match_create import MatchCreate
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
    api_instance = openapi_client.MatchesApi(api_client)
    match_create = openapi_client.MatchCreate() # MatchCreate | 

    try:
        # Create a new match
        api_response = api_instance.create_match_matches_post(match_create)
        print("The response of MatchesApi->create_match_matches_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MatchesApi->create_match_matches_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **match_create** | [**MatchCreate**](MatchCreate.md)|  | 

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
**201** | Match created successfully |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_match_matches_match_id_delete**
> delete_match_matches_match_id_delete(match_id)

Delete a match

Remove a match from the database.

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
    api_instance = openapi_client.MatchesApi(api_client)
    match_id = 'match_id_example' # str | 

    try:
        # Delete a match
        api_instance.delete_match_matches_match_id_delete(match_id)
    except Exception as e:
        print("Exception when calling MatchesApi->delete_match_matches_match_id_delete: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **match_id** | **str**|  | 

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
**204** | Match deleted successfully |  -  |
**404** | Match not found |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_match_lesson_matches_match_id_lesson_get**
> Dict[str, object] get_match_lesson_matches_match_id_lesson_get(match_id)

Get match lesson

Get the life lesson learned from a specific match.

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
    api_instance = openapi_client.MatchesApi(api_client)
    match_id = 'match_id_example' # str | 

    try:
        # Get match lesson
        api_response = api_instance.get_match_lesson_matches_match_id_lesson_get(match_id)
        print("The response of MatchesApi->get_match_lesson_matches_match_id_lesson_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MatchesApi->get_match_lesson_matches_match_id_lesson_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **match_id** | **str**|  | 

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
**200** | Match lesson details |  -  |
**404** | Match not found |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_match_matches_match_id_get**
> Match get_match_matches_match_id_get(match_id)

Get a match by ID

Retrieve detailed information about a specific match.

### Example

* Bearer Authentication (HTTPBearer):

```python
import openapi_client
from openapi_client.models.match import Match
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
    api_instance = openapi_client.MatchesApi(api_client)
    match_id = 'match_id_example' # str | 

    try:
        # Get a match by ID
        api_response = api_instance.get_match_matches_match_id_get(match_id)
        print("The response of MatchesApi->get_match_matches_match_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MatchesApi->get_match_matches_match_id_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **match_id** | **str**|  | 

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
**200** | Match details |  -  |
**404** | Match not found |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_turning_points_matches_match_id_turning_points_get**
> List[Dict[str, object]] get_turning_points_matches_match_id_turning_points_get(match_id)

Get match turning points

Get all turning points from a specific match.

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
    api_instance = openapi_client.MatchesApi(api_client)
    match_id = 'match_id_example' # str | 

    try:
        # Get match turning points
        api_response = api_instance.get_turning_points_matches_match_id_turning_points_get(match_id)
        print("The response of MatchesApi->get_turning_points_matches_match_id_turning_points_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MatchesApi->get_turning_points_matches_match_id_turning_points_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **match_id** | **str**|  | 

### Return type

**List[Dict[str, object]]**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | List of turning points |  -  |
**404** | Match not found |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_matches_matches_get**
> PaginatedResponseMatch list_matches_matches_get(team_id=team_id, result=result, match_type=match_type, skip=skip, limit=limit)

List all matches

Get a paginated list of all matches with optional filtering.

### Example

* Bearer Authentication (HTTPBearer):

```python
import openapi_client
from openapi_client.models.paginated_response_match import PaginatedResponseMatch
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
    api_instance = openapi_client.MatchesApi(api_client)
    team_id = 'team_id_example' # str | Filter by team (home or away) (optional)
    result = openapi_client.MatchResult() # MatchResult | Filter by result (optional)
    match_type = openapi_client.MatchType() # MatchType | Filter by match type (optional)
    skip = 0 # int | Number of items to skip (offset) (optional) (default to 0)
    limit = 20 # int | Maximum number of items to return (max: 100) (optional) (default to 20)

    try:
        # List all matches
        api_response = api_instance.list_matches_matches_get(team_id=team_id, result=result, match_type=match_type, skip=skip, limit=limit)
        print("The response of MatchesApi->list_matches_matches_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MatchesApi->list_matches_matches_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **str**| Filter by team (home or away) | [optional] 
 **result** | [**MatchResult**](.md)| Filter by result | [optional] 
 **match_type** | [**MatchType**](.md)| Filter by match type | [optional] 
 **skip** | **int**| Number of items to skip (offset) | [optional] [default to 0]
 **limit** | **int**| Maximum number of items to return (max: 100) | [optional] [default to 20]

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
**200** | Paginated list of matches |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_match_matches_match_id_patch**
> Match update_match_matches_match_id_patch(match_id, match_update)

Update a match

Update specific fields of an existing match (e.g., update score).

### Example

* Bearer Authentication (HTTPBearer):

```python
import openapi_client
from openapi_client.models.match import Match
from openapi_client.models.match_update import MatchUpdate
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
    api_instance = openapi_client.MatchesApi(api_client)
    match_id = 'match_id_example' # str | 
    match_update = openapi_client.MatchUpdate() # MatchUpdate | 

    try:
        # Update a match
        api_response = api_instance.update_match_matches_match_id_patch(match_id, match_update)
        print("The response of MatchesApi->update_match_matches_match_id_patch:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MatchesApi->update_match_matches_match_id_patch: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **match_id** | **str**|  | 
 **match_update** | [**MatchUpdate**](MatchUpdate.md)|  | 

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
**200** | Match updated successfully |  -  |
**404** | Match not found |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

