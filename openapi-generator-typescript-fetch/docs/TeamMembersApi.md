# TeamMembersApi

All URIs are relative to *https://believe.cjav.dev*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
| [**createTeamMemberTeamMembersPost**](TeamMembersApi.md#createteammemberteammemberspost) | **POST** /team-members | Create a new team member |
| [**deleteTeamMemberTeamMembersMemberIdDelete**](TeamMembersApi.md#deleteteammemberteammembersmemberiddelete) | **DELETE** /team-members/{member_id} | Delete a team member |
| [**getTeamMemberTeamMembersMemberIdGet**](TeamMembersApi.md#getteammemberteammembersmemberidget) | **GET** /team-members/{member_id} | Get a team member by ID |
| [**listCoachesTeamMembersCoachesGet**](TeamMembersApi.md#listcoachesteammemberscoachesget) | **GET** /team-members/coaches/ | List all coaches |
| [**listPlayersTeamMembersPlayersGet**](TeamMembersApi.md#listplayersteammembersplayersget) | **GET** /team-members/players/ | List all players |
| [**listStaffTeamMembersStaffGet**](TeamMembersApi.md#liststaffteammembersstaffget) | **GET** /team-members/staff/ | List all staff (non-player, non-coach) |
| [**listTeamMembersTeamMembersGet**](TeamMembersApi.md#listteammembersteammembersget) | **GET** /team-members | List all team members |
| [**updateTeamMemberTeamMembersMemberIdPatch**](TeamMembersApi.md#updateteammemberteammembersmemberidpatch) | **PATCH** /team-members/{member_id} | Update a team member |



## createTeamMemberTeamMembersPost

> ResponseCreateTeamMemberTeamMembersPost createTeamMemberTeamMembersPost(member)

Create a new team member

Add a new team member to a team.  The request body is a **union type (oneOf)** - you must include the &#x60;member_type&#x60; discriminator field: - &#x60;\&quot;member_type\&quot;: \&quot;player\&quot;&#x60; - Creates a player (requires position, jersey_number, etc.) - &#x60;\&quot;member_type\&quot;: \&quot;coach\&quot;&#x60; - Creates a coach (requires specialty, etc.) - &#x60;\&quot;member_type\&quot;: \&quot;medical_staff\&quot;&#x60; - Creates medical staff (requires medical specialty, etc.) - &#x60;\&quot;member_type\&quot;: \&quot;equipment_manager\&quot;&#x60; - Creates equipment manager (requires responsibilities, etc.)  The &#x60;character_id&#x60; field references an existing character from &#x60;/characters/{id}&#x60;.  **Example for creating a player:** &#x60;&#x60;&#x60;json {   \&quot;member_type\&quot;: \&quot;player\&quot;,   \&quot;character_id\&quot;: \&quot;sam-obisanya\&quot;,   \&quot;team_id\&quot;: \&quot;afc-richmond\&quot;,   \&quot;years_with_team\&quot;: 2,   \&quot;position\&quot;: \&quot;midfielder\&quot;,   \&quot;jersey_number\&quot;: 24,   \&quot;goals_scored\&quot;: 12,   \&quot;assists\&quot;: 15 } &#x60;&#x60;&#x60;

### Example

```ts
import {
  Configuration,
  TeamMembersApi,
} from '';
import type { CreateTeamMemberTeamMembersPostRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new TeamMembersApi(config);

  const body = {
    // Member
    member: ...,
  } satisfies CreateTeamMemberTeamMembersPostRequest;

  try {
    const data = await api.createTeamMemberTeamMembersPost(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **member** | [Member](Member.md) |  | |

### Return type

[**ResponseCreateTeamMemberTeamMembersPost**](ResponseCreateTeamMemberTeamMembersPost.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **201** | Team member created successfully |  -  |
| **409** | Team member already exists |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## deleteTeamMemberTeamMembersMemberIdDelete

> deleteTeamMemberTeamMembersMemberIdDelete(memberId)

Delete a team member

Remove a team member from the roster.

### Example

```ts
import {
  Configuration,
  TeamMembersApi,
} from '';
import type { DeleteTeamMemberTeamMembersMemberIdDeleteRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new TeamMembersApi(config);

  const body = {
    // string
    memberId: memberId_example,
  } satisfies DeleteTeamMemberTeamMembersMemberIdDeleteRequest;

  try {
    const data = await api.deleteTeamMemberTeamMembersMemberIdDelete(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **memberId** | `string` |  | [Defaults to `undefined`] |

### Return type

`void` (Empty response body)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **204** | Team member removed successfully |  -  |
| **404** | Team member not found |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## getTeamMemberTeamMembersMemberIdGet

> ResponseGetTeamMemberTeamMembersMemberIdGet getTeamMemberTeamMembersMemberIdGet(memberId)

Get a team member by ID

Retrieve detailed information about a specific team member.  The response is a **union type (oneOf)** - the actual shape depends on the member\&#39;s type: - **player**: Includes position, jersey_number, goals_scored, assists, is_captain - **coach**: Includes specialty, certifications, win_rate - **medical_staff**: Includes specialty, qualifications, license_number - **equipment_manager**: Includes responsibilities, is_head_kitman  Use &#x60;character_id&#x60; to fetch full character details from &#x60;/characters/{character_id}&#x60;.

### Example

```ts
import {
  Configuration,
  TeamMembersApi,
} from '';
import type { GetTeamMemberTeamMembersMemberIdGetRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new TeamMembersApi(config);

  const body = {
    // string
    memberId: memberId_example,
  } satisfies GetTeamMemberTeamMembersMemberIdGetRequest;

  try {
    const data = await api.getTeamMemberTeamMembersMemberIdGet(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **memberId** | `string` |  | [Defaults to `undefined`] |

### Return type

[**ResponseGetTeamMemberTeamMembersMemberIdGet**](ResponseGetTeamMemberTeamMembersMemberIdGet.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Team member details (oneOf based on member_type) |  -  |
| **404** | Team member not found |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## listCoachesTeamMembersCoachesGet

> PaginatedResponseCoach listCoachesTeamMembersCoachesGet(specialty, teamId, skip, limit)

List all coaches

Get only coaches (filtered subset of team members).

### Example

```ts
import {
  Configuration,
  TeamMembersApi,
} from '';
import type { ListCoachesTeamMembersCoachesGetRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new TeamMembersApi(config);

  const body = {
    // CoachSpecialty | Filter by specialty (optional)
    specialty: ...,
    // string | Filter by team ID (optional)
    teamId: teamId_example,
    // number | Number of items to skip (offset) (optional)
    skip: 56,
    // number | Maximum number of items to return (max: 100) (optional)
    limit: 56,
  } satisfies ListCoachesTeamMembersCoachesGetRequest;

  try {
    const data = await api.listCoachesTeamMembersCoachesGet(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **specialty** | `CoachSpecialty` | Filter by specialty | [Optional] [Defaults to `undefined`] [Enum: head_coach, assistant_coach, goalkeeping_coach, fitness_coach, tactical_analyst] |
| **teamId** | `string` | Filter by team ID | [Optional] [Defaults to `undefined`] |
| **skip** | `number` | Number of items to skip (offset) | [Optional] [Defaults to `0`] |
| **limit** | `number` | Maximum number of items to return (max: 100) | [Optional] [Defaults to `20`] |

### Return type

[**PaginatedResponseCoach**](PaginatedResponseCoach.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Successful Response |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## listPlayersTeamMembersPlayersGet

> PaginatedResponsePlayer listPlayersTeamMembersPlayersGet(position, teamId, skip, limit)

List all players

Get only players (filtered subset of team members).

### Example

```ts
import {
  Configuration,
  TeamMembersApi,
} from '';
import type { ListPlayersTeamMembersPlayersGetRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new TeamMembersApi(config);

  const body = {
    // Position | Filter by position (optional)
    position: ...,
    // string | Filter by team ID (optional)
    teamId: teamId_example,
    // number | Number of items to skip (offset) (optional)
    skip: 56,
    // number | Maximum number of items to return (max: 100) (optional)
    limit: 56,
  } satisfies ListPlayersTeamMembersPlayersGetRequest;

  try {
    const data = await api.listPlayersTeamMembersPlayersGet(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **position** | `Position` | Filter by position | [Optional] [Defaults to `undefined`] [Enum: goalkeeper, defender, midfielder, forward] |
| **teamId** | `string` | Filter by team ID | [Optional] [Defaults to `undefined`] |
| **skip** | `number` | Number of items to skip (offset) | [Optional] [Defaults to `0`] |
| **limit** | `number` | Maximum number of items to return (max: 100) | [Optional] [Defaults to `20`] |

### Return type

[**PaginatedResponsePlayer**](PaginatedResponsePlayer.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Successful Response |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## listStaffTeamMembersStaffGet

> PaginatedResponseUnionMedicalStaffEquipmentManager listStaffTeamMembersStaffGet(teamId, skip, limit)

List all staff (non-player, non-coach)

Get all staff members (medical staff and equipment managers).  This demonstrates a **narrower union type** - the response is oneOf MedicalStaff or EquipmentManager.

### Example

```ts
import {
  Configuration,
  TeamMembersApi,
} from '';
import type { ListStaffTeamMembersStaffGetRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new TeamMembersApi(config);

  const body = {
    // string | Filter by team ID (optional)
    teamId: teamId_example,
    // number | Number of items to skip (offset) (optional)
    skip: 56,
    // number | Maximum number of items to return (max: 100) (optional)
    limit: 56,
  } satisfies ListStaffTeamMembersStaffGetRequest;

  try {
    const data = await api.listStaffTeamMembersStaffGet(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **teamId** | `string` | Filter by team ID | [Optional] [Defaults to `undefined`] |
| **skip** | `number` | Number of items to skip (offset) | [Optional] [Defaults to `0`] |
| **limit** | `number` | Maximum number of items to return (max: 100) | [Optional] [Defaults to `20`] |

### Return type

[**PaginatedResponseUnionMedicalStaffEquipmentManager**](PaginatedResponseUnionMedicalStaffEquipmentManager.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Successful Response |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## listTeamMembersTeamMembersGet

> PaginatedResponseAnnotatedUnionPlayerCoachMedicalStaffEquipmentManagerFieldInfoAnnotationNoneTypeRequiredTrueDiscriminatorMemberType listTeamMembersTeamMembersGet(memberType, teamId, skip, limit)

List all team members

Get a paginated list of all team members.  This endpoint demonstrates **union types (oneOf)** in the response. Each team member can be one of: Player, Coach, MedicalStaff, or EquipmentManager. The &#x60;member_type&#x60; field acts as a discriminator to determine the shape of each object.

### Example

```ts
import {
  Configuration,
  TeamMembersApi,
} from '';
import type { ListTeamMembersTeamMembersGetRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new TeamMembersApi(config);

  const body = {
    // MemberType | Filter by member type (optional)
    memberType: ...,
    // string | Filter by team ID (optional)
    teamId: teamId_example,
    // number | Number of items to skip (offset) (optional)
    skip: 56,
    // number | Maximum number of items to return (max: 100) (optional)
    limit: 56,
  } satisfies ListTeamMembersTeamMembersGetRequest;

  try {
    const data = await api.listTeamMembersTeamMembersGet(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **memberType** | `MemberType` | Filter by member type | [Optional] [Defaults to `undefined`] [Enum: player, coach, medical_staff, equipment_manager] |
| **teamId** | `string` | Filter by team ID | [Optional] [Defaults to `undefined`] |
| **skip** | `number` | Number of items to skip (offset) | [Optional] [Defaults to `0`] |
| **limit** | `number` | Maximum number of items to return (max: 100) | [Optional] [Defaults to `20`] |

### Return type

[**PaginatedResponseAnnotatedUnionPlayerCoachMedicalStaffEquipmentManagerFieldInfoAnnotationNoneTypeRequiredTrueDiscriminatorMemberType**](PaginatedResponseAnnotatedUnionPlayerCoachMedicalStaffEquipmentManagerFieldInfoAnnotationNoneTypeRequiredTrueDiscriminatorMemberType.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Paginated list of team members (oneOf: Player, Coach, MedicalStaff, EquipmentManager) |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)


## updateTeamMemberTeamMembersMemberIdPatch

> ResponseUpdateTeamMemberTeamMembersMemberIdPatch updateTeamMemberTeamMembersMemberIdPatch(memberId, updates)

Update a team member

Update specific fields of an existing team member. Fields vary by member type.

### Example

```ts
import {
  Configuration,
  TeamMembersApi,
} from '';
import type { UpdateTeamMemberTeamMembersMemberIdPatchRequest } from '';

async function example() {
  console.log("🚀 Testing  SDK...");
  const config = new Configuration({ 
    // Configure HTTP bearer authorization: HTTPBearer
    accessToken: "YOUR BEARER TOKEN",
  });
  const api = new TeamMembersApi(config);

  const body = {
    // string
    memberId: memberId_example,
    // Updates
    updates: ...,
  } satisfies UpdateTeamMemberTeamMembersMemberIdPatchRequest;

  try {
    const data = await api.updateTeamMemberTeamMembersMemberIdPatch(body);
    console.log(data);
  } catch (error) {
    console.error(error);
  }
}

// Run the test
example().catch(console.error);
```

### Parameters


| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **memberId** | `string` |  | [Defaults to `undefined`] |
| **updates** | [Updates](Updates.md) |  | |

### Return type

[**ResponseUpdateTeamMemberTeamMembersMemberIdPatch**](ResponseUpdateTeamMemberTeamMembersMemberIdPatch.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | Team member updated successfully |  -  |
| **404** | Team member not found |  -  |
| **422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#api-endpoints) [[Back to Model list]](../README.md#models) [[Back to README]](../README.md)

