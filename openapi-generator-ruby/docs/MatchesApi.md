# OpenapiClient::MatchesApi

All URIs are relative to *https://believe.cjav.dev*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_match_matches_post**](MatchesApi.md#create_match_matches_post) | **POST** /matches | Create a new match |
| [**delete_match_matches_match_id_delete**](MatchesApi.md#delete_match_matches_match_id_delete) | **DELETE** /matches/{match_id} | Delete a match |
| [**get_match_lesson_matches_match_id_lesson_get**](MatchesApi.md#get_match_lesson_matches_match_id_lesson_get) | **GET** /matches/{match_id}/lesson | Get match lesson |
| [**get_match_matches_match_id_get**](MatchesApi.md#get_match_matches_match_id_get) | **GET** /matches/{match_id} | Get a match by ID |
| [**get_turning_points_matches_match_id_turning_points_get**](MatchesApi.md#get_turning_points_matches_match_id_turning_points_get) | **GET** /matches/{match_id}/turning-points | Get match turning points |
| [**list_matches_matches_get**](MatchesApi.md#list_matches_matches_get) | **GET** /matches | List all matches |
| [**update_match_matches_match_id_patch**](MatchesApi.md#update_match_matches_match_id_patch) | **PATCH** /matches/{match_id} | Update a match |


## create_match_matches_post

> <Match> create_match_matches_post(match_create)

Create a new match

Schedule a new match.

### Examples

```ruby
require 'time'
require 'openapi_client'
# setup authorization
OpenapiClient.configure do |config|
  # Configure Bearer authorization: HTTPBearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = OpenapiClient::MatchesApi.new
match_create = OpenapiClient::MatchCreate.new({away_team_id: 'manchester-city', date: Time.now, home_team_id: 'afc-richmond', match_type: OpenapiClient::MatchType::LEAGUE}) # MatchCreate | 

begin
  # Create a new match
  result = api_instance.create_match_matches_post(match_create)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling MatchesApi->create_match_matches_post: #{e}"
end
```

#### Using the create_match_matches_post_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Match>, Integer, Hash)> create_match_matches_post_with_http_info(match_create)

```ruby
begin
  # Create a new match
  data, status_code, headers = api_instance.create_match_matches_post_with_http_info(match_create)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Match>
rescue OpenapiClient::ApiError => e
  puts "Error when calling MatchesApi->create_match_matches_post_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **match_create** | [**MatchCreate**](MatchCreate.md) |  |  |

### Return type

[**Match**](Match.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## delete_match_matches_match_id_delete

> delete_match_matches_match_id_delete(match_id)

Delete a match

Remove a match from the database.

### Examples

```ruby
require 'time'
require 'openapi_client'
# setup authorization
OpenapiClient.configure do |config|
  # Configure Bearer authorization: HTTPBearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = OpenapiClient::MatchesApi.new
match_id = 'match_id_example' # String | 

begin
  # Delete a match
  api_instance.delete_match_matches_match_id_delete(match_id)
rescue OpenapiClient::ApiError => e
  puts "Error when calling MatchesApi->delete_match_matches_match_id_delete: #{e}"
end
```

#### Using the delete_match_matches_match_id_delete_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_match_matches_match_id_delete_with_http_info(match_id)

```ruby
begin
  # Delete a match
  data, status_code, headers = api_instance.delete_match_matches_match_id_delete_with_http_info(match_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling MatchesApi->delete_match_matches_match_id_delete_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **match_id** | **String** |  |  |

### Return type

nil (empty response body)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## get_match_lesson_matches_match_id_lesson_get

> Hash&lt;String, Object&gt; get_match_lesson_matches_match_id_lesson_get(match_id)

Get match lesson

Get the life lesson learned from a specific match.

### Examples

```ruby
require 'time'
require 'openapi_client'
# setup authorization
OpenapiClient.configure do |config|
  # Configure Bearer authorization: HTTPBearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = OpenapiClient::MatchesApi.new
match_id = 'match_id_example' # String | 

begin
  # Get match lesson
  result = api_instance.get_match_lesson_matches_match_id_lesson_get(match_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling MatchesApi->get_match_lesson_matches_match_id_lesson_get: #{e}"
end
```

#### Using the get_match_lesson_matches_match_id_lesson_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Hash&lt;String, Object&gt;, Integer, Hash)> get_match_lesson_matches_match_id_lesson_get_with_http_info(match_id)

```ruby
begin
  # Get match lesson
  data, status_code, headers = api_instance.get_match_lesson_matches_match_id_lesson_get_with_http_info(match_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Hash&lt;String, Object&gt;
rescue OpenapiClient::ApiError => e
  puts "Error when calling MatchesApi->get_match_lesson_matches_match_id_lesson_get_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **match_id** | **String** |  |  |

### Return type

**Hash&lt;String, Object&gt;**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## get_match_matches_match_id_get

> <Match> get_match_matches_match_id_get(match_id)

Get a match by ID

Retrieve detailed information about a specific match.

### Examples

```ruby
require 'time'
require 'openapi_client'
# setup authorization
OpenapiClient.configure do |config|
  # Configure Bearer authorization: HTTPBearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = OpenapiClient::MatchesApi.new
match_id = 'match_id_example' # String | 

begin
  # Get a match by ID
  result = api_instance.get_match_matches_match_id_get(match_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling MatchesApi->get_match_matches_match_id_get: #{e}"
end
```

#### Using the get_match_matches_match_id_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Match>, Integer, Hash)> get_match_matches_match_id_get_with_http_info(match_id)

```ruby
begin
  # Get a match by ID
  data, status_code, headers = api_instance.get_match_matches_match_id_get_with_http_info(match_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Match>
rescue OpenapiClient::ApiError => e
  puts "Error when calling MatchesApi->get_match_matches_match_id_get_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **match_id** | **String** |  |  |

### Return type

[**Match**](Match.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## get_turning_points_matches_match_id_turning_points_get

> Array&lt;Hash&lt;String, Object&gt;&gt; get_turning_points_matches_match_id_turning_points_get(match_id)

Get match turning points

Get all turning points from a specific match.

### Examples

```ruby
require 'time'
require 'openapi_client'
# setup authorization
OpenapiClient.configure do |config|
  # Configure Bearer authorization: HTTPBearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = OpenapiClient::MatchesApi.new
match_id = 'match_id_example' # String | 

begin
  # Get match turning points
  result = api_instance.get_turning_points_matches_match_id_turning_points_get(match_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling MatchesApi->get_turning_points_matches_match_id_turning_points_get: #{e}"
end
```

#### Using the get_turning_points_matches_match_id_turning_points_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Array&lt;Hash&lt;String, Object&gt;&gt;, Integer, Hash)> get_turning_points_matches_match_id_turning_points_get_with_http_info(match_id)

```ruby
begin
  # Get match turning points
  data, status_code, headers = api_instance.get_turning_points_matches_match_id_turning_points_get_with_http_info(match_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Array&lt;Hash&lt;String, Object&gt;&gt;
rescue OpenapiClient::ApiError => e
  puts "Error when calling MatchesApi->get_turning_points_matches_match_id_turning_points_get_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **match_id** | **String** |  |  |

### Return type

**Array&lt;Hash&lt;String, Object&gt;&gt;**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## list_matches_matches_get

> <PaginatedResponseMatch> list_matches_matches_get(opts)

List all matches

Get a paginated list of all matches with optional filtering.

### Examples

```ruby
require 'time'
require 'openapi_client'
# setup authorization
OpenapiClient.configure do |config|
  # Configure Bearer authorization: HTTPBearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = OpenapiClient::MatchesApi.new
opts = {
  team_id: 'team_id_example', # String | Filter by team (home or away)
  result: OpenapiClient::MatchResult::WIN, # MatchResult | Filter by result
  match_type: OpenapiClient::MatchType::LEAGUE, # MatchType | Filter by match type
  skip: 56, # Integer | Number of items to skip (offset)
  limit: 56 # Integer | Maximum number of items to return (max: 100)
}

begin
  # List all matches
  result = api_instance.list_matches_matches_get(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling MatchesApi->list_matches_matches_get: #{e}"
end
```

#### Using the list_matches_matches_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<PaginatedResponseMatch>, Integer, Hash)> list_matches_matches_get_with_http_info(opts)

```ruby
begin
  # List all matches
  data, status_code, headers = api_instance.list_matches_matches_get_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <PaginatedResponseMatch>
rescue OpenapiClient::ApiError => e
  puts "Error when calling MatchesApi->list_matches_matches_get_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **team_id** | **String** | Filter by team (home or away) | [optional] |
| **result** | [**MatchResult**](.md) | Filter by result | [optional] |
| **match_type** | [**MatchType**](.md) | Filter by match type | [optional] |
| **skip** | **Integer** | Number of items to skip (offset) | [optional][default to 0] |
| **limit** | **Integer** | Maximum number of items to return (max: 100) | [optional][default to 20] |

### Return type

[**PaginatedResponseMatch**](PaginatedResponseMatch.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## update_match_matches_match_id_patch

> <Match> update_match_matches_match_id_patch(match_id, match_update)

Update a match

Update specific fields of an existing match (e.g., update score).

### Examples

```ruby
require 'time'
require 'openapi_client'
# setup authorization
OpenapiClient.configure do |config|
  # Configure Bearer authorization: HTTPBearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = OpenapiClient::MatchesApi.new
match_id = 'match_id_example' # String | 
match_update = OpenapiClient::MatchUpdate.new # MatchUpdate | 

begin
  # Update a match
  result = api_instance.update_match_matches_match_id_patch(match_id, match_update)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling MatchesApi->update_match_matches_match_id_patch: #{e}"
end
```

#### Using the update_match_matches_match_id_patch_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Match>, Integer, Hash)> update_match_matches_match_id_patch_with_http_info(match_id, match_update)

```ruby
begin
  # Update a match
  data, status_code, headers = api_instance.update_match_matches_match_id_patch_with_http_info(match_id, match_update)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Match>
rescue OpenapiClient::ApiError => e
  puts "Error when calling MatchesApi->update_match_matches_match_id_patch_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **match_id** | **String** |  |  |
| **match_update** | [**MatchUpdate**](MatchUpdate.md) |  |  |

### Return type

[**Match**](Match.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

