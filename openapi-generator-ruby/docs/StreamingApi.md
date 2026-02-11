# OpenapiClient::StreamingApi

All URIs are relative to *https://believe.cjav.dev*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**get_pep_talk_pep_talk_get**](StreamingApi.md#get_pep_talk_pep_talk_get) | **GET** /pep-talk | Get a Pep Talk |
| [**stream_match_commentary_matches_match_id_commentary_stream_post**](StreamingApi.md#stream_match_commentary_matches_match_id_commentary_stream_post) | **POST** /matches/{match_id}/commentary/stream | Stream Match Commentary |
| [**test_stream_stream_test_get**](StreamingApi.md#test_stream_stream_test_get) | **GET** /stream/test | Test SSE Connection |


## get_pep_talk_pep_talk_get

> <PepTalkResponse> get_pep_talk_pep_talk_get(opts)

Get a Pep Talk

Get a motivational pep talk from Ted Lasso himself. By default returns the complete pep talk. Add `?stream=true` to get Server-Sent Events (SSE) streaming the pep talk chunk by chunk.

### Examples

```ruby
require 'time'
require 'openapi_client'
# setup authorization
OpenapiClient.configure do |config|
  # Configure Bearer authorization: HTTPBearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = OpenapiClient::StreamingApi.new
opts = {
  stream: true # Boolean | If true, returns SSE stream instead of full response
}

begin
  # Get a Pep Talk
  result = api_instance.get_pep_talk_pep_talk_get(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling StreamingApi->get_pep_talk_pep_talk_get: #{e}"
end
```

#### Using the get_pep_talk_pep_talk_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<PepTalkResponse>, Integer, Hash)> get_pep_talk_pep_talk_get_with_http_info(opts)

```ruby
begin
  # Get a Pep Talk
  data, status_code, headers = api_instance.get_pep_talk_pep_talk_get_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <PepTalkResponse>
rescue OpenapiClient::ApiError => e
  puts "Error when calling StreamingApi->get_pep_talk_pep_talk_get_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **stream** | **Boolean** | If true, returns SSE stream instead of full response | [optional][default to false] |

### Return type

[**PepTalkResponse**](PepTalkResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, text/event-stream


## stream_match_commentary_matches_match_id_commentary_stream_post

> Object stream_match_commentary_matches_match_id_commentary_stream_post(match_id)

Stream Match Commentary

Stream live match commentary for a specific match. Uses Server-Sent Events (SSE) to stream commentary events in real-time.

### Examples

```ruby
require 'time'
require 'openapi_client'
# setup authorization
OpenapiClient.configure do |config|
  # Configure Bearer authorization: HTTPBearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = OpenapiClient::StreamingApi.new
match_id = 'match_id_example' # String | 

begin
  # Stream Match Commentary
  result = api_instance.stream_match_commentary_matches_match_id_commentary_stream_post(match_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling StreamingApi->stream_match_commentary_matches_match_id_commentary_stream_post: #{e}"
end
```

#### Using the stream_match_commentary_matches_match_id_commentary_stream_post_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> stream_match_commentary_matches_match_id_commentary_stream_post_with_http_info(match_id)

```ruby
begin
  # Stream Match Commentary
  data, status_code, headers = api_instance.stream_match_commentary_matches_match_id_commentary_stream_post_with_http_info(match_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue OpenapiClient::ApiError => e
  puts "Error when calling StreamingApi->stream_match_commentary_matches_match_id_commentary_stream_post_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **match_id** | **String** |  |  |

### Return type

**Object**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, text/event-stream


## test_stream_stream_test_get

> Object test_stream_stream_test_get

Test SSE Connection

A simple SSE test endpoint that streams numbers 1-5.

### Examples

```ruby
require 'time'
require 'openapi_client'
# setup authorization
OpenapiClient.configure do |config|
  # Configure Bearer authorization: HTTPBearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = OpenapiClient::StreamingApi.new

begin
  # Test SSE Connection
  result = api_instance.test_stream_stream_test_get
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling StreamingApi->test_stream_stream_test_get: #{e}"
end
```

#### Using the test_stream_stream_test_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> test_stream_stream_test_get_with_http_info

```ruby
begin
  # Test SSE Connection
  data, status_code, headers = api_instance.test_stream_stream_test_get_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue OpenapiClient::ApiError => e
  puts "Error when calling StreamingApi->test_stream_stream_test_get_with_http_info: #{e}"
end
```

### Parameters

This endpoint does not need any parameter.

### Return type

**Object**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, text/event-stream

