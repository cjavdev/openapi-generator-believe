# openapi_client.TeamMembersApi

All URIs are relative to *https://believe.cjav.dev*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_team_member_team_members_post**](TeamMembersApi.md#create_team_member_team_members_post) | **POST** /team-members | Create a new team member
[**delete_team_member_team_members_member_id_delete**](TeamMembersApi.md#delete_team_member_team_members_member_id_delete) | **DELETE** /team-members/{member_id} | Delete a team member
[**get_team_member_team_members_member_id_get**](TeamMembersApi.md#get_team_member_team_members_member_id_get) | **GET** /team-members/{member_id} | Get a team member by ID
[**list_coaches_team_members_coaches_get**](TeamMembersApi.md#list_coaches_team_members_coaches_get) | **GET** /team-members/coaches/ | List all coaches
[**list_players_team_members_players_get**](TeamMembersApi.md#list_players_team_members_players_get) | **GET** /team-members/players/ | List all players
[**list_staff_team_members_staff_get**](TeamMembersApi.md#list_staff_team_members_staff_get) | **GET** /team-members/staff/ | List all staff (non-player, non-coach)
[**list_team_members_team_members_get**](TeamMembersApi.md#list_team_members_team_members_get) | **GET** /team-members | List all team members
[**update_team_member_team_members_member_id_patch**](TeamMembersApi.md#update_team_member_team_members_member_id_patch) | **PATCH** /team-members/{member_id} | Update a team member


# **create_team_member_team_members_post**
> ResponseCreateTeamMemberTeamMembersPost create_team_member_team_members_post(member)

Create a new team member

Add a new team member to a team.

The request body is a **union type (oneOf)** - you must include the `member_type` discriminator field:
- `"member_type": "player"` - Creates a player (requires position, jersey_number, etc.)
- `"member_type": "coach"` - Creates a coach (requires specialty, etc.)
- `"member_type": "medical_staff"` - Creates medical staff (requires medical specialty, etc.)
- `"member_type": "equipment_manager"` - Creates equipment manager (requires responsibilities, etc.)

The `character_id` field references an existing character from `/characters/{id}`.

**Example for creating a player:**
```json
{
  "member_type": "player",
  "character_id": "sam-obisanya",
  "team_id": "afc-richmond",
  "years_with_team": 2,
  "position": "midfielder",
  "jersey_number": 24,
  "goals_scored": 12,
  "assists": 15
}
```

### Example

* Bearer Authentication (HTTPBearer):

```python
import openapi_client
from openapi_client.models.member import Member
from openapi_client.models.response_create_team_member_team_members_post import ResponseCreateTeamMemberTeamMembersPost
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
    api_instance = openapi_client.TeamMembersApi(api_client)
    member = openapi_client.Member() # Member | 

    try:
        # Create a new team member
        api_response = api_instance.create_team_member_team_members_post(member)
        print("The response of TeamMembersApi->create_team_member_team_members_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TeamMembersApi->create_team_member_team_members_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **member** | [**Member**](Member.md)|  | 

### Return type

[**ResponseCreateTeamMemberTeamMembersPost**](ResponseCreateTeamMemberTeamMembersPost.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Team member created successfully |  -  |
**409** | Team member already exists |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_team_member_team_members_member_id_delete**
> delete_team_member_team_members_member_id_delete(member_id)

Delete a team member

Remove a team member from the roster.

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
    api_instance = openapi_client.TeamMembersApi(api_client)
    member_id = 'member_id_example' # str | 

    try:
        # Delete a team member
        api_instance.delete_team_member_team_members_member_id_delete(member_id)
    except Exception as e:
        print("Exception when calling TeamMembersApi->delete_team_member_team_members_member_id_delete: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **member_id** | **str**|  | 

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
**204** | Team member removed successfully |  -  |
**404** | Team member not found |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_team_member_team_members_member_id_get**
> ResponseGetTeamMemberTeamMembersMemberIdGet get_team_member_team_members_member_id_get(member_id)

Get a team member by ID

Retrieve detailed information about a specific team member.

The response is a **union type (oneOf)** - the actual shape depends on the member's type:
- **player**: Includes position, jersey_number, goals_scored, assists, is_captain
- **coach**: Includes specialty, certifications, win_rate
- **medical_staff**: Includes specialty, qualifications, license_number
- **equipment_manager**: Includes responsibilities, is_head_kitman

Use `character_id` to fetch full character details from `/characters/{character_id}`.

### Example

* Bearer Authentication (HTTPBearer):

```python
import openapi_client
from openapi_client.models.response_get_team_member_team_members_member_id_get import ResponseGetTeamMemberTeamMembersMemberIdGet
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
    api_instance = openapi_client.TeamMembersApi(api_client)
    member_id = 'member_id_example' # str | 

    try:
        # Get a team member by ID
        api_response = api_instance.get_team_member_team_members_member_id_get(member_id)
        print("The response of TeamMembersApi->get_team_member_team_members_member_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TeamMembersApi->get_team_member_team_members_member_id_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **member_id** | **str**|  | 

### Return type

[**ResponseGetTeamMemberTeamMembersMemberIdGet**](ResponseGetTeamMemberTeamMembersMemberIdGet.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Team member details (oneOf based on member_type) |  -  |
**404** | Team member not found |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_coaches_team_members_coaches_get**
> PaginatedResponseCoach list_coaches_team_members_coaches_get(specialty=specialty, team_id=team_id, skip=skip, limit=limit)

List all coaches

Get only coaches (filtered subset of team members).

### Example

* Bearer Authentication (HTTPBearer):

```python
import openapi_client
from openapi_client.models.paginated_response_coach import PaginatedResponseCoach
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
    api_instance = openapi_client.TeamMembersApi(api_client)
    specialty = openapi_client.CoachSpecialty() # CoachSpecialty | Filter by specialty (optional)
    team_id = 'team_id_example' # str | Filter by team ID (optional)
    skip = 0 # int | Number of items to skip (offset) (optional) (default to 0)
    limit = 20 # int | Maximum number of items to return (max: 100) (optional) (default to 20)

    try:
        # List all coaches
        api_response = api_instance.list_coaches_team_members_coaches_get(specialty=specialty, team_id=team_id, skip=skip, limit=limit)
        print("The response of TeamMembersApi->list_coaches_team_members_coaches_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TeamMembersApi->list_coaches_team_members_coaches_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **specialty** | [**CoachSpecialty**](.md)| Filter by specialty | [optional] 
 **team_id** | **str**| Filter by team ID | [optional] 
 **skip** | **int**| Number of items to skip (offset) | [optional] [default to 0]
 **limit** | **int**| Maximum number of items to return (max: 100) | [optional] [default to 20]

### Return type

[**PaginatedResponseCoach**](PaginatedResponseCoach.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_players_team_members_players_get**
> PaginatedResponsePlayer list_players_team_members_players_get(position=position, team_id=team_id, skip=skip, limit=limit)

List all players

Get only players (filtered subset of team members).

### Example

* Bearer Authentication (HTTPBearer):

```python
import openapi_client
from openapi_client.models.paginated_response_player import PaginatedResponsePlayer
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
    api_instance = openapi_client.TeamMembersApi(api_client)
    position = openapi_client.Position() # Position | Filter by position (optional)
    team_id = 'team_id_example' # str | Filter by team ID (optional)
    skip = 0 # int | Number of items to skip (offset) (optional) (default to 0)
    limit = 20 # int | Maximum number of items to return (max: 100) (optional) (default to 20)

    try:
        # List all players
        api_response = api_instance.list_players_team_members_players_get(position=position, team_id=team_id, skip=skip, limit=limit)
        print("The response of TeamMembersApi->list_players_team_members_players_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TeamMembersApi->list_players_team_members_players_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **position** | [**Position**](.md)| Filter by position | [optional] 
 **team_id** | **str**| Filter by team ID | [optional] 
 **skip** | **int**| Number of items to skip (offset) | [optional] [default to 0]
 **limit** | **int**| Maximum number of items to return (max: 100) | [optional] [default to 20]

### Return type

[**PaginatedResponsePlayer**](PaginatedResponsePlayer.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_staff_team_members_staff_get**
> PaginatedResponseUnionMedicalStaffEquipmentManager list_staff_team_members_staff_get(team_id=team_id, skip=skip, limit=limit)

List all staff (non-player, non-coach)

Get all staff members (medical staff and equipment managers).

This demonstrates a **narrower union type** - the response is oneOf MedicalStaff or EquipmentManager.

### Example

* Bearer Authentication (HTTPBearer):

```python
import openapi_client
from openapi_client.models.paginated_response_union_medical_staff_equipment_manager import PaginatedResponseUnionMedicalStaffEquipmentManager
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
    api_instance = openapi_client.TeamMembersApi(api_client)
    team_id = 'team_id_example' # str | Filter by team ID (optional)
    skip = 0 # int | Number of items to skip (offset) (optional) (default to 0)
    limit = 20 # int | Maximum number of items to return (max: 100) (optional) (default to 20)

    try:
        # List all staff (non-player, non-coach)
        api_response = api_instance.list_staff_team_members_staff_get(team_id=team_id, skip=skip, limit=limit)
        print("The response of TeamMembersApi->list_staff_team_members_staff_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TeamMembersApi->list_staff_team_members_staff_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **team_id** | **str**| Filter by team ID | [optional] 
 **skip** | **int**| Number of items to skip (offset) | [optional] [default to 0]
 **limit** | **int**| Maximum number of items to return (max: 100) | [optional] [default to 20]

### Return type

[**PaginatedResponseUnionMedicalStaffEquipmentManager**](PaginatedResponseUnionMedicalStaffEquipmentManager.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_team_members_team_members_get**
> PaginatedResponseAnnotatedUnionPlayerCoachMedicalStaffEquipmentManagerFieldInfoAnnotationNoneTypeRequiredTrueDiscriminatorMemberType list_team_members_team_members_get(member_type=member_type, team_id=team_id, skip=skip, limit=limit)

List all team members

Get a paginated list of all team members.

This endpoint demonstrates **union types (oneOf)** in the response.
Each team member can be one of: Player, Coach, MedicalStaff, or EquipmentManager.
The `member_type` field acts as a discriminator to determine the shape of each object.

### Example

* Bearer Authentication (HTTPBearer):

```python
import openapi_client
from openapi_client.models.paginated_response_annotated_union_player_coach_medical_staff_equipment_manager_field_info_annotation_none_type_required_true_discriminator_member_type import PaginatedResponseAnnotatedUnionPlayerCoachMedicalStaffEquipmentManagerFieldInfoAnnotationNoneTypeRequiredTrueDiscriminatorMemberType
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
    api_instance = openapi_client.TeamMembersApi(api_client)
    member_type = openapi_client.MemberType() # MemberType | Filter by member type (optional)
    team_id = 'team_id_example' # str | Filter by team ID (optional)
    skip = 0 # int | Number of items to skip (offset) (optional) (default to 0)
    limit = 20 # int | Maximum number of items to return (max: 100) (optional) (default to 20)

    try:
        # List all team members
        api_response = api_instance.list_team_members_team_members_get(member_type=member_type, team_id=team_id, skip=skip, limit=limit)
        print("The response of TeamMembersApi->list_team_members_team_members_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TeamMembersApi->list_team_members_team_members_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **member_type** | [**MemberType**](.md)| Filter by member type | [optional] 
 **team_id** | **str**| Filter by team ID | [optional] 
 **skip** | **int**| Number of items to skip (offset) | [optional] [default to 0]
 **limit** | **int**| Maximum number of items to return (max: 100) | [optional] [default to 20]

### Return type

[**PaginatedResponseAnnotatedUnionPlayerCoachMedicalStaffEquipmentManagerFieldInfoAnnotationNoneTypeRequiredTrueDiscriminatorMemberType**](PaginatedResponseAnnotatedUnionPlayerCoachMedicalStaffEquipmentManagerFieldInfoAnnotationNoneTypeRequiredTrueDiscriminatorMemberType.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Paginated list of team members (oneOf: Player, Coach, MedicalStaff, EquipmentManager) |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_team_member_team_members_member_id_patch**
> ResponseUpdateTeamMemberTeamMembersMemberIdPatch update_team_member_team_members_member_id_patch(member_id, updates)

Update a team member

Update specific fields of an existing team member. Fields vary by member type.

### Example

* Bearer Authentication (HTTPBearer):

```python
import openapi_client
from openapi_client.models.response_update_team_member_team_members_member_id_patch import ResponseUpdateTeamMemberTeamMembersMemberIdPatch
from openapi_client.models.updates import Updates
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
    api_instance = openapi_client.TeamMembersApi(api_client)
    member_id = 'member_id_example' # str | 
    updates = openapi_client.Updates() # Updates | 

    try:
        # Update a team member
        api_response = api_instance.update_team_member_team_members_member_id_patch(member_id, updates)
        print("The response of TeamMembersApi->update_team_member_team_members_member_id_patch:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TeamMembersApi->update_team_member_team_members_member_id_patch: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **member_id** | **str**|  | 
 **updates** | [**Updates**](Updates.md)|  | 

### Return type

[**ResponseUpdateTeamMemberTeamMembersMemberIdPatch**](ResponseUpdateTeamMemberTeamMembersMemberIdPatch.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Team member updated successfully |  -  |
**404** | Team member not found |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

