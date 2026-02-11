# openapi_client.CharactersApi

All URIs are relative to *https://believe.cjav.dev*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_character_characters_post**](CharactersApi.md#create_character_characters_post) | **POST** /characters | Create a new character
[**delete_character_characters_character_id_delete**](CharactersApi.md#delete_character_characters_character_id_delete) | **DELETE** /characters/{character_id} | Delete a character
[**get_character_characters_character_id_get**](CharactersApi.md#get_character_characters_character_id_get) | **GET** /characters/{character_id} | Get a character by ID
[**get_character_quotes_characters_character_id_quotes_get**](CharactersApi.md#get_character_quotes_characters_character_id_quotes_get) | **GET** /characters/{character_id}/quotes | Get character&#39;s signature quotes
[**list_characters_characters_get**](CharactersApi.md#list_characters_characters_get) | **GET** /characters | List all characters
[**update_character_characters_character_id_patch**](CharactersApi.md#update_character_characters_character_id_patch) | **PATCH** /characters/{character_id} | Update a character


# **create_character_characters_post**
> Character create_character_characters_post(character_create)

Create a new character

Add a new character to the Ted Lasso universe.

### Example

* Bearer Authentication (HTTPBearer):

```python
import openapi_client
from openapi_client.models.character import Character
from openapi_client.models.character_create import CharacterCreate
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
    api_instance = openapi_client.CharactersApi(api_client)
    character_create = openapi_client.CharacterCreate() # CharacterCreate | 

    try:
        # Create a new character
        api_response = api_instance.create_character_characters_post(character_create)
        print("The response of CharactersApi->create_character_characters_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CharactersApi->create_character_characters_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **character_create** | [**CharacterCreate**](CharacterCreate.md)|  | 

### Return type

[**Character**](Character.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Character created successfully |  -  |
**409** | Character already exists |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_character_characters_character_id_delete**
> delete_character_characters_character_id_delete(character_id)

Delete a character

Remove a character from the database.

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
    api_instance = openapi_client.CharactersApi(api_client)
    character_id = 'character_id_example' # str | 

    try:
        # Delete a character
        api_instance.delete_character_characters_character_id_delete(character_id)
    except Exception as e:
        print("Exception when calling CharactersApi->delete_character_characters_character_id_delete: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **character_id** | **str**|  | 

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
**204** | Character deleted successfully |  -  |
**404** | Character not found |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_character_characters_character_id_get**
> Character get_character_characters_character_id_get(character_id)

Get a character by ID

Retrieve detailed information about a specific character.

### Example

* Bearer Authentication (HTTPBearer):

```python
import openapi_client
from openapi_client.models.character import Character
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
    api_instance = openapi_client.CharactersApi(api_client)
    character_id = 'character_id_example' # str | 

    try:
        # Get a character by ID
        api_response = api_instance.get_character_characters_character_id_get(character_id)
        print("The response of CharactersApi->get_character_characters_character_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CharactersApi->get_character_characters_character_id_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **character_id** | **str**|  | 

### Return type

[**Character**](Character.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Character details |  -  |
**404** | Character not found |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_character_quotes_characters_character_id_quotes_get**
> List[Optional[str]] get_character_quotes_characters_character_id_quotes_get(character_id)

Get character's signature quotes

Get all signature quotes from a specific character.

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
    api_instance = openapi_client.CharactersApi(api_client)
    character_id = 'character_id_example' # str | 

    try:
        # Get character's signature quotes
        api_response = api_instance.get_character_quotes_characters_character_id_quotes_get(character_id)
        print("The response of CharactersApi->get_character_quotes_characters_character_id_quotes_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CharactersApi->get_character_quotes_characters_character_id_quotes_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **character_id** | **str**|  | 

### Return type

**List[Optional[str]]**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | List of signature quotes |  -  |
**404** | Character not found |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_characters_characters_get**
> PaginatedResponseCharacter list_characters_characters_get(role=role, team_id=team_id, min_optimism=min_optimism, skip=skip, limit=limit)

List all characters

Get a paginated list of Ted Lasso characters.

### Example

* Bearer Authentication (HTTPBearer):

```python
import openapi_client
from openapi_client.models.paginated_response_character import PaginatedResponseCharacter
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
    api_instance = openapi_client.CharactersApi(api_client)
    role = openapi_client.CharacterRole() # CharacterRole | Filter by role (optional)
    team_id = 'team_id_example' # str | Filter by team ID (optional)
    min_optimism = 56 # int | Minimum optimism score (optional)
    skip = 0 # int | Number of items to skip (offset) (optional) (default to 0)
    limit = 20 # int | Maximum number of items to return (max: 100) (optional) (default to 20)

    try:
        # List all characters
        api_response = api_instance.list_characters_characters_get(role=role, team_id=team_id, min_optimism=min_optimism, skip=skip, limit=limit)
        print("The response of CharactersApi->list_characters_characters_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CharactersApi->list_characters_characters_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **role** | [**CharacterRole**](.md)| Filter by role | [optional] 
 **team_id** | **str**| Filter by team ID | [optional] 
 **min_optimism** | **int**| Minimum optimism score | [optional] 
 **skip** | **int**| Number of items to skip (offset) | [optional] [default to 0]
 **limit** | **int**| Maximum number of items to return (max: 100) | [optional] [default to 20]

### Return type

[**PaginatedResponseCharacter**](PaginatedResponseCharacter.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Paginated list of characters |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_character_characters_character_id_patch**
> Character update_character_characters_character_id_patch(character_id, character_update)

Update a character

Update specific fields of an existing character.

### Example

* Bearer Authentication (HTTPBearer):

```python
import openapi_client
from openapi_client.models.character import Character
from openapi_client.models.character_update import CharacterUpdate
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
    api_instance = openapi_client.CharactersApi(api_client)
    character_id = 'character_id_example' # str | 
    character_update = openapi_client.CharacterUpdate() # CharacterUpdate | 

    try:
        # Update a character
        api_response = api_instance.update_character_characters_character_id_patch(character_id, character_update)
        print("The response of CharactersApi->update_character_characters_character_id_patch:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CharactersApi->update_character_characters_character_id_patch: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **character_id** | **str**|  | 
 **character_update** | [**CharacterUpdate**](CharacterUpdate.md)|  | 

### Return type

[**Character**](Character.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Character updated successfully |  -  |
**404** | Character not found |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

