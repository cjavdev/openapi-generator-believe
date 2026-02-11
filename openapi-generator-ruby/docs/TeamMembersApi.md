# OpenapiClient::TeamMembersApi

All URIs are relative to *https://believe.cjav.dev*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**create_team_member_team_members_post**](TeamMembersApi.md#create_team_member_team_members_post) | **POST** /team-members | Create a new team member |
| [**delete_team_member_team_members_member_id_delete**](TeamMembersApi.md#delete_team_member_team_members_member_id_delete) | **DELETE** /team-members/{member_id} | Delete a team member |
| [**get_team_member_team_members_member_id_get**](TeamMembersApi.md#get_team_member_team_members_member_id_get) | **GET** /team-members/{member_id} | Get a team member by ID |
| [**list_coaches_team_members_coaches_get**](TeamMembersApi.md#list_coaches_team_members_coaches_get) | **GET** /team-members/coaches/ | List all coaches |
| [**list_players_team_members_players_get**](TeamMembersApi.md#list_players_team_members_players_get) | **GET** /team-members/players/ | List all players |
| [**list_staff_team_members_staff_get**](TeamMembersApi.md#list_staff_team_members_staff_get) | **GET** /team-members/staff/ | List all staff (non-player, non-coach) |
| [**list_team_members_team_members_get**](TeamMembersApi.md#list_team_members_team_members_get) | **GET** /team-members | List all team members |
| [**update_team_member_team_members_member_id_patch**](TeamMembersApi.md#update_team_member_team_members_member_id_patch) | **PATCH** /team-members/{member_id} | Update a team member |


## create_team_member_team_members_post

> <ResponseCreateTeamMemberTeamMembersPost> create_team_member_team_members_post(member)

Create a new team member

Add a new team member to a team.  The request body is a **union type (oneOf)** - you must include the `member_type` discriminator field: - `\"member_type\": \"player\"` - Creates a player (requires position, jersey_number, etc.) - `\"member_type\": \"coach\"` - Creates a coach (requires specialty, etc.) - `\"member_type\": \"medical_staff\"` - Creates medical staff (requires medical specialty, etc.) - `\"member_type\": \"equipment_manager\"` - Creates equipment manager (requires responsibilities, etc.)  The `character_id` field references an existing character from `/characters/{id}`.  **Example for creating a player:** ```json {   \"member_type\": \"player\",   \"character_id\": \"sam-obisanya\",   \"team_id\": \"afc-richmond\",   \"years_with_team\": 2,   \"position\": \"midfielder\",   \"jersey_number\": 24,   \"goals_scored\": 12,   \"assists\": 15 } ```

### Examples

```ruby
require 'time'
require 'openapi_client'
# setup authorization
OpenapiClient.configure do |config|
  # Configure Bearer authorization: HTTPBearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = OpenapiClient::TeamMembersApi.new
member = OpenapiClient::CoachBase.new({character_id: 'jamie-tartt', specialty: OpenapiClient::CoachSpecialty::HEAD_COACH, team_id: 'afc-richmond', years_with_team: 3}) # Member | 

begin
  # Create a new team member
  result = api_instance.create_team_member_team_members_post(member)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamMembersApi->create_team_member_team_members_post: #{e}"
end
```

#### Using the create_team_member_team_members_post_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ResponseCreateTeamMemberTeamMembersPost>, Integer, Hash)> create_team_member_team_members_post_with_http_info(member)

```ruby
begin
  # Create a new team member
  data, status_code, headers = api_instance.create_team_member_team_members_post_with_http_info(member)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ResponseCreateTeamMemberTeamMembersPost>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamMembersApi->create_team_member_team_members_post_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **member** | [**Member**](Member.md) |  |  |

### Return type

[**ResponseCreateTeamMemberTeamMembersPost**](ResponseCreateTeamMemberTeamMembersPost.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## delete_team_member_team_members_member_id_delete

> delete_team_member_team_members_member_id_delete(member_id)

Delete a team member

Remove a team member from the roster.

### Examples

```ruby
require 'time'
require 'openapi_client'
# setup authorization
OpenapiClient.configure do |config|
  # Configure Bearer authorization: HTTPBearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = OpenapiClient::TeamMembersApi.new
member_id = 'member_id_example' # String | 

begin
  # Delete a team member
  api_instance.delete_team_member_team_members_member_id_delete(member_id)
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamMembersApi->delete_team_member_team_members_member_id_delete: #{e}"
end
```

#### Using the delete_team_member_team_members_member_id_delete_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> delete_team_member_team_members_member_id_delete_with_http_info(member_id)

```ruby
begin
  # Delete a team member
  data, status_code, headers = api_instance.delete_team_member_team_members_member_id_delete_with_http_info(member_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamMembersApi->delete_team_member_team_members_member_id_delete_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **member_id** | **String** |  |  |

### Return type

nil (empty response body)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## get_team_member_team_members_member_id_get

> <ResponseGetTeamMemberTeamMembersMemberIdGet> get_team_member_team_members_member_id_get(member_id)

Get a team member by ID

Retrieve detailed information about a specific team member.  The response is a **union type (oneOf)** - the actual shape depends on the member's type: - **player**: Includes position, jersey_number, goals_scored, assists, is_captain - **coach**: Includes specialty, certifications, win_rate - **medical_staff**: Includes specialty, qualifications, license_number - **equipment_manager**: Includes responsibilities, is_head_kitman  Use `character_id` to fetch full character details from `/characters/{character_id}`.

### Examples

```ruby
require 'time'
require 'openapi_client'
# setup authorization
OpenapiClient.configure do |config|
  # Configure Bearer authorization: HTTPBearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = OpenapiClient::TeamMembersApi.new
member_id = 'member_id_example' # String | 

begin
  # Get a team member by ID
  result = api_instance.get_team_member_team_members_member_id_get(member_id)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamMembersApi->get_team_member_team_members_member_id_get: #{e}"
end
```

#### Using the get_team_member_team_members_member_id_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ResponseGetTeamMemberTeamMembersMemberIdGet>, Integer, Hash)> get_team_member_team_members_member_id_get_with_http_info(member_id)

```ruby
begin
  # Get a team member by ID
  data, status_code, headers = api_instance.get_team_member_team_members_member_id_get_with_http_info(member_id)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ResponseGetTeamMemberTeamMembersMemberIdGet>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamMembersApi->get_team_member_team_members_member_id_get_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **member_id** | **String** |  |  |

### Return type

[**ResponseGetTeamMemberTeamMembersMemberIdGet**](ResponseGetTeamMemberTeamMembersMemberIdGet.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## list_coaches_team_members_coaches_get

> <PaginatedResponseCoach> list_coaches_team_members_coaches_get(opts)

List all coaches

Get only coaches (filtered subset of team members).

### Examples

```ruby
require 'time'
require 'openapi_client'
# setup authorization
OpenapiClient.configure do |config|
  # Configure Bearer authorization: HTTPBearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = OpenapiClient::TeamMembersApi.new
opts = {
  specialty: OpenapiClient::CoachSpecialty::HEAD_COACH, # CoachSpecialty | Filter by specialty
  team_id: 'team_id_example', # String | Filter by team ID
  skip: 56, # Integer | Number of items to skip (offset)
  limit: 56 # Integer | Maximum number of items to return (max: 100)
}

begin
  # List all coaches
  result = api_instance.list_coaches_team_members_coaches_get(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamMembersApi->list_coaches_team_members_coaches_get: #{e}"
end
```

#### Using the list_coaches_team_members_coaches_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<PaginatedResponseCoach>, Integer, Hash)> list_coaches_team_members_coaches_get_with_http_info(opts)

```ruby
begin
  # List all coaches
  data, status_code, headers = api_instance.list_coaches_team_members_coaches_get_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <PaginatedResponseCoach>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamMembersApi->list_coaches_team_members_coaches_get_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **specialty** | [**CoachSpecialty**](.md) | Filter by specialty | [optional] |
| **team_id** | **String** | Filter by team ID | [optional] |
| **skip** | **Integer** | Number of items to skip (offset) | [optional][default to 0] |
| **limit** | **Integer** | Maximum number of items to return (max: 100) | [optional][default to 20] |

### Return type

[**PaginatedResponseCoach**](PaginatedResponseCoach.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## list_players_team_members_players_get

> <PaginatedResponsePlayer> list_players_team_members_players_get(opts)

List all players

Get only players (filtered subset of team members).

### Examples

```ruby
require 'time'
require 'openapi_client'
# setup authorization
OpenapiClient.configure do |config|
  # Configure Bearer authorization: HTTPBearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = OpenapiClient::TeamMembersApi.new
opts = {
  position: OpenapiClient::Position::GOALKEEPER, # Position | Filter by position
  team_id: 'team_id_example', # String | Filter by team ID
  skip: 56, # Integer | Number of items to skip (offset)
  limit: 56 # Integer | Maximum number of items to return (max: 100)
}

begin
  # List all players
  result = api_instance.list_players_team_members_players_get(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamMembersApi->list_players_team_members_players_get: #{e}"
end
```

#### Using the list_players_team_members_players_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<PaginatedResponsePlayer>, Integer, Hash)> list_players_team_members_players_get_with_http_info(opts)

```ruby
begin
  # List all players
  data, status_code, headers = api_instance.list_players_team_members_players_get_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <PaginatedResponsePlayer>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamMembersApi->list_players_team_members_players_get_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **position** | [**Position**](.md) | Filter by position | [optional] |
| **team_id** | **String** | Filter by team ID | [optional] |
| **skip** | **Integer** | Number of items to skip (offset) | [optional][default to 0] |
| **limit** | **Integer** | Maximum number of items to return (max: 100) | [optional][default to 20] |

### Return type

[**PaginatedResponsePlayer**](PaginatedResponsePlayer.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## list_staff_team_members_staff_get

> <PaginatedResponseUnionMedicalStaffEquipmentManager> list_staff_team_members_staff_get(opts)

List all staff (non-player, non-coach)

Get all staff members (medical staff and equipment managers).  This demonstrates a **narrower union type** - the response is oneOf MedicalStaff or EquipmentManager.

### Examples

```ruby
require 'time'
require 'openapi_client'
# setup authorization
OpenapiClient.configure do |config|
  # Configure Bearer authorization: HTTPBearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = OpenapiClient::TeamMembersApi.new
opts = {
  team_id: 'team_id_example', # String | Filter by team ID
  skip: 56, # Integer | Number of items to skip (offset)
  limit: 56 # Integer | Maximum number of items to return (max: 100)
}

begin
  # List all staff (non-player, non-coach)
  result = api_instance.list_staff_team_members_staff_get(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamMembersApi->list_staff_team_members_staff_get: #{e}"
end
```

#### Using the list_staff_team_members_staff_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<PaginatedResponseUnionMedicalStaffEquipmentManager>, Integer, Hash)> list_staff_team_members_staff_get_with_http_info(opts)

```ruby
begin
  # List all staff (non-player, non-coach)
  data, status_code, headers = api_instance.list_staff_team_members_staff_get_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <PaginatedResponseUnionMedicalStaffEquipmentManager>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamMembersApi->list_staff_team_members_staff_get_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **team_id** | **String** | Filter by team ID | [optional] |
| **skip** | **Integer** | Number of items to skip (offset) | [optional][default to 0] |
| **limit** | **Integer** | Maximum number of items to return (max: 100) | [optional][default to 20] |

### Return type

[**PaginatedResponseUnionMedicalStaffEquipmentManager**](PaginatedResponseUnionMedicalStaffEquipmentManager.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## list_team_members_team_members_get

> <PaginatedResponseAnnotatedUnionPlayerCoachMedicalStaffEquipmentManagerFieldInfoAnnotationNoneTypeRequiredTrueDiscriminatorMemberType> list_team_members_team_members_get(opts)

List all team members

Get a paginated list of all team members.  This endpoint demonstrates **union types (oneOf)** in the response. Each team member can be one of: Player, Coach, MedicalStaff, or EquipmentManager. The `member_type` field acts as a discriminator to determine the shape of each object.

### Examples

```ruby
require 'time'
require 'openapi_client'
# setup authorization
OpenapiClient.configure do |config|
  # Configure Bearer authorization: HTTPBearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = OpenapiClient::TeamMembersApi.new
opts = {
  member_type: OpenapiClient::MemberType::PLAYER, # MemberType | Filter by member type
  team_id: 'team_id_example', # String | Filter by team ID
  skip: 56, # Integer | Number of items to skip (offset)
  limit: 56 # Integer | Maximum number of items to return (max: 100)
}

begin
  # List all team members
  result = api_instance.list_team_members_team_members_get(opts)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamMembersApi->list_team_members_team_members_get: #{e}"
end
```

#### Using the list_team_members_team_members_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<PaginatedResponseAnnotatedUnionPlayerCoachMedicalStaffEquipmentManagerFieldInfoAnnotationNoneTypeRequiredTrueDiscriminatorMemberType>, Integer, Hash)> list_team_members_team_members_get_with_http_info(opts)

```ruby
begin
  # List all team members
  data, status_code, headers = api_instance.list_team_members_team_members_get_with_http_info(opts)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <PaginatedResponseAnnotatedUnionPlayerCoachMedicalStaffEquipmentManagerFieldInfoAnnotationNoneTypeRequiredTrueDiscriminatorMemberType>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamMembersApi->list_team_members_team_members_get_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **member_type** | [**MemberType**](.md) | Filter by member type | [optional] |
| **team_id** | **String** | Filter by team ID | [optional] |
| **skip** | **Integer** | Number of items to skip (offset) | [optional][default to 0] |
| **limit** | **Integer** | Maximum number of items to return (max: 100) | [optional][default to 20] |

### Return type

[**PaginatedResponseAnnotatedUnionPlayerCoachMedicalStaffEquipmentManagerFieldInfoAnnotationNoneTypeRequiredTrueDiscriminatorMemberType**](PaginatedResponseAnnotatedUnionPlayerCoachMedicalStaffEquipmentManagerFieldInfoAnnotationNoneTypeRequiredTrueDiscriminatorMemberType.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## update_team_member_team_members_member_id_patch

> <ResponseUpdateTeamMemberTeamMembersMemberIdPatch> update_team_member_team_members_member_id_patch(member_id, updates)

Update a team member

Update specific fields of an existing team member. Fields vary by member type.

### Examples

```ruby
require 'time'
require 'openapi_client'
# setup authorization
OpenapiClient.configure do |config|
  # Configure Bearer authorization: HTTPBearer
  config.access_token = 'YOUR_BEARER_TOKEN'
end

api_instance = OpenapiClient::TeamMembersApi.new
member_id = 'member_id_example' # String | 
updates = OpenapiClient::Updates.new # Updates | 

begin
  # Update a team member
  result = api_instance.update_team_member_team_members_member_id_patch(member_id, updates)
  p result
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamMembersApi->update_team_member_team_members_member_id_patch: #{e}"
end
```

#### Using the update_team_member_team_members_member_id_patch_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ResponseUpdateTeamMemberTeamMembersMemberIdPatch>, Integer, Hash)> update_team_member_team_members_member_id_patch_with_http_info(member_id, updates)

```ruby
begin
  # Update a team member
  data, status_code, headers = api_instance.update_team_member_team_members_member_id_patch_with_http_info(member_id, updates)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ResponseUpdateTeamMemberTeamMembersMemberIdPatch>
rescue OpenapiClient::ApiError => e
  puts "Error when calling TeamMembersApi->update_team_member_team_members_member_id_patch_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **member_id** | **String** |  |  |
| **updates** | [**Updates**](Updates.md) |  |  |

### Return type

[**ResponseUpdateTeamMemberTeamMembersMemberIdPatch**](ResponseUpdateTeamMemberTeamMembersMemberIdPatch.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

