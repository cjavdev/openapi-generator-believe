# OpenapiClient::EpisodesApi

All URIs are relative to *https://believe.cjav.dev*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_episode_episodes_post**](EpisodesApi.md#create_episode_episodes_post) | **POST** /episodes | Create a new episode |
| [**delete_episode_episodes_episode_id_delete**](EpisodesApi.md#delete_episode_episodes_episode_id_delete) | **DELETE** /episodes/{episode_id} | Delete an episode |
| [**get_episode_episodes_episode_id_get**](EpisodesApi.md#get_episode_episodes_episode_id_get) | **GET** /episodes/{episode_id} | Get an episode by ID |
| [**get_episode_wisdom_episodes_episode_id_wisdom_get**](EpisodesApi.md#get_episode_wisdom_episodes_episode_id_wisdom_get) | **GET** /episodes/{episode_id}/wisdom | Get episode wisdom |
| [**get_season_episodes_episodes_seasons_season_number_get**](EpisodesApi.md#get_season_episodes_episodes_seasons_season_number_get) | **GET** /episodes/seasons/{season_number} | Get all episodes from a season |
| [**list_episodes_episodes_get**](EpisodesApi.md#list_episodes_episodes_get) | **GET** /episodes | List all episodes |
| [**update_episode_episodes_episode_id_patch**](EpisodesApi.md#update_episode_episodes_episode_id_patch) | **PATCH** /episodes/{episode_id} | Update an episode |


## create_episode_episodes_post

> <Episode> create_episode_episodes_post(episode_create)

Create a new episode

Add a new episode to the series.

### Examples

```ruby
require 'time'
require 'openapi_client'
# setup authorization
OpenapiClient.configure do |config|
  # Configure Bearer authorization: HTTPBearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = OpenapiClient::EpisodesApi.new
episode_create = OpenapiClient::EpisodeCreate.new({air_date: Date.parse('2020-08-14'), character_focus: [ted-lasso,  rebecca-welton], director: 'director_example', episode_number: 37, main_theme: 'Taking chances and believing in yourself', runtime_minutes: 37, season: 37, synopsis: 'American football coach Ted Lasso is hired to manage AFC Richmond, a struggling English Premier League team.', ted_wisdom: 'Taking on a challenge is a lot like riding a horse. If you're comfortable while you're doing it, you're probably doing it wrong.', title: 'Pilot', writer: 'writer_example'}) # EpisodeCreate | 

begin
  # Create a new episode
  result = api_instance.create_episode_episodes_post(episode_create)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EpisodesApi->create_episode_episodes_post: #{e}"
end
```

#### Using the create_episode_episodes_post_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Episode>, Integer, Hash)> create_episode_episodes_post_with_http_info(episode_create)

```ruby
begin
  # Create a new episode
  data, status_code, headers = api_instance.create_episode_episodes_post_with_http_info(episode_create)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Episode>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EpisodesApi->create_episode_episodes_post_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **episode_create** | [**EpisodeCreate**](EpisodeCreate.md) |  |  |

### Return type

[**Episode**](Episode.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## delete_episode_episodes_episode_id_delete

> delete_episode_episodes_episode_id_delete(episode_id)

Delete an episode

Remove an episode from the database.

### Examples

```ruby
require 'time'
require 'openapi_client'
# setup authorization
OpenapiClient.configure do |config|
  # Configure Bearer authorization: HTTPBearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = OpenapiClient::EpisodesApi.new
episode_id = 'episode_id_example' # String | 

begin
  # Delete an episode
  api_instance.delete_episode_episodes_episode_id_delete(episode_id)
rescue OpenapiClient::ApiError => e
  puts "Error when calling EpisodesApi->delete_episode_episodes_episode_id_delete: #{e}"
end
```

#### Using the delete_episode_episodes_episode_id_delete_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_episode_episodes_episode_id_delete_with_http_info(episode_id)

```ruby
begin
  # Delete an episode
  data, status_code, headers = api_instance.delete_episode_episodes_episode_id_delete_with_http_info(episode_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling EpisodesApi->delete_episode_episodes_episode_id_delete_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **episode_id** | **String** |  |  |

### Return type

nil (empty response body)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## get_episode_episodes_episode_id_get

> <Episode> get_episode_episodes_episode_id_get(episode_id)

Get an episode by ID

Retrieve detailed information about a specific episode.

### Examples

```ruby
require 'time'
require 'openapi_client'
# setup authorization
OpenapiClient.configure do |config|
  # Configure Bearer authorization: HTTPBearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = OpenapiClient::EpisodesApi.new
episode_id = 'episode_id_example' # String | 

begin
  # Get an episode by ID
  result = api_instance.get_episode_episodes_episode_id_get(episode_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EpisodesApi->get_episode_episodes_episode_id_get: #{e}"
end
```

#### Using the get_episode_episodes_episode_id_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Episode>, Integer, Hash)> get_episode_episodes_episode_id_get_with_http_info(episode_id)

```ruby
begin
  # Get an episode by ID
  data, status_code, headers = api_instance.get_episode_episodes_episode_id_get_with_http_info(episode_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Episode>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EpisodesApi->get_episode_episodes_episode_id_get_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **episode_id** | **String** |  |  |

### Return type

[**Episode**](Episode.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## get_episode_wisdom_episodes_episode_id_wisdom_get

> Hash&lt;String, Object&gt; get_episode_wisdom_episodes_episode_id_wisdom_get(episode_id)

Get episode wisdom

Get Ted's wisdom and memorable moments from a specific episode.

### Examples

```ruby
require 'time'
require 'openapi_client'
# setup authorization
OpenapiClient.configure do |config|
  # Configure Bearer authorization: HTTPBearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = OpenapiClient::EpisodesApi.new
episode_id = 'episode_id_example' # String | 

begin
  # Get episode wisdom
  result = api_instance.get_episode_wisdom_episodes_episode_id_wisdom_get(episode_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EpisodesApi->get_episode_wisdom_episodes_episode_id_wisdom_get: #{e}"
end
```

#### Using the get_episode_wisdom_episodes_episode_id_wisdom_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Hash&lt;String, Object&gt;, Integer, Hash)> get_episode_wisdom_episodes_episode_id_wisdom_get_with_http_info(episode_id)

```ruby
begin
  # Get episode wisdom
  data, status_code, headers = api_instance.get_episode_wisdom_episodes_episode_id_wisdom_get_with_http_info(episode_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Hash&lt;String, Object&gt;
rescue OpenapiClient::ApiError => e
  puts "Error when calling EpisodesApi->get_episode_wisdom_episodes_episode_id_wisdom_get_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **episode_id** | **String** |  |  |

### Return type

**Hash&lt;String, Object&gt;**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## get_season_episodes_episodes_seasons_season_number_get

> <PaginatedResponseEpisode> get_season_episodes_episodes_seasons_season_number_get(season_number, opts)

Get all episodes from a season

Get a paginated list of episodes from a specific season.

### Examples

```ruby
require 'time'
require 'openapi_client'
# setup authorization
OpenapiClient.configure do |config|
  # Configure Bearer authorization: HTTPBearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = OpenapiClient::EpisodesApi.new
season_number = 56 # Integer | 
opts = {
  skip: 56, # Integer | Number of items to skip (offset)
  limit: 56 # Integer | Maximum number of items to return (max: 100)
}

begin
  # Get all episodes from a season
  result = api_instance.get_season_episodes_episodes_seasons_season_number_get(season_number, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EpisodesApi->get_season_episodes_episodes_seasons_season_number_get: #{e}"
end
```

#### Using the get_season_episodes_episodes_seasons_season_number_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<PaginatedResponseEpisode>, Integer, Hash)> get_season_episodes_episodes_seasons_season_number_get_with_http_info(season_number, opts)

```ruby
begin
  # Get all episodes from a season
  data, status_code, headers = api_instance.get_season_episodes_episodes_seasons_season_number_get_with_http_info(season_number, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <PaginatedResponseEpisode>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EpisodesApi->get_season_episodes_episodes_seasons_season_number_get_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **season_number** | **Integer** |  |  |
| **skip** | **Integer** | Number of items to skip (offset) | [optional][default to 0] |
| **limit** | **Integer** | Maximum number of items to return (max: 100) | [optional][default to 20] |

### Return type

[**PaginatedResponseEpisode**](PaginatedResponseEpisode.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## list_episodes_episodes_get

> <PaginatedResponseEpisode> list_episodes_episodes_get(opts)

List all episodes

Get a paginated list of all Ted Lasso episodes with optional filtering by season.

### Examples

```ruby
require 'time'
require 'openapi_client'
# setup authorization
OpenapiClient.configure do |config|
  # Configure Bearer authorization: HTTPBearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = OpenapiClient::EpisodesApi.new
opts = {
  season: 56, # Integer | Filter by season
  character_focus: 'character_focus_example', # String | Filter by character focus (character ID)
  skip: 56, # Integer | Number of items to skip (offset)
  limit: 56 # Integer | Maximum number of items to return (max: 100)
}

begin
  # List all episodes
  result = api_instance.list_episodes_episodes_get(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EpisodesApi->list_episodes_episodes_get: #{e}"
end
```

#### Using the list_episodes_episodes_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<PaginatedResponseEpisode>, Integer, Hash)> list_episodes_episodes_get_with_http_info(opts)

```ruby
begin
  # List all episodes
  data, status_code, headers = api_instance.list_episodes_episodes_get_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <PaginatedResponseEpisode>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EpisodesApi->list_episodes_episodes_get_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **season** | **Integer** | Filter by season | [optional] |
| **character_focus** | **String** | Filter by character focus (character ID) | [optional] |
| **skip** | **Integer** | Number of items to skip (offset) | [optional][default to 0] |
| **limit** | **Integer** | Maximum number of items to return (max: 100) | [optional][default to 20] |

### Return type

[**PaginatedResponseEpisode**](PaginatedResponseEpisode.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## update_episode_episodes_episode_id_patch

> <Episode> update_episode_episodes_episode_id_patch(episode_id, episode_update)

Update an episode

Update specific fields of an existing episode.

### Examples

```ruby
require 'time'
require 'openapi_client'
# setup authorization
OpenapiClient.configure do |config|
  # Configure Bearer authorization: HTTPBearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = OpenapiClient::EpisodesApi.new
episode_id = 'episode_id_example' # String | 
episode_update = OpenapiClient::EpisodeUpdate.new # EpisodeUpdate | 

begin
  # Update an episode
  result = api_instance.update_episode_episodes_episode_id_patch(episode_id, episode_update)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling EpisodesApi->update_episode_episodes_episode_id_patch: #{e}"
end
```

#### Using the update_episode_episodes_episode_id_patch_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Episode>, Integer, Hash)> update_episode_episodes_episode_id_patch_with_http_info(episode_id, episode_update)

```ruby
begin
  # Update an episode
  data, status_code, headers = api_instance.update_episode_episodes_episode_id_patch_with_http_info(episode_id, episode_update)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Episode>
rescue OpenapiClient::ApiError => e
  puts "Error when calling EpisodesApi->update_episode_episodes_episode_id_patch_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **episode_id** | **String** |  |  |
| **episode_update** | [**EpisodeUpdate**](EpisodeUpdate.md) |  |  |

### Return type

[**Episode**](Episode.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

