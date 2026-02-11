# openapi_client.InteractiveApi

All URIs are relative to *https://believe.cjav.dev*

Method | HTTP request | Description
------------- | ------------- | -------------
[**believe_engine_believe_post**](InteractiveApi.md#believe_engine_believe_post) | **POST** /believe | The Believe Engine
[**get_biscuit_biscuits_biscuit_id_get**](InteractiveApi.md#get_biscuit_biscuits_biscuit_id_get) | **GET** /biscuits/{biscuit_id} | Get a Specific Biscuit
[**get_biscuits_biscuits_get**](InteractiveApi.md#get_biscuits_biscuits_get) | **GET** /biscuits | Biscuits as a Service
[**get_coaching_principle_coaching_principles_principle_id_get**](InteractiveApi.md#get_coaching_principle_coaching_principles_principle_id_get) | **GET** /coaching/principles/{principle_id} | Get a Specific Coaching Principle
[**get_coaching_principles_coaching_principles_get**](InteractiveApi.md#get_coaching_principles_coaching_principles_get) | **GET** /coaching/principles | Get Coaching Principles
[**get_fresh_biscuit_biscuits_fresh_get**](InteractiveApi.md#get_fresh_biscuit_biscuits_fresh_get) | **GET** /biscuits/fresh | Get a Fresh Biscuit
[**get_random_principle_coaching_principles_random_get**](InteractiveApi.md#get_random_principle_coaching_principles_random_get) | **GET** /coaching/principles/random | Get a Random Coaching Principle
[**press_conference_press_post**](InteractiveApi.md#press_conference_press_post) | **POST** /press | Press Conference Simulator
[**reframe_thought_reframe_post**](InteractiveApi.md#reframe_thought_reframe_post) | **POST** /reframe | Reframe Negative Thoughts
[**resolve_conflict_conflicts_resolve_post**](InteractiveApi.md#resolve_conflict_conflicts_resolve_post) | **POST** /conflicts/resolve | Resolve Conflicts


# **believe_engine_believe_post**
> BelieveResponse believe_engine_believe_post(believe_request)

The Believe Engine

Submit your situation and receive Ted Lasso-style motivational guidance.

### Example

* Bearer Authentication (HTTPBearer):

```python
import openapi_client
from openapi_client.models.believe_request import BelieveRequest
from openapi_client.models.believe_response import BelieveResponse
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
    api_instance = openapi_client.InteractiveApi(api_client)
    believe_request = openapi_client.BelieveRequest() # BelieveRequest | 

    try:
        # The Believe Engine
        api_response = api_instance.believe_engine_believe_post(believe_request)
        print("The response of InteractiveApi->believe_engine_believe_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InteractiveApi->believe_engine_believe_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **believe_request** | [**BelieveRequest**](BelieveRequest.md)|  | 

### Return type

[**BelieveResponse**](BelieveResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Motivational response generated |  -  |
**418** | You&#39;re already a believer! |  -  |
**422** | Validation Error |  -  |
**429** | Too much negativity detected |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_biscuit_biscuits_biscuit_id_get**
> Biscuit get_biscuit_biscuits_biscuit_id_get(biscuit_id)

Get a Specific Biscuit

Get a specific type of biscuit by ID.

### Example

* Bearer Authentication (HTTPBearer):

```python
import openapi_client
from openapi_client.models.biscuit import Biscuit
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
    api_instance = openapi_client.InteractiveApi(api_client)
    biscuit_id = 'biscuit_id_example' # str | 

    try:
        # Get a Specific Biscuit
        api_response = api_instance.get_biscuit_biscuits_biscuit_id_get(biscuit_id)
        print("The response of InteractiveApi->get_biscuit_biscuits_biscuit_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InteractiveApi->get_biscuit_biscuits_biscuit_id_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **biscuit_id** | **str**|  | 

### Return type

[**Biscuit**](Biscuit.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Biscuit details |  -  |
**404** | Biscuit not found |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_biscuits_biscuits_get**
> PaginatedResponseBiscuit get_biscuits_biscuits_get(skip=skip, limit=limit)

Biscuits as a Service

Get a paginated list of Ted's famous homemade biscuits! Each comes with a heartwarming message.

### Example

* Bearer Authentication (HTTPBearer):

```python
import openapi_client
from openapi_client.models.paginated_response_biscuit import PaginatedResponseBiscuit
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
    api_instance = openapi_client.InteractiveApi(api_client)
    skip = 0 # int | Number of items to skip (offset) (optional) (default to 0)
    limit = 20 # int | Maximum number of items to return (max: 100) (optional) (default to 20)

    try:
        # Biscuits as a Service
        api_response = api_instance.get_biscuits_biscuits_get(skip=skip, limit=limit)
        print("The response of InteractiveApi->get_biscuits_biscuits_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InteractiveApi->get_biscuits_biscuits_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **skip** | **int**| Number of items to skip (offset) | [optional] [default to 0]
 **limit** | **int**| Maximum number of items to return (max: 100) | [optional] [default to 20]

### Return type

[**PaginatedResponseBiscuit**](PaginatedResponseBiscuit.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Paginated list of fresh biscuits from Ted&#39;s kitchen |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_coaching_principle_coaching_principles_principle_id_get**
> CoachingPrinciple get_coaching_principle_coaching_principles_principle_id_get(principle_id)

Get a Specific Coaching Principle

Get details about a specific coaching principle.

### Example

* Bearer Authentication (HTTPBearer):

```python
import openapi_client
from openapi_client.models.coaching_principle import CoachingPrinciple
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
    api_instance = openapi_client.InteractiveApi(api_client)
    principle_id = 'principle_id_example' # str | 

    try:
        # Get a Specific Coaching Principle
        api_response = api_instance.get_coaching_principle_coaching_principles_principle_id_get(principle_id)
        print("The response of InteractiveApi->get_coaching_principle_coaching_principles_principle_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InteractiveApi->get_coaching_principle_coaching_principles_principle_id_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **principle_id** | **str**|  | 

### Return type

[**CoachingPrinciple**](CoachingPrinciple.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Coaching principle details |  -  |
**404** | Principle not found |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_coaching_principles_coaching_principles_get**
> PaginatedResponseCoachingPrinciple get_coaching_principles_coaching_principles_get(skip=skip, limit=limit)

Get Coaching Principles

Get a paginated list of Ted Lasso's core coaching principles and philosophy.

### Example

* Bearer Authentication (HTTPBearer):

```python
import openapi_client
from openapi_client.models.paginated_response_coaching_principle import PaginatedResponseCoachingPrinciple
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
    api_instance = openapi_client.InteractiveApi(api_client)
    skip = 0 # int | Number of items to skip (offset) (optional) (default to 0)
    limit = 20 # int | Maximum number of items to return (max: 100) (optional) (default to 20)

    try:
        # Get Coaching Principles
        api_response = api_instance.get_coaching_principles_coaching_principles_get(skip=skip, limit=limit)
        print("The response of InteractiveApi->get_coaching_principles_coaching_principles_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InteractiveApi->get_coaching_principles_coaching_principles_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **skip** | **int**| Number of items to skip (offset) | [optional] [default to 0]
 **limit** | **int**| Maximum number of items to return (max: 100) | [optional] [default to 20]

### Return type

[**PaginatedResponseCoachingPrinciple**](PaginatedResponseCoachingPrinciple.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Paginated list of coaching principles |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_fresh_biscuit_biscuits_fresh_get**
> Biscuit get_fresh_biscuit_biscuits_fresh_get()

Get a Fresh Biscuit

Get a single fresh biscuit with a personalized message from Ted.

### Example

* Bearer Authentication (HTTPBearer):

```python
import openapi_client
from openapi_client.models.biscuit import Biscuit
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
    api_instance = openapi_client.InteractiveApi(api_client)

    try:
        # Get a Fresh Biscuit
        api_response = api_instance.get_fresh_biscuit_biscuits_fresh_get()
        print("The response of InteractiveApi->get_fresh_biscuit_biscuits_fresh_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InteractiveApi->get_fresh_biscuit_biscuits_fresh_get: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**Biscuit**](Biscuit.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | A fresh biscuit from Ted&#39;s kitchen |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_random_principle_coaching_principles_random_get**
> CoachingPrinciple get_random_principle_coaching_principles_random_get()

Get a Random Coaching Principle

Get a random coaching principle to inspire your day.

### Example

* Bearer Authentication (HTTPBearer):

```python
import openapi_client
from openapi_client.models.coaching_principle import CoachingPrinciple
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
    api_instance = openapi_client.InteractiveApi(api_client)

    try:
        # Get a Random Coaching Principle
        api_response = api_instance.get_random_principle_coaching_principles_random_get()
        print("The response of InteractiveApi->get_random_principle_coaching_principles_random_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InteractiveApi->get_random_principle_coaching_principles_random_get: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**CoachingPrinciple**](CoachingPrinciple.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | A random coaching principle |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **press_conference_press_post**
> PressConferenceResponse press_conference_press_post(press_conference_request)

Press Conference Simulator

Get Ted's response to press conference questions.

### Example

* Bearer Authentication (HTTPBearer):

```python
import openapi_client
from openapi_client.models.press_conference_request import PressConferenceRequest
from openapi_client.models.press_conference_response import PressConferenceResponse
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
    api_instance = openapi_client.InteractiveApi(api_client)
    press_conference_request = openapi_client.PressConferenceRequest() # PressConferenceRequest | 

    try:
        # Press Conference Simulator
        api_response = api_instance.press_conference_press_post(press_conference_request)
        print("The response of InteractiveApi->press_conference_press_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InteractiveApi->press_conference_press_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **press_conference_request** | [**PressConferenceRequest**](PressConferenceRequest.md)|  | 

### Return type

[**PressConferenceResponse**](PressConferenceResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Press conference response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **reframe_thought_reframe_post**
> ReframeResponse reframe_thought_reframe_post(reframe_request)

Reframe Negative Thoughts

Transform negative thoughts into positive perspectives with Ted's help.

### Example

* Bearer Authentication (HTTPBearer):

```python
import openapi_client
from openapi_client.models.reframe_request import ReframeRequest
from openapi_client.models.reframe_response import ReframeResponse
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
    api_instance = openapi_client.InteractiveApi(api_client)
    reframe_request = openapi_client.ReframeRequest() # ReframeRequest | 

    try:
        # Reframe Negative Thoughts
        api_response = api_instance.reframe_thought_reframe_post(reframe_request)
        print("The response of InteractiveApi->reframe_thought_reframe_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InteractiveApi->reframe_thought_reframe_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **reframe_request** | [**ReframeRequest**](ReframeRequest.md)|  | 

### Return type

[**ReframeResponse**](ReframeResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Reframed perspective |  -  |
**422** | Validation Error |  -  |
**429** | Too much negativity |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **resolve_conflict_conflicts_resolve_post**
> ConflictResolution resolve_conflict_conflicts_resolve_post(conflict_request)

Resolve Conflicts

Get Ted Lasso-style advice for resolving conflicts.

### Example

* Bearer Authentication (HTTPBearer):

```python
import openapi_client
from openapi_client.models.conflict_request import ConflictRequest
from openapi_client.models.conflict_resolution import ConflictResolution
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
    api_instance = openapi_client.InteractiveApi(api_client)
    conflict_request = openapi_client.ConflictRequest() # ConflictRequest | 

    try:
        # Resolve Conflicts
        api_response = api_instance.resolve_conflict_conflicts_resolve_post(conflict_request)
        print("The response of InteractiveApi->resolve_conflict_conflicts_resolve_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InteractiveApi->resolve_conflict_conflicts_resolve_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **conflict_request** | [**ConflictRequest**](ConflictRequest.md)|  | 

### Return type

[**ConflictResolution**](ConflictResolution.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Conflict resolution guidance |  -  |
**403** | Too judgmental |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

