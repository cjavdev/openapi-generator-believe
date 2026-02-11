# Org.OpenAPITools.Api.TeamMembersApi

All URIs are relative to *https://believe.cjav.dev*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**CreateTeamMemberTeamMembersPost**](TeamMembersApi.md#createteammemberteammemberspost) | **POST** /team-members | Create a new team member |
| [**DeleteTeamMemberTeamMembersMemberIdDelete**](TeamMembersApi.md#deleteteammemberteammembersmemberiddelete) | **DELETE** /team-members/{member_id} | Delete a team member |
| [**GetTeamMemberTeamMembersMemberIdGet**](TeamMembersApi.md#getteammemberteammembersmemberidget) | **GET** /team-members/{member_id} | Get a team member by ID |
| [**ListCoachesTeamMembersCoachesGet**](TeamMembersApi.md#listcoachesteammemberscoachesget) | **GET** /team-members/coaches/ | List all coaches |
| [**ListPlayersTeamMembersPlayersGet**](TeamMembersApi.md#listplayersteammembersplayersget) | **GET** /team-members/players/ | List all players |
| [**ListStaffTeamMembersStaffGet**](TeamMembersApi.md#liststaffteammembersstaffget) | **GET** /team-members/staff/ | List all staff (non-player, non-coach) |
| [**ListTeamMembersTeamMembersGet**](TeamMembersApi.md#listteammembersteammembersget) | **GET** /team-members | List all team members |
| [**UpdateTeamMemberTeamMembersMemberIdPatch**](TeamMembersApi.md#updateteammemberteammembersmemberidpatch) | **PATCH** /team-members/{member_id} | Update a team member |

<a id="createteammemberteammemberspost"></a>
# **CreateTeamMemberTeamMembersPost**
> ResponseCreateTeamMemberTeamMembersPost CreateTeamMemberTeamMembersPost (Member member)

Create a new team member

Add a new team member to a team.  The request body is a **union type (oneOf)** - you must include the `member_type` discriminator field: - `\"member_type\": \"player\"` - Creates a player (requires position, jersey_number, etc.) - `\"member_type\": \"coach\"` - Creates a coach (requires specialty, etc.) - `\"member_type\": \"medical_staff\"` - Creates medical staff (requires medical specialty, etc.) - `\"member_type\": \"equipment_manager\"` - Creates equipment manager (requires responsibilities, etc.)  The `character_id` field references an existing character from `/characters/{id}`.  **Example for creating a player:** ```json {   \"member_type\": \"player\",   \"character_id\": \"sam-obisanya\",   \"team_id\": \"afc-richmond\",   \"years_with_team\": 2,   \"position\": \"midfielder\",   \"jersey_number\": 24,   \"goals_scored\": 12,   \"assists\": 15 } ```


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **member** | [**Member**](Member.md) |  |  |

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
| **201** | Team member created successfully |  -  |
| **409** | Team member already exists |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="deleteteammemberteammembersmemberiddelete"></a>
# **DeleteTeamMemberTeamMembersMemberIdDelete**
> void DeleteTeamMemberTeamMembersMemberIdDelete (string memberId)

Delete a team member

Remove a team member from the roster.


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **memberId** | **string** |  |  |

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
| **204** | Team member removed successfully |  -  |
| **404** | Team member not found |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="getteammemberteammembersmemberidget"></a>
# **GetTeamMemberTeamMembersMemberIdGet**
> ResponseGetTeamMemberTeamMembersMemberIdGet GetTeamMemberTeamMembersMemberIdGet (string memberId)

Get a team member by ID

Retrieve detailed information about a specific team member.  The response is a **union type (oneOf)** - the actual shape depends on the member's type: - **player**: Includes position, jersey_number, goals_scored, assists, is_captain - **coach**: Includes specialty, certifications, win_rate - **medical_staff**: Includes specialty, qualifications, license_number - **equipment_manager**: Includes responsibilities, is_head_kitman  Use `character_id` to fetch full character details from `/characters/{character_id}`.


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **memberId** | **string** |  |  |

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
| **200** | Team member details (oneOf based on member_type) |  -  |
| **404** | Team member not found |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="listcoachesteammemberscoachesget"></a>
# **ListCoachesTeamMembersCoachesGet**
> PaginatedResponseCoach ListCoachesTeamMembersCoachesGet (CoachSpecialty specialty = null, string teamId = null, int skip = null, int limit = null)

List all coaches

Get only coaches (filtered subset of team members).


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **specialty** | **CoachSpecialty** | Filter by specialty | [optional]  |
| **teamId** | **string** | Filter by team ID | [optional]  |
| **skip** | **int** | Number of items to skip (offset) | [optional] [default to 0] |
| **limit** | **int** | Maximum number of items to return (max: 100) | [optional] [default to 20] |

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
| **200** | Successful Response |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="listplayersteammembersplayersget"></a>
# **ListPlayersTeamMembersPlayersGet**
> PaginatedResponsePlayer ListPlayersTeamMembersPlayersGet (Position position = null, string teamId = null, int skip = null, int limit = null)

List all players

Get only players (filtered subset of team members).


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **position** | **Position** | Filter by position | [optional]  |
| **teamId** | **string** | Filter by team ID | [optional]  |
| **skip** | **int** | Number of items to skip (offset) | [optional] [default to 0] |
| **limit** | **int** | Maximum number of items to return (max: 100) | [optional] [default to 20] |

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
| **200** | Successful Response |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="liststaffteammembersstaffget"></a>
# **ListStaffTeamMembersStaffGet**
> PaginatedResponseUnionMedicalStaffEquipmentManager ListStaffTeamMembersStaffGet (string teamId = null, int skip = null, int limit = null)

List all staff (non-player, non-coach)

Get all staff members (medical staff and equipment managers).  This demonstrates a **narrower union type** - the response is oneOf MedicalStaff or EquipmentManager.


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **teamId** | **string** | Filter by team ID | [optional]  |
| **skip** | **int** | Number of items to skip (offset) | [optional] [default to 0] |
| **limit** | **int** | Maximum number of items to return (max: 100) | [optional] [default to 20] |

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
| **200** | Successful Response |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="listteammembersteammembersget"></a>
# **ListTeamMembersTeamMembersGet**
> PaginatedResponseAnnotatedUnionPlayerCoachMedicalStaffEquipmentManagerFieldInfoAnnotationNoneTypeRequiredTrueDiscriminatorMemberType ListTeamMembersTeamMembersGet (MemberType memberType = null, string teamId = null, int skip = null, int limit = null)

List all team members

Get a paginated list of all team members.  This endpoint demonstrates **union types (oneOf)** in the response. Each team member can be one of: Player, Coach, MedicalStaff, or EquipmentManager. The `member_type` field acts as a discriminator to determine the shape of each object.


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **memberType** | **MemberType** | Filter by member type | [optional]  |
| **teamId** | **string** | Filter by team ID | [optional]  |
| **skip** | **int** | Number of items to skip (offset) | [optional] [default to 0] |
| **limit** | **int** | Maximum number of items to return (max: 100) | [optional] [default to 20] |

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
| **200** | Paginated list of team members (oneOf: Player, Coach, MedicalStaff, EquipmentManager) |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="updateteammemberteammembersmemberidpatch"></a>
# **UpdateTeamMemberTeamMembersMemberIdPatch**
> ResponseUpdateTeamMemberTeamMembersMemberIdPatch UpdateTeamMemberTeamMembersMemberIdPatch (string memberId, Updates updates)

Update a team member

Update specific fields of an existing team member. Fields vary by member type.


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **memberId** | **string** |  |  |
| **updates** | [**Updates**](Updates.md) |  |  |

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
| **200** | Team member updated successfully |  -  |
| **404** | Team member not found |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

