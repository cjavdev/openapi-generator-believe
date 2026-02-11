# OpenapiClient::QuotesApi

All URIs are relative to *https://believe.cjav.dev*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_quote_quotes_post**](QuotesApi.md#create_quote_quotes_post) | **POST** /quotes | Create a new quote |
| [**delete_quote_quotes_quote_id_delete**](QuotesApi.md#delete_quote_quotes_quote_id_delete) | **DELETE** /quotes/{quote_id} | Delete a quote |
| [**get_character_quotes_quotes_characters_character_id_get**](QuotesApi.md#get_character_quotes_quotes_characters_character_id_get) | **GET** /quotes/characters/{character_id} | Get all quotes by a character |
| [**get_quote_quotes_quote_id_get**](QuotesApi.md#get_quote_quotes_quote_id_get) | **GET** /quotes/{quote_id} | Get a quote by ID |
| [**get_quotes_by_theme_quotes_themes_theme_get**](QuotesApi.md#get_quotes_by_theme_quotes_themes_theme_get) | **GET** /quotes/themes/{theme} | Get quotes by theme |
| [**get_random_quote_quotes_random_get**](QuotesApi.md#get_random_quote_quotes_random_get) | **GET** /quotes/random | Get a random quote |
| [**list_quotes_quotes_get**](QuotesApi.md#list_quotes_quotes_get) | **GET** /quotes | List all quotes |
| [**update_quote_quotes_quote_id_patch**](QuotesApi.md#update_quote_quotes_quote_id_patch) | **PATCH** /quotes/{quote_id} | Update a quote |


## create_quote_quotes_post

> <Quote> create_quote_quotes_post(quote_create)

Create a new quote

Add a new memorable quote to the collection.

### Examples

```ruby
require 'time'
require 'openapi_client'
# setup authorization
OpenapiClient.configure do |config|
  # Configure Bearer authorization: HTTPBearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = OpenapiClient::QuotesApi.new
quote_create = OpenapiClient::QuoteCreate.new({character_id: 'ted-lasso', context: 'Ted playing darts against Rupert in the pub, explaining his philosophy', moment_type: OpenapiClient::QuoteMoment::HALFTIME_SPEECH, text: 'Be curious, not judgmental.', theme: OpenapiClient::QuoteTheme::BELIEF}) # QuoteCreate | 

begin
  # Create a new quote
  result = api_instance.create_quote_quotes_post(quote_create)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling QuotesApi->create_quote_quotes_post: #{e}"
end
```

#### Using the create_quote_quotes_post_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Quote>, Integer, Hash)> create_quote_quotes_post_with_http_info(quote_create)

```ruby
begin
  # Create a new quote
  data, status_code, headers = api_instance.create_quote_quotes_post_with_http_info(quote_create)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Quote>
rescue OpenapiClient::ApiError => e
  puts "Error when calling QuotesApi->create_quote_quotes_post_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **quote_create** | [**QuoteCreate**](QuoteCreate.md) |  |  |

### Return type

[**Quote**](Quote.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## delete_quote_quotes_quote_id_delete

> delete_quote_quotes_quote_id_delete(quote_id)

Delete a quote

Remove a quote from the collection.

### Examples

```ruby
require 'time'
require 'openapi_client'
# setup authorization
OpenapiClient.configure do |config|
  # Configure Bearer authorization: HTTPBearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = OpenapiClient::QuotesApi.new
quote_id = 'quote_id_example' # String | 

begin
  # Delete a quote
  api_instance.delete_quote_quotes_quote_id_delete(quote_id)
rescue OpenapiClient::ApiError => e
  puts "Error when calling QuotesApi->delete_quote_quotes_quote_id_delete: #{e}"
end
```

#### Using the delete_quote_quotes_quote_id_delete_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_quote_quotes_quote_id_delete_with_http_info(quote_id)

```ruby
begin
  # Delete a quote
  data, status_code, headers = api_instance.delete_quote_quotes_quote_id_delete_with_http_info(quote_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling QuotesApi->delete_quote_quotes_quote_id_delete_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **quote_id** | **String** |  |  |

### Return type

nil (empty response body)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## get_character_quotes_quotes_characters_character_id_get

> <PaginatedResponseQuote> get_character_quotes_quotes_characters_character_id_get(character_id, opts)

Get all quotes by a character

Get a paginated list of quotes from a specific character.

### Examples

```ruby
require 'time'
require 'openapi_client'
# setup authorization
OpenapiClient.configure do |config|
  # Configure Bearer authorization: HTTPBearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = OpenapiClient::QuotesApi.new
character_id = 'character_id_example' # String | 
opts = {
  skip: 56, # Integer | Number of items to skip (offset)
  limit: 56 # Integer | Maximum number of items to return (max: 100)
}

begin
  # Get all quotes by a character
  result = api_instance.get_character_quotes_quotes_characters_character_id_get(character_id, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling QuotesApi->get_character_quotes_quotes_characters_character_id_get: #{e}"
end
```

#### Using the get_character_quotes_quotes_characters_character_id_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<PaginatedResponseQuote>, Integer, Hash)> get_character_quotes_quotes_characters_character_id_get_with_http_info(character_id, opts)

```ruby
begin
  # Get all quotes by a character
  data, status_code, headers = api_instance.get_character_quotes_quotes_characters_character_id_get_with_http_info(character_id, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <PaginatedResponseQuote>
rescue OpenapiClient::ApiError => e
  puts "Error when calling QuotesApi->get_character_quotes_quotes_characters_character_id_get_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **character_id** | **String** |  |  |
| **skip** | **Integer** | Number of items to skip (offset) | [optional][default to 0] |
| **limit** | **Integer** | Maximum number of items to return (max: 100) | [optional][default to 20] |

### Return type

[**PaginatedResponseQuote**](PaginatedResponseQuote.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## get_quote_quotes_quote_id_get

> <Quote> get_quote_quotes_quote_id_get(quote_id)

Get a quote by ID

Retrieve a specific quote by its ID.

### Examples

```ruby
require 'time'
require 'openapi_client'
# setup authorization
OpenapiClient.configure do |config|
  # Configure Bearer authorization: HTTPBearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = OpenapiClient::QuotesApi.new
quote_id = 'quote_id_example' # String | 

begin
  # Get a quote by ID
  result = api_instance.get_quote_quotes_quote_id_get(quote_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling QuotesApi->get_quote_quotes_quote_id_get: #{e}"
end
```

#### Using the get_quote_quotes_quote_id_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Quote>, Integer, Hash)> get_quote_quotes_quote_id_get_with_http_info(quote_id)

```ruby
begin
  # Get a quote by ID
  data, status_code, headers = api_instance.get_quote_quotes_quote_id_get_with_http_info(quote_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Quote>
rescue OpenapiClient::ApiError => e
  puts "Error when calling QuotesApi->get_quote_quotes_quote_id_get_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **quote_id** | **String** |  |  |

### Return type

[**Quote**](Quote.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## get_quotes_by_theme_quotes_themes_theme_get

> <PaginatedResponseQuote> get_quotes_by_theme_quotes_themes_theme_get(theme, opts)

Get quotes by theme

Get a paginated list of quotes related to a specific theme.

### Examples

```ruby
require 'time'
require 'openapi_client'
# setup authorization
OpenapiClient.configure do |config|
  # Configure Bearer authorization: HTTPBearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = OpenapiClient::QuotesApi.new
theme = OpenapiClient::QuoteTheme::BELIEF # QuoteTheme | 
opts = {
  skip: 56, # Integer | Number of items to skip (offset)
  limit: 56 # Integer | Maximum number of items to return (max: 100)
}

begin
  # Get quotes by theme
  result = api_instance.get_quotes_by_theme_quotes_themes_theme_get(theme, opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling QuotesApi->get_quotes_by_theme_quotes_themes_theme_get: #{e}"
end
```

#### Using the get_quotes_by_theme_quotes_themes_theme_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<PaginatedResponseQuote>, Integer, Hash)> get_quotes_by_theme_quotes_themes_theme_get_with_http_info(theme, opts)

```ruby
begin
  # Get quotes by theme
  data, status_code, headers = api_instance.get_quotes_by_theme_quotes_themes_theme_get_with_http_info(theme, opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <PaginatedResponseQuote>
rescue OpenapiClient::ApiError => e
  puts "Error when calling QuotesApi->get_quotes_by_theme_quotes_themes_theme_get_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **theme** | [**QuoteTheme**](.md) |  |  |
| **skip** | **Integer** | Number of items to skip (offset) | [optional][default to 0] |
| **limit** | **Integer** | Maximum number of items to return (max: 100) | [optional][default to 20] |

### Return type

[**PaginatedResponseQuote**](PaginatedResponseQuote.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## get_random_quote_quotes_random_get

> <Quote> get_random_quote_quotes_random_get(opts)

Get a random quote

Get a random Ted Lasso quote, optionally filtered.

### Examples

```ruby
require 'time'
require 'openapi_client'
# setup authorization
OpenapiClient.configure do |config|
  # Configure Bearer authorization: HTTPBearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = OpenapiClient::QuotesApi.new
opts = {
  character_id: 'character_id_example', # String | Filter by character
  theme: OpenapiClient::QuoteTheme::BELIEF, # QuoteTheme | Filter by theme
  inspirational: true # Boolean | Filter inspirational quotes
}

begin
  # Get a random quote
  result = api_instance.get_random_quote_quotes_random_get(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling QuotesApi->get_random_quote_quotes_random_get: #{e}"
end
```

#### Using the get_random_quote_quotes_random_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Quote>, Integer, Hash)> get_random_quote_quotes_random_get_with_http_info(opts)

```ruby
begin
  # Get a random quote
  data, status_code, headers = api_instance.get_random_quote_quotes_random_get_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Quote>
rescue OpenapiClient::ApiError => e
  puts "Error when calling QuotesApi->get_random_quote_quotes_random_get_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **character_id** | **String** | Filter by character | [optional] |
| **theme** | [**QuoteTheme**](.md) | Filter by theme | [optional] |
| **inspirational** | **Boolean** | Filter inspirational quotes | [optional] |

### Return type

[**Quote**](Quote.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## list_quotes_quotes_get

> <PaginatedResponseQuote> list_quotes_quotes_get(opts)

List all quotes

Get a paginated list of all memorable Ted Lasso quotes with optional filtering.

### Examples

```ruby
require 'time'
require 'openapi_client'
# setup authorization
OpenapiClient.configure do |config|
  # Configure Bearer authorization: HTTPBearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = OpenapiClient::QuotesApi.new
opts = {
  character_id: 'character_id_example', # String | Filter by character
  theme: OpenapiClient::QuoteTheme::BELIEF, # QuoteTheme | Filter by theme
  moment_type: OpenapiClient::QuoteMoment::HALFTIME_SPEECH, # QuoteMoment | Filter by moment type
  inspirational: true, # Boolean | Filter inspirational quotes
  funny: true, # Boolean | Filter funny quotes
  skip: 56, # Integer | Number of items to skip (offset)
  limit: 56 # Integer | Maximum number of items to return (max: 100)
}

begin
  # List all quotes
  result = api_instance.list_quotes_quotes_get(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling QuotesApi->list_quotes_quotes_get: #{e}"
end
```

#### Using the list_quotes_quotes_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<PaginatedResponseQuote>, Integer, Hash)> list_quotes_quotes_get_with_http_info(opts)

```ruby
begin
  # List all quotes
  data, status_code, headers = api_instance.list_quotes_quotes_get_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <PaginatedResponseQuote>
rescue OpenapiClient::ApiError => e
  puts "Error when calling QuotesApi->list_quotes_quotes_get_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **character_id** | **String** | Filter by character | [optional] |
| **theme** | [**QuoteTheme**](.md) | Filter by theme | [optional] |
| **moment_type** | [**QuoteMoment**](.md) | Filter by moment type | [optional] |
| **inspirational** | **Boolean** | Filter inspirational quotes | [optional] |
| **funny** | **Boolean** | Filter funny quotes | [optional] |
| **skip** | **Integer** | Number of items to skip (offset) | [optional][default to 0] |
| **limit** | **Integer** | Maximum number of items to return (max: 100) | [optional][default to 20] |

### Return type

[**PaginatedResponseQuote**](PaginatedResponseQuote.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## update_quote_quotes_quote_id_patch

> <Quote> update_quote_quotes_quote_id_patch(quote_id, quote_update)

Update a quote

Update specific fields of an existing quote.

### Examples

```ruby
require 'time'
require 'openapi_client'
# setup authorization
OpenapiClient.configure do |config|
  # Configure Bearer authorization: HTTPBearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = OpenapiClient::QuotesApi.new
quote_id = 'quote_id_example' # String | 
quote_update = OpenapiClient::QuoteUpdate.new # QuoteUpdate | 

begin
  # Update a quote
  result = api_instance.update_quote_quotes_quote_id_patch(quote_id, quote_update)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling QuotesApi->update_quote_quotes_quote_id_patch: #{e}"
end
```

#### Using the update_quote_quotes_quote_id_patch_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Quote>, Integer, Hash)> update_quote_quotes_quote_id_patch_with_http_info(quote_id, quote_update)

```ruby
begin
  # Update a quote
  data, status_code, headers = api_instance.update_quote_quotes_quote_id_patch_with_http_info(quote_id, quote_update)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Quote>
rescue OpenapiClient::ApiError => e
  puts "Error when calling QuotesApi->update_quote_quotes_quote_id_patch_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **quote_id** | **String** |  |  |
| **quote_update** | [**QuoteUpdate**](QuoteUpdate.md) |  |  |

### Return type

[**Quote**](Quote.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

