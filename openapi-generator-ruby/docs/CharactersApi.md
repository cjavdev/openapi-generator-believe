# OpenapiClient::CharactersApi

All URIs are relative to *https://believe.cjav.dev*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_character_characters_post**](CharactersApi.md#create_character_characters_post) | **POST** /characters | Create a new character |
| [**delete_character_characters_character_id_delete**](CharactersApi.md#delete_character_characters_character_id_delete) | **DELETE** /characters/{character_id} | Delete a character |
| [**get_character_characters_character_id_get**](CharactersApi.md#get_character_characters_character_id_get) | **GET** /characters/{character_id} | Get a character by ID |
| [**get_character_quotes_characters_character_id_quotes_get**](CharactersApi.md#get_character_quotes_characters_character_id_quotes_get) | **GET** /characters/{character_id}/quotes | Get character&#39;s signature quotes |
| [**list_characters_characters_get**](CharactersApi.md#list_characters_characters_get) | **GET** /characters | List all characters |
| [**update_character_characters_character_id_patch**](CharactersApi.md#update_character_characters_character_id_patch) | **PATCH** /characters/{character_id} | Update a character |


## create_character_characters_post

> <Character> create_character_characters_post(character_create)

Create a new character

Add a new character to the Ted Lasso universe.

### Examples

```ruby
require 'time'
require 'openapi_client'
# setup authorization
OpenapiClient.configure do |config|
  # Configure Bearer authorization: HTTPBearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = OpenapiClient::CharactersApi.new
character_create = OpenapiClient::CharacterCreate.new({background: 'Former American football coach from Kansas who moved to London to coach AFC Richmond', emotional_stats: OpenapiClient::EmotionalStats.new({curiosity: 99, empathy: 100, optimism: 95, resilience: 90, vulnerability: 80}), name: 'Ted Lasso', personality_traits: [optimistic,  kind,  folksy,  persistent], role: OpenapiClient::CharacterRole::COACH}) # CharacterCreate | 

begin
  # Create a new character
  result = api_instance.create_character_characters_post(character_create)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CharactersApi->create_character_characters_post: #{e}"
end
```

#### Using the create_character_characters_post_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Character>, Integer, Hash)> create_character_characters_post_with_http_info(character_create)

```ruby
begin
  # Create a new character
  data, status_code, headers = api_instance.create_character_characters_post_with_http_info(character_create)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Character>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CharactersApi->create_character_characters_post_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **character_create** | [**CharacterCreate**](CharacterCreate.md) |  |  |

### Return type

[**Character**](Character.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## delete_character_characters_character_id_delete

> delete_character_characters_character_id_delete(character_id)

Delete a character

Remove a character from the database.

### Examples

```ruby
require 'time'
require 'openapi_client'
# setup authorization
OpenapiClient.configure do |config|
  # Configure Bearer authorization: HTTPBearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = OpenapiClient::CharactersApi.new
character_id = 'character_id_example' # String | 

begin
  # Delete a character
  api_instance.delete_character_characters_character_id_delete(character_id)
rescue OpenapiClient::ApiError => e
  puts "Error when calling CharactersApi->delete_character_characters_character_id_delete: #{e}"
end
```

#### Using the delete_character_characters_character_id_delete_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_character_characters_character_id_delete_with_http_info(character_id)

```ruby
begin
  # Delete a character
  data, status_code, headers = api_instance.delete_character_characters_character_id_delete_with_http_info(character_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling CharactersApi->delete_character_characters_character_id_delete_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **character_id** | **String** |  |  |

### Return type

nil (empty response body)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## get_character_characters_character_id_get

> <Character> get_character_characters_character_id_get(character_id)

Get a character by ID

Retrieve detailed information about a specific character.

### Examples

```ruby
require 'time'
require 'openapi_client'
# setup authorization
OpenapiClient.configure do |config|
  # Configure Bearer authorization: HTTPBearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = OpenapiClient::CharactersApi.new
character_id = 'character_id_example' # String | 

begin
  # Get a character by ID
  result = api_instance.get_character_characters_character_id_get(character_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CharactersApi->get_character_characters_character_id_get: #{e}"
end
```

#### Using the get_character_characters_character_id_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Character>, Integer, Hash)> get_character_characters_character_id_get_with_http_info(character_id)

```ruby
begin
  # Get a character by ID
  data, status_code, headers = api_instance.get_character_characters_character_id_get_with_http_info(character_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Character>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CharactersApi->get_character_characters_character_id_get_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **character_id** | **String** |  |  |

### Return type

[**Character**](Character.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## get_character_quotes_characters_character_id_quotes_get

> Array&lt;String&gt; get_character_quotes_characters_character_id_quotes_get(character_id)

Get character's signature quotes

Get all signature quotes from a specific character.

### Examples

```ruby
require 'time'
require 'openapi_client'
# setup authorization
OpenapiClient.configure do |config|
  # Configure Bearer authorization: HTTPBearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = OpenapiClient::CharactersApi.new
character_id = 'character_id_example' # String | 

begin
  # Get character's signature quotes
  result = api_instance.get_character_quotes_characters_character_id_quotes_get(character_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CharactersApi->get_character_quotes_characters_character_id_quotes_get: #{e}"
end
```

#### Using the get_character_quotes_characters_character_id_quotes_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Array&lt;String&gt;, Integer, Hash)> get_character_quotes_characters_character_id_quotes_get_with_http_info(character_id)

```ruby
begin
  # Get character's signature quotes
  data, status_code, headers = api_instance.get_character_quotes_characters_character_id_quotes_get_with_http_info(character_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Array&lt;String&gt;
rescue OpenapiClient::ApiError => e
  puts "Error when calling CharactersApi->get_character_quotes_characters_character_id_quotes_get_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **character_id** | **String** |  |  |

### Return type

**Array&lt;String&gt;**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## list_characters_characters_get

> <PaginatedResponseCharacter> list_characters_characters_get(opts)

List all characters

Get a paginated list of Ted Lasso characters.

### Examples

```ruby
require 'time'
require 'openapi_client'
# setup authorization
OpenapiClient.configure do |config|
  # Configure Bearer authorization: HTTPBearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = OpenapiClient::CharactersApi.new
opts = {
  role: OpenapiClient::CharacterRole::COACH, # CharacterRole | Filter by role
  team_id: 'team_id_example', # String | Filter by team ID
  min_optimism: 56, # Integer | Minimum optimism score
  skip: 56, # Integer | Number of items to skip (offset)
  limit: 56 # Integer | Maximum number of items to return (max: 100)
}

begin
  # List all characters
  result = api_instance.list_characters_characters_get(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CharactersApi->list_characters_characters_get: #{e}"
end
```

#### Using the list_characters_characters_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<PaginatedResponseCharacter>, Integer, Hash)> list_characters_characters_get_with_http_info(opts)

```ruby
begin
  # List all characters
  data, status_code, headers = api_instance.list_characters_characters_get_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <PaginatedResponseCharacter>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CharactersApi->list_characters_characters_get_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **role** | [**CharacterRole**](.md) | Filter by role | [optional] |
| **team_id** | **String** | Filter by team ID | [optional] |
| **min_optimism** | **Integer** | Minimum optimism score | [optional] |
| **skip** | **Integer** | Number of items to skip (offset) | [optional][default to 0] |
| **limit** | **Integer** | Maximum number of items to return (max: 100) | [optional][default to 20] |

### Return type

[**PaginatedResponseCharacter**](PaginatedResponseCharacter.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## update_character_characters_character_id_patch

> <Character> update_character_characters_character_id_patch(character_id, character_update)

Update a character

Update specific fields of an existing character.

### Examples

```ruby
require 'time'
require 'openapi_client'
# setup authorization
OpenapiClient.configure do |config|
  # Configure Bearer authorization: HTTPBearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = OpenapiClient::CharactersApi.new
character_id = 'character_id_example' # String | 
character_update = OpenapiClient::CharacterUpdate.new # CharacterUpdate | 

begin
  # Update a character
  result = api_instance.update_character_characters_character_id_patch(character_id, character_update)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling CharactersApi->update_character_characters_character_id_patch: #{e}"
end
```

#### Using the update_character_characters_character_id_patch_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Character>, Integer, Hash)> update_character_characters_character_id_patch_with_http_info(character_id, character_update)

```ruby
begin
  # Update a character
  data, status_code, headers = api_instance.update_character_characters_character_id_patch_with_http_info(character_id, character_update)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Character>
rescue OpenapiClient::ApiError => e
  puts "Error when calling CharactersApi->update_character_characters_character_id_patch_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **character_id** | **String** |  |  |
| **character_update** | [**CharacterUpdate**](CharacterUpdate.md) |  |  |

### Return type

[**Character**](Character.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

