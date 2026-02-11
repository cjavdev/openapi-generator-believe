# openapi_client.StreamingApi

All URIs are relative to *https://believe.cjav.dev*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_pep_talk_pep_talk_get**](StreamingApi.md#get_pep_talk_pep_talk_get) | **GET** /pep-talk | Get a Pep Talk
[**stream_match_commentary_matches_match_id_commentary_stream_post**](StreamingApi.md#stream_match_commentary_matches_match_id_commentary_stream_post) | **POST** /matches/{match_id}/commentary/stream | Stream Match Commentary
[**test_stream_stream_test_get**](StreamingApi.md#test_stream_stream_test_get) | **GET** /stream/test | Test SSE Connection


# **get_pep_talk_pep_talk_get**
> PepTalkResponse get_pep_talk_pep_talk_get(stream=stream)

Get a Pep Talk

Get a motivational pep talk from Ted Lasso himself. By default returns the complete pep talk. Add `?stream=true` to get Server-Sent Events (SSE) streaming the pep talk chunk by chunk.

### Example

* Bearer Authentication (HTTPBearer):

```python
import openapi_client
from openapi_client.models.pep_talk_response import PepTalkResponse
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
    api_instance = openapi_client.StreamingApi(api_client)
    stream = False # bool | If true, returns SSE stream instead of full response (optional) (default to False)

    try:
        # Get a Pep Talk
        api_response = api_instance.get_pep_talk_pep_talk_get(stream=stream)
        print("The response of StreamingApi->get_pep_talk_pep_talk_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling StreamingApi->get_pep_talk_pep_talk_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **stream** | **bool**| If true, returns SSE stream instead of full response | [optional] [default to False]

### Return type

[**PepTalkResponse**](PepTalkResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/event-stream

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Pep talk response (JSON or SSE stream) |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **stream_match_commentary_matches_match_id_commentary_stream_post**
> object stream_match_commentary_matches_match_id_commentary_stream_post(match_id)

Stream Match Commentary

Stream live match commentary for a specific match. Uses Server-Sent Events (SSE) to stream commentary events in real-time.

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
    api_instance = openapi_client.StreamingApi(api_client)
    match_id = 'match_id_example' # str | 

    try:
        # Stream Match Commentary
        api_response = api_instance.stream_match_commentary_matches_match_id_commentary_stream_post(match_id)
        print("The response of StreamingApi->stream_match_commentary_matches_match_id_commentary_stream_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling StreamingApi->stream_match_commentary_matches_match_id_commentary_stream_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **match_id** | **str**|  | 

### Return type

**object**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/event-stream

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | SSE stream of match commentary events |  -  |
**404** | Match not found |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **test_stream_stream_test_get**
> object test_stream_stream_test_get()

Test SSE Connection

A simple SSE test endpoint that streams numbers 1-5.

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
    api_instance = openapi_client.StreamingApi(api_client)

    try:
        # Test SSE Connection
        api_response = api_instance.test_stream_stream_test_get()
        print("The response of StreamingApi->test_stream_stream_test_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling StreamingApi->test_stream_stream_test_get: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

**object**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/event-stream

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | SSE stream of test messages |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

