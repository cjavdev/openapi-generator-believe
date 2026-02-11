# openapi_client.QuotesApi

All URIs are relative to *https://believe.cjav.dev*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_quote_quotes_post**](QuotesApi.md#create_quote_quotes_post) | **POST** /quotes | Create a new quote
[**delete_quote_quotes_quote_id_delete**](QuotesApi.md#delete_quote_quotes_quote_id_delete) | **DELETE** /quotes/{quote_id} | Delete a quote
[**get_character_quotes_quotes_characters_character_id_get**](QuotesApi.md#get_character_quotes_quotes_characters_character_id_get) | **GET** /quotes/characters/{character_id} | Get all quotes by a character
[**get_quote_quotes_quote_id_get**](QuotesApi.md#get_quote_quotes_quote_id_get) | **GET** /quotes/{quote_id} | Get a quote by ID
[**get_quotes_by_theme_quotes_themes_theme_get**](QuotesApi.md#get_quotes_by_theme_quotes_themes_theme_get) | **GET** /quotes/themes/{theme} | Get quotes by theme
[**get_random_quote_quotes_random_get**](QuotesApi.md#get_random_quote_quotes_random_get) | **GET** /quotes/random | Get a random quote
[**list_quotes_quotes_get**](QuotesApi.md#list_quotes_quotes_get) | **GET** /quotes | List all quotes
[**update_quote_quotes_quote_id_patch**](QuotesApi.md#update_quote_quotes_quote_id_patch) | **PATCH** /quotes/{quote_id} | Update a quote


# **create_quote_quotes_post**
> Quote create_quote_quotes_post(quote_create)

Create a new quote

Add a new memorable quote to the collection.

### Example

* Bearer Authentication (HTTPBearer):

```python
import openapi_client
from openapi_client.models.quote import Quote
from openapi_client.models.quote_create import QuoteCreate
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
    api_instance = openapi_client.QuotesApi(api_client)
    quote_create = openapi_client.QuoteCreate() # QuoteCreate | 

    try:
        # Create a new quote
        api_response = api_instance.create_quote_quotes_post(quote_create)
        print("The response of QuotesApi->create_quote_quotes_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling QuotesApi->create_quote_quotes_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **quote_create** | [**QuoteCreate**](QuoteCreate.md)|  | 

### Return type

[**Quote**](Quote.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Quote created successfully |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_quote_quotes_quote_id_delete**
> delete_quote_quotes_quote_id_delete(quote_id)

Delete a quote

Remove a quote from the collection.

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
    api_instance = openapi_client.QuotesApi(api_client)
    quote_id = 'quote_id_example' # str | 

    try:
        # Delete a quote
        api_instance.delete_quote_quotes_quote_id_delete(quote_id)
    except Exception as e:
        print("Exception when calling QuotesApi->delete_quote_quotes_quote_id_delete: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **quote_id** | **str**|  | 

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
**204** | Quote deleted successfully |  -  |
**404** | Quote not found |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_character_quotes_quotes_characters_character_id_get**
> PaginatedResponseQuote get_character_quotes_quotes_characters_character_id_get(character_id, skip=skip, limit=limit)

Get all quotes by a character

Get a paginated list of quotes from a specific character.

### Example

* Bearer Authentication (HTTPBearer):

```python
import openapi_client
from openapi_client.models.paginated_response_quote import PaginatedResponseQuote
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
    api_instance = openapi_client.QuotesApi(api_client)
    character_id = 'character_id_example' # str | 
    skip = 0 # int | Number of items to skip (offset) (optional) (default to 0)
    limit = 20 # int | Maximum number of items to return (max: 100) (optional) (default to 20)

    try:
        # Get all quotes by a character
        api_response = api_instance.get_character_quotes_quotes_characters_character_id_get(character_id, skip=skip, limit=limit)
        print("The response of QuotesApi->get_character_quotes_quotes_characters_character_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling QuotesApi->get_character_quotes_quotes_characters_character_id_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **character_id** | **str**|  | 
 **skip** | **int**| Number of items to skip (offset) | [optional] [default to 0]
 **limit** | **int**| Maximum number of items to return (max: 100) | [optional] [default to 20]

### Return type

[**PaginatedResponseQuote**](PaginatedResponseQuote.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Paginated list of quotes from the character |  -  |
**404** | No quotes found for character |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_quote_quotes_quote_id_get**
> Quote get_quote_quotes_quote_id_get(quote_id)

Get a quote by ID

Retrieve a specific quote by its ID.

### Example

* Bearer Authentication (HTTPBearer):

```python
import openapi_client
from openapi_client.models.quote import Quote
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
    api_instance = openapi_client.QuotesApi(api_client)
    quote_id = 'quote_id_example' # str | 

    try:
        # Get a quote by ID
        api_response = api_instance.get_quote_quotes_quote_id_get(quote_id)
        print("The response of QuotesApi->get_quote_quotes_quote_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling QuotesApi->get_quote_quotes_quote_id_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **quote_id** | **str**|  | 

### Return type

[**Quote**](Quote.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Quote details |  -  |
**404** | Quote not found |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_quotes_by_theme_quotes_themes_theme_get**
> PaginatedResponseQuote get_quotes_by_theme_quotes_themes_theme_get(theme, skip=skip, limit=limit)

Get quotes by theme

Get a paginated list of quotes related to a specific theme.

### Example

* Bearer Authentication (HTTPBearer):

```python
import openapi_client
from openapi_client.models.paginated_response_quote import PaginatedResponseQuote
from openapi_client.models.quote_theme import QuoteTheme
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
    api_instance = openapi_client.QuotesApi(api_client)
    theme = openapi_client.QuoteTheme() # QuoteTheme | 
    skip = 0 # int | Number of items to skip (offset) (optional) (default to 0)
    limit = 20 # int | Maximum number of items to return (max: 100) (optional) (default to 20)

    try:
        # Get quotes by theme
        api_response = api_instance.get_quotes_by_theme_quotes_themes_theme_get(theme, skip=skip, limit=limit)
        print("The response of QuotesApi->get_quotes_by_theme_quotes_themes_theme_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling QuotesApi->get_quotes_by_theme_quotes_themes_theme_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **theme** | [**QuoteTheme**](.md)|  | 
 **skip** | **int**| Number of items to skip (offset) | [optional] [default to 0]
 **limit** | **int**| Maximum number of items to return (max: 100) | [optional] [default to 20]

### Return type

[**PaginatedResponseQuote**](PaginatedResponseQuote.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Paginated list of quotes for the theme |  -  |
**404** | No quotes found for theme |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_random_quote_quotes_random_get**
> Quote get_random_quote_quotes_random_get(character_id=character_id, theme=theme, inspirational=inspirational)

Get a random quote

Get a random Ted Lasso quote, optionally filtered.

### Example

* Bearer Authentication (HTTPBearer):

```python
import openapi_client
from openapi_client.models.quote import Quote
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
    api_instance = openapi_client.QuotesApi(api_client)
    character_id = 'character_id_example' # str | Filter by character (optional)
    theme = openapi_client.QuoteTheme() # QuoteTheme | Filter by theme (optional)
    inspirational = True # bool | Filter inspirational quotes (optional)

    try:
        # Get a random quote
        api_response = api_instance.get_random_quote_quotes_random_get(character_id=character_id, theme=theme, inspirational=inspirational)
        print("The response of QuotesApi->get_random_quote_quotes_random_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling QuotesApi->get_random_quote_quotes_random_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **character_id** | **str**| Filter by character | [optional] 
 **theme** | [**QuoteTheme**](.md)| Filter by theme | [optional] 
 **inspirational** | **bool**| Filter inspirational quotes | [optional] 

### Return type

[**Quote**](Quote.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | A random quote |  -  |
**404** | No quotes found matching criteria |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_quotes_quotes_get**
> PaginatedResponseQuote list_quotes_quotes_get(character_id=character_id, theme=theme, moment_type=moment_type, inspirational=inspirational, funny=funny, skip=skip, limit=limit)

List all quotes

Get a paginated list of all memorable Ted Lasso quotes with optional filtering.

### Example

* Bearer Authentication (HTTPBearer):

```python
import openapi_client
from openapi_client.models.paginated_response_quote import PaginatedResponseQuote
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
    api_instance = openapi_client.QuotesApi(api_client)
    character_id = 'character_id_example' # str | Filter by character (optional)
    theme = openapi_client.QuoteTheme() # QuoteTheme | Filter by theme (optional)
    moment_type = openapi_client.QuoteMoment() # QuoteMoment | Filter by moment type (optional)
    inspirational = True # bool | Filter inspirational quotes (optional)
    funny = True # bool | Filter funny quotes (optional)
    skip = 0 # int | Number of items to skip (offset) (optional) (default to 0)
    limit = 20 # int | Maximum number of items to return (max: 100) (optional) (default to 20)

    try:
        # List all quotes
        api_response = api_instance.list_quotes_quotes_get(character_id=character_id, theme=theme, moment_type=moment_type, inspirational=inspirational, funny=funny, skip=skip, limit=limit)
        print("The response of QuotesApi->list_quotes_quotes_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling QuotesApi->list_quotes_quotes_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **character_id** | **str**| Filter by character | [optional] 
 **theme** | [**QuoteTheme**](.md)| Filter by theme | [optional] 
 **moment_type** | [**QuoteMoment**](.md)| Filter by moment type | [optional] 
 **inspirational** | **bool**| Filter inspirational quotes | [optional] 
 **funny** | **bool**| Filter funny quotes | [optional] 
 **skip** | **int**| Number of items to skip (offset) | [optional] [default to 0]
 **limit** | **int**| Maximum number of items to return (max: 100) | [optional] [default to 20]

### Return type

[**PaginatedResponseQuote**](PaginatedResponseQuote.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Paginated list of quotes |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_quote_quotes_quote_id_patch**
> Quote update_quote_quotes_quote_id_patch(quote_id, quote_update)

Update a quote

Update specific fields of an existing quote.

### Example

* Bearer Authentication (HTTPBearer):

```python
import openapi_client
from openapi_client.models.quote import Quote
from openapi_client.models.quote_update import QuoteUpdate
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
    api_instance = openapi_client.QuotesApi(api_client)
    quote_id = 'quote_id_example' # str | 
    quote_update = openapi_client.QuoteUpdate() # QuoteUpdate | 

    try:
        # Update a quote
        api_response = api_instance.update_quote_quotes_quote_id_patch(quote_id, quote_update)
        print("The response of QuotesApi->update_quote_quotes_quote_id_patch:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling QuotesApi->update_quote_quotes_quote_id_patch: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **quote_id** | **str**|  | 
 **quote_update** | [**QuoteUpdate**](QuoteUpdate.md)|  | 

### Return type

[**Quote**](Quote.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Quote updated successfully |  -  |
**404** | Quote not found |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

