# OpenapiClient::TeamsApi

All URIs are relative to *https://believe.cjav.dev*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_team_teams_post**](TeamsApi.md#create_team_teams_post) | **POST** /teams | Create a new team |
| [**delete_team_logo_teams_team_id_logo_file_id_delete**](TeamsApi.md#delete_team_logo_teams_team_id_logo_file_id_delete) | **DELETE** /teams/{team_id}/logo/{file_id} | Delete team logo |
| [**delete_team_teams_team_id_delete**](TeamsApi.md#delete_team_teams_team_id_delete) | **DELETE** /teams/{team_id} | Delete a team |
| [**download_team_logo_teams_team_id_logo_file_id_get**](TeamsApi.md#download_team_logo_teams_team_id_logo_file_id_get) | **GET** /teams/{team_id}/logo/{file_id} | Download team logo |
| [**get_team_culture_teams_team_id_culture_get**](TeamsApi.md#get_team_culture_teams_team_id_culture_get) | **GET** /teams/{team_id}/culture | Get team culture details |
| [**get_team_rivals_teams_team_id_rivals_get**](TeamsApi.md#get_team_rivals_teams_team_id_rivals_get) | **GET** /teams/{team_id}/rivals | Get team&#39;s rivals |
| [**get_team_teams_team_id_get**](TeamsApi.md#get_team_teams_team_id_get) | **GET** /teams/{team_id} | Get a team by ID |
| [**list_team_logos_teams_team_id_logos_get**](TeamsApi.md#list_team_logos_teams_team_id_logos_get) | **GET** /teams/{team_id}/logos | List team logos |
| [**list_teams_teams_get**](TeamsApi.md#list_teams_teams_get) | **GET** /teams | List all teams |
| [**update_team_teams_team_id_patch**](TeamsApi.md#update_team_teams_team_id_patch) | **PATCH** /teams/{team_id} | Update a team |
| [**upload_team_logo_teams_team_id_logo_post**](TeamsApi.md#upload_team_logo_teams_team_id_logo_post) | **POST** /teams/{team_id}/logo | Upload team logo |


## create_team_teams_post

> <Team> create_team_teams_post(team_create)

Create a new team

Add a new team to the league.

### Examples

```ruby
require 'time'
require 'openapi_client'
# setup authorization
OpenapiClient.configure do |config|
  # Configure Bearer authorization: HTTPBearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = OpenapiClient::TeamsApi.new
team_create = OpenapiClient::TeamCreate.new({culture_score: 85, founded_year: 1897, league: OpenapiClient::League::PREMIER_LEAGUE, name: 'AFC Richmond', stadium: 'Nelson Road', values: OpenapiClient::TeamValues.new({primary_value: 'Believe', secondary_values: [Family,  Resilience,  Joy], team_motto: 'Football is life!'})}) # TeamCreate | 

begin
  # Create a new team
  result = api_instance.create_team_teams_post(team_create)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamsApi->create_team_teams_post: #{e}"
end
```

#### Using the create_team_teams_post_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Team>, Integer, Hash)> create_team_teams_post_with_http_info(team_create)

```ruby
begin
  # Create a new team
  data, status_code, headers = api_instance.create_team_teams_post_with_http_info(team_create)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Team>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamsApi->create_team_teams_post_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **team_create** | [**TeamCreate**](TeamCreate.md) |  |  |

### Return type

[**Team**](Team.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## delete_team_logo_teams_team_id_logo_file_id_delete

> delete_team_logo_teams_team_id_logo_file_id_delete(team_id, file_id)

Delete team logo

Delete a team's logo.

### Examples

```ruby
require 'time'
require 'openapi_client'
# setup authorization
OpenapiClient.configure do |config|
  # Configure Bearer authorization: HTTPBearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = OpenapiClient::TeamsApi.new
team_id = 'team_id_example' # String | 
file_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Delete team logo
  api_instance.delete_team_logo_teams_team_id_logo_file_id_delete(team_id, file_id)
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamsApi->delete_team_logo_teams_team_id_logo_file_id_delete: #{e}"
end
```

#### Using the delete_team_logo_teams_team_id_logo_file_id_delete_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_team_logo_teams_team_id_logo_file_id_delete_with_http_info(team_id, file_id)

```ruby
begin
  # Delete team logo
  data, status_code, headers = api_instance.delete_team_logo_teams_team_id_logo_file_id_delete_with_http_info(team_id, file_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamsApi->delete_team_logo_teams_team_id_logo_file_id_delete_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **team_id** | **String** |  |  |
| **file_id** | **String** |  |  |

### Return type

nil (empty response body)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## delete_team_teams_team_id_delete

> delete_team_teams_team_id_delete(team_id)

Delete a team

Remove a team from the database (relegation to oblivion).

### Examples

```ruby
require 'time'
require 'openapi_client'
# setup authorization
OpenapiClient.configure do |config|
  # Configure Bearer authorization: HTTPBearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = OpenapiClient::TeamsApi.new
team_id = 'team_id_example' # String | 

begin
  # Delete a team
  api_instance.delete_team_teams_team_id_delete(team_id)
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamsApi->delete_team_teams_team_id_delete: #{e}"
end
```

#### Using the delete_team_teams_team_id_delete_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_team_teams_team_id_delete_with_http_info(team_id)

```ruby
begin
  # Delete a team
  data, status_code, headers = api_instance.delete_team_teams_team_id_delete_with_http_info(team_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamsApi->delete_team_teams_team_id_delete_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **team_id** | **String** |  |  |

### Return type

nil (empty response body)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## download_team_logo_teams_team_id_logo_file_id_get

> Object download_team_logo_teams_team_id_logo_file_id_get(team_id, file_id)

Download team logo

Download a team's logo by file ID.

### Examples

```ruby
require 'time'
require 'openapi_client'
# setup authorization
OpenapiClient.configure do |config|
  # Configure Bearer authorization: HTTPBearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = OpenapiClient::TeamsApi.new
team_id = 'team_id_example' # String | 
file_id = '38400000-8cf0-11bd-b23e-10b96e4ef00d' # String | 

begin
  # Download team logo
  result = api_instance.download_team_logo_teams_team_id_logo_file_id_get(team_id, file_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamsApi->download_team_logo_teams_team_id_logo_file_id_get: #{e}"
end
```

#### Using the download_team_logo_teams_team_id_logo_file_id_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Object, Integer, Hash)> download_team_logo_teams_team_id_logo_file_id_get_with_http_info(team_id, file_id)

```ruby
begin
  # Download team logo
  data, status_code, headers = api_instance.download_team_logo_teams_team_id_logo_file_id_get_with_http_info(team_id, file_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Object
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamsApi->download_team_logo_teams_team_id_logo_file_id_get_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **team_id** | **String** |  |  |
| **file_id** | **String** |  |  |

### Return type

**Object**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json, image/*


## get_team_culture_teams_team_id_culture_get

> Hash&lt;String, Object&gt; get_team_culture_teams_team_id_culture_get(team_id)

Get team culture details

Get detailed culture and values information for a team.

### Examples

```ruby
require 'time'
require 'openapi_client'
# setup authorization
OpenapiClient.configure do |config|
  # Configure Bearer authorization: HTTPBearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = OpenapiClient::TeamsApi.new
team_id = 'team_id_example' # String | 

begin
  # Get team culture details
  result = api_instance.get_team_culture_teams_team_id_culture_get(team_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamsApi->get_team_culture_teams_team_id_culture_get: #{e}"
end
```

#### Using the get_team_culture_teams_team_id_culture_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(Hash&lt;String, Object&gt;, Integer, Hash)> get_team_culture_teams_team_id_culture_get_with_http_info(team_id)

```ruby
begin
  # Get team culture details
  data, status_code, headers = api_instance.get_team_culture_teams_team_id_culture_get_with_http_info(team_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => Hash&lt;String, Object&gt;
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamsApi->get_team_culture_teams_team_id_culture_get_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **team_id** | **String** |  |  |

### Return type

**Hash&lt;String, Object&gt;**

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## get_team_rivals_teams_team_id_rivals_get

> <Array<Team>> get_team_rivals_teams_team_id_rivals_get(team_id)

Get team's rivals

Get all rival teams for a specific team.

### Examples

```ruby
require 'time'
require 'openapi_client'
# setup authorization
OpenapiClient.configure do |config|
  # Configure Bearer authorization: HTTPBearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = OpenapiClient::TeamsApi.new
team_id = 'team_id_example' # String | 

begin
  # Get team's rivals
  result = api_instance.get_team_rivals_teams_team_id_rivals_get(team_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamsApi->get_team_rivals_teams_team_id_rivals_get: #{e}"
end
```

#### Using the get_team_rivals_teams_team_id_rivals_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Array<Team>>, Integer, Hash)> get_team_rivals_teams_team_id_rivals_get_with_http_info(team_id)

```ruby
begin
  # Get team's rivals
  data, status_code, headers = api_instance.get_team_rivals_teams_team_id_rivals_get_with_http_info(team_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Array<Team>>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamsApi->get_team_rivals_teams_team_id_rivals_get_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **team_id** | **String** |  |  |

### Return type

[**Array&lt;Team&gt;**](Team.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## get_team_teams_team_id_get

> <Team> get_team_teams_team_id_get(team_id)

Get a team by ID

Retrieve detailed information about a specific team.

### Examples

```ruby
require 'time'
require 'openapi_client'
# setup authorization
OpenapiClient.configure do |config|
  # Configure Bearer authorization: HTTPBearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = OpenapiClient::TeamsApi.new
team_id = 'team_id_example' # String | 

begin
  # Get a team by ID
  result = api_instance.get_team_teams_team_id_get(team_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamsApi->get_team_teams_team_id_get: #{e}"
end
```

#### Using the get_team_teams_team_id_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Team>, Integer, Hash)> get_team_teams_team_id_get_with_http_info(team_id)

```ruby
begin
  # Get a team by ID
  data, status_code, headers = api_instance.get_team_teams_team_id_get_with_http_info(team_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Team>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamsApi->get_team_teams_team_id_get_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **team_id** | **String** |  |  |

### Return type

[**Team**](Team.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## list_team_logos_teams_team_id_logos_get

> <Array<FileUploadResponse>> list_team_logos_teams_team_id_logos_get(team_id)

List team logos

List all uploaded logos for a team.

### Examples

```ruby
require 'time'
require 'openapi_client'
# setup authorization
OpenapiClient.configure do |config|
  # Configure Bearer authorization: HTTPBearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = OpenapiClient::TeamsApi.new
team_id = 'team_id_example' # String | 

begin
  # List team logos
  result = api_instance.list_team_logos_teams_team_id_logos_get(team_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamsApi->list_team_logos_teams_team_id_logos_get: #{e}"
end
```

#### Using the list_team_logos_teams_team_id_logos_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Array<FileUploadResponse>>, Integer, Hash)> list_team_logos_teams_team_id_logos_get_with_http_info(team_id)

```ruby
begin
  # List team logos
  data, status_code, headers = api_instance.list_team_logos_teams_team_id_logos_get_with_http_info(team_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Array<FileUploadResponse>>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamsApi->list_team_logos_teams_team_id_logos_get_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **team_id** | **String** |  |  |

### Return type

[**Array&lt;FileUploadResponse&gt;**](FileUploadResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## list_teams_teams_get

> <PaginatedResponseTeam> list_teams_teams_get(opts)

List all teams

Get a paginated list of all teams with optional filtering by league or culture score.

### Examples

```ruby
require 'time'
require 'openapi_client'
# setup authorization
OpenapiClient.configure do |config|
  # Configure Bearer authorization: HTTPBearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = OpenapiClient::TeamsApi.new
opts = {
  league: OpenapiClient::League::PREMIER_LEAGUE, # League | Filter by league
  min_culture_score: 56, # Integer | Minimum culture score
  skip: 56, # Integer | Number of items to skip (offset)
  limit: 56 # Integer | Maximum number of items to return (max: 100)
}

begin
  # List all teams
  result = api_instance.list_teams_teams_get(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamsApi->list_teams_teams_get: #{e}"
end
```

#### Using the list_teams_teams_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<PaginatedResponseTeam>, Integer, Hash)> list_teams_teams_get_with_http_info(opts)

```ruby
begin
  # List all teams
  data, status_code, headers = api_instance.list_teams_teams_get_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <PaginatedResponseTeam>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamsApi->list_teams_teams_get_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **league** | [**League**](.md) | Filter by league | [optional] |
| **min_culture_score** | **Integer** | Minimum culture score | [optional] |
| **skip** | **Integer** | Number of items to skip (offset) | [optional][default to 0] |
| **limit** | **Integer** | Maximum number of items to return (max: 100) | [optional][default to 20] |

### Return type

[**PaginatedResponseTeam**](PaginatedResponseTeam.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## update_team_teams_team_id_patch

> <Team> update_team_teams_team_id_patch(team_id, team_update)

Update a team

Update specific fields of an existing team.

### Examples

```ruby
require 'time'
require 'openapi_client'
# setup authorization
OpenapiClient.configure do |config|
  # Configure Bearer authorization: HTTPBearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = OpenapiClient::TeamsApi.new
team_id = 'team_id_example' # String | 
team_update = OpenapiClient::TeamUpdate.new # TeamUpdate | 

begin
  # Update a team
  result = api_instance.update_team_teams_team_id_patch(team_id, team_update)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamsApi->update_team_teams_team_id_patch: #{e}"
end
```

#### Using the update_team_teams_team_id_patch_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<Team>, Integer, Hash)> update_team_teams_team_id_patch_with_http_info(team_id, team_update)

```ruby
begin
  # Update a team
  data, status_code, headers = api_instance.update_team_teams_team_id_patch_with_http_info(team_id, team_update)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <Team>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamsApi->update_team_teams_team_id_patch_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **team_id** | **String** |  |  |
| **team_update** | [**TeamUpdate**](TeamUpdate.md) |  |  |

### Return type

[**Team**](Team.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## upload_team_logo_teams_team_id_logo_post

> <FileUploadResponse> upload_team_logo_teams_team_id_logo_post(team_id, file)

Upload team logo

Upload a logo image for a team. Accepts image files (jpg, png, gif, webp).

### Examples

```ruby
require 'time'
require 'openapi_client'
# setup authorization
OpenapiClient.configure do |config|
  # Configure Bearer authorization: HTTPBearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = OpenapiClient::TeamsApi.new
team_id = 'team_id_example' # String | 
file = File.new('/path/to/some/file') # File | Logo image file

begin
  # Upload team logo
  result = api_instance.upload_team_logo_teams_team_id_logo_post(team_id, file)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamsApi->upload_team_logo_teams_team_id_logo_post: #{e}"
end
```

#### Using the upload_team_logo_teams_team_id_logo_post_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<FileUploadResponse>, Integer, Hash)> upload_team_logo_teams_team_id_logo_post_with_http_info(team_id, file)

```ruby
begin
  # Upload team logo
  data, status_code, headers = api_instance.upload_team_logo_teams_team_id_logo_post_with_http_info(team_id, file)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <FileUploadResponse>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamsApi->upload_team_logo_teams_team_id_logo_post_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **team_id** | **String** |  |  |
| **file** | **File** | Logo image file |  |

### Return type

[**FileUploadResponse**](FileUploadResponse.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: application/json

