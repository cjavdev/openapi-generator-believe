# TeamMembersApi

All URIs are relative to *https://believe.cjav.dev*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createTeamMemberTeamMembersPost**](TeamMembersApi.md#createTeamMemberTeamMembersPost) | **POST** /team-members | Create a new team member |
| [**deleteTeamMemberTeamMembersMemberIdDelete**](TeamMembersApi.md#deleteTeamMemberTeamMembersMemberIdDelete) | **DELETE** /team-members/{member_id} | Delete a team member |
| [**getTeamMemberTeamMembersMemberIdGet**](TeamMembersApi.md#getTeamMemberTeamMembersMemberIdGet) | **GET** /team-members/{member_id} | Get a team member by ID |
| [**listCoachesTeamMembersCoachesGet**](TeamMembersApi.md#listCoachesTeamMembersCoachesGet) | **GET** /team-members/coaches/ | List all coaches |
| [**listPlayersTeamMembersPlayersGet**](TeamMembersApi.md#listPlayersTeamMembersPlayersGet) | **GET** /team-members/players/ | List all players |
| [**listStaffTeamMembersStaffGet**](TeamMembersApi.md#listStaffTeamMembersStaffGet) | **GET** /team-members/staff/ | List all staff (non-player, non-coach) |
| [**listTeamMembersTeamMembersGet**](TeamMembersApi.md#listTeamMembersTeamMembersGet) | **GET** /team-members | List all team members |
| [**updateTeamMemberTeamMembersMemberIdPatch**](TeamMembersApi.md#updateTeamMemberTeamMembersMemberIdPatch) | **PATCH** /team-members/{member_id} | Update a team member |


<a id="createTeamMemberTeamMembersPost"></a>
# **createTeamMemberTeamMembersPost**
> ResponseCreateTeamMemberTeamMembersPost createTeamMemberTeamMembersPost(member)

Create a new team member

Add a new team member to a team.  The request body is a **union type (oneOf)** - you must include the &#x60;member_type&#x60; discriminator field: - &#x60;\&quot;member_type\&quot;: \&quot;player\&quot;&#x60; - Creates a player (requires position, jersey_number, etc.) - &#x60;\&quot;member_type\&quot;: \&quot;coach\&quot;&#x60; - Creates a coach (requires specialty, etc.) - &#x60;\&quot;member_type\&quot;: \&quot;medical_staff\&quot;&#x60; - Creates medical staff (requires medical specialty, etc.) - &#x60;\&quot;member_type\&quot;: \&quot;equipment_manager\&quot;&#x60; - Creates equipment manager (requires responsibilities, etc.)  The &#x60;character_id&#x60; field references an existing character from &#x60;/characters/{id}&#x60;.  **Example for creating a player:** &#x60;&#x60;&#x60;json {   \&quot;member_type\&quot;: \&quot;player\&quot;,   \&quot;character_id\&quot;: \&quot;sam-obisanya\&quot;,   \&quot;team_id\&quot;: \&quot;afc-richmond\&quot;,   \&quot;years_with_team\&quot;: 2,   \&quot;position\&quot;: \&quot;midfielder\&quot;,   \&quot;jersey_number\&quot;: 24,   \&quot;goals_scored\&quot;: 12,   \&quot;assists\&quot;: 15 } &#x60;&#x60;&#x60;

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = TeamMembersApi()
val member : Member =  // Member | 
try {
    val result : ResponseCreateTeamMemberTeamMembersPost = apiInstance.createTeamMemberTeamMembersPost(member)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TeamMembersApi#createTeamMemberTeamMembersPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TeamMembersApi#createTeamMemberTeamMembersPost")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **member** | [**Member**](Member.md)|  | |

### Return type

[**ResponseCreateTeamMemberTeamMembersPost**](ResponseCreateTeamMemberTeamMembersPost.md)

### Authorization


Configure HTTPBearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="deleteTeamMemberTeamMembersMemberIdDelete"></a>
# **deleteTeamMemberTeamMembersMemberIdDelete**
> deleteTeamMemberTeamMembersMemberIdDelete(memberId)

Delete a team member

Remove a team member from the roster.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = TeamMembersApi()
val memberId : kotlin.String = memberId_example // kotlin.String | 
try {
    apiInstance.deleteTeamMemberTeamMembersMemberIdDelete(memberId)
} catch (e: ClientException) {
    println("4xx response calling TeamMembersApi#deleteTeamMemberTeamMembersMemberIdDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TeamMembersApi#deleteTeamMemberTeamMembersMemberIdDelete")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **memberId** | **kotlin.String**|  | |

### Return type

null (empty response body)

### Authorization


Configure HTTPBearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="getTeamMemberTeamMembersMemberIdGet"></a>
# **getTeamMemberTeamMembersMemberIdGet**
> ResponseGetTeamMemberTeamMembersMemberIdGet getTeamMemberTeamMembersMemberIdGet(memberId)

Get a team member by ID

Retrieve detailed information about a specific team member.  The response is a **union type (oneOf)** - the actual shape depends on the member&#39;s type: - **player**: Includes position, jersey_number, goals_scored, assists, is_captain - **coach**: Includes specialty, certifications, win_rate - **medical_staff**: Includes specialty, qualifications, license_number - **equipment_manager**: Includes responsibilities, is_head_kitman  Use &#x60;character_id&#x60; to fetch full character details from &#x60;/characters/{character_id}&#x60;.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = TeamMembersApi()
val memberId : kotlin.String = memberId_example // kotlin.String | 
try {
    val result : ResponseGetTeamMemberTeamMembersMemberIdGet = apiInstance.getTeamMemberTeamMembersMemberIdGet(memberId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TeamMembersApi#getTeamMemberTeamMembersMemberIdGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TeamMembersApi#getTeamMemberTeamMembersMemberIdGet")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **memberId** | **kotlin.String**|  | |

### Return type

[**ResponseGetTeamMemberTeamMembersMemberIdGet**](ResponseGetTeamMemberTeamMembersMemberIdGet.md)

### Authorization


Configure HTTPBearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="listCoachesTeamMembersCoachesGet"></a>
# **listCoachesTeamMembersCoachesGet**
> PaginatedResponseCoach listCoachesTeamMembersCoachesGet(specialty, teamId, skip, limit)

List all coaches

Get only coaches (filtered subset of team members).

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = TeamMembersApi()
val specialty : CoachSpecialty =  // CoachSpecialty | Filter by specialty
val teamId : kotlin.String = teamId_example // kotlin.String | Filter by team ID
val skip : kotlin.Int = 56 // kotlin.Int | Number of items to skip (offset)
val limit : kotlin.Int = 56 // kotlin.Int | Maximum number of items to return (max: 100)
try {
    val result : PaginatedResponseCoach = apiInstance.listCoachesTeamMembersCoachesGet(specialty, teamId, skip, limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TeamMembersApi#listCoachesTeamMembersCoachesGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TeamMembersApi#listCoachesTeamMembersCoachesGet")
    e.printStackTrace()
}
```

### Parameters
| **specialty** | [**CoachSpecialty**](.md)| Filter by specialty | [optional] [enum: head_coach, assistant_coach, goalkeeping_coach, fitness_coach, tactical_analyst] |
| **teamId** | **kotlin.String**| Filter by team ID | [optional] |
| **skip** | **kotlin.Int**| Number of items to skip (offset) | [optional] [default to 0] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.Int**| Maximum number of items to return (max: 100) | [optional] [default to 20] |

### Return type

[**PaginatedResponseCoach**](PaginatedResponseCoach.md)

### Authorization


Configure HTTPBearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="listPlayersTeamMembersPlayersGet"></a>
# **listPlayersTeamMembersPlayersGet**
> PaginatedResponsePlayer listPlayersTeamMembersPlayersGet(position, teamId, skip, limit)

List all players

Get only players (filtered subset of team members).

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = TeamMembersApi()
val position : Position =  // Position | Filter by position
val teamId : kotlin.String = teamId_example // kotlin.String | Filter by team ID
val skip : kotlin.Int = 56 // kotlin.Int | Number of items to skip (offset)
val limit : kotlin.Int = 56 // kotlin.Int | Maximum number of items to return (max: 100)
try {
    val result : PaginatedResponsePlayer = apiInstance.listPlayersTeamMembersPlayersGet(position, teamId, skip, limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TeamMembersApi#listPlayersTeamMembersPlayersGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TeamMembersApi#listPlayersTeamMembersPlayersGet")
    e.printStackTrace()
}
```

### Parameters
| **position** | [**Position**](.md)| Filter by position | [optional] [enum: goalkeeper, defender, midfielder, forward] |
| **teamId** | **kotlin.String**| Filter by team ID | [optional] |
| **skip** | **kotlin.Int**| Number of items to skip (offset) | [optional] [default to 0] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.Int**| Maximum number of items to return (max: 100) | [optional] [default to 20] |

### Return type

[**PaginatedResponsePlayer**](PaginatedResponsePlayer.md)

### Authorization


Configure HTTPBearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="listStaffTeamMembersStaffGet"></a>
# **listStaffTeamMembersStaffGet**
> PaginatedResponseUnionMedicalStaffEquipmentManager listStaffTeamMembersStaffGet(teamId, skip, limit)

List all staff (non-player, non-coach)

Get all staff members (medical staff and equipment managers).  This demonstrates a **narrower union type** - the response is oneOf MedicalStaff or EquipmentManager.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = TeamMembersApi()
val teamId : kotlin.String = teamId_example // kotlin.String | Filter by team ID
val skip : kotlin.Int = 56 // kotlin.Int | Number of items to skip (offset)
val limit : kotlin.Int = 56 // kotlin.Int | Maximum number of items to return (max: 100)
try {
    val result : PaginatedResponseUnionMedicalStaffEquipmentManager = apiInstance.listStaffTeamMembersStaffGet(teamId, skip, limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TeamMembersApi#listStaffTeamMembersStaffGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TeamMembersApi#listStaffTeamMembersStaffGet")
    e.printStackTrace()
}
```

### Parameters
| **teamId** | **kotlin.String**| Filter by team ID | [optional] |
| **skip** | **kotlin.Int**| Number of items to skip (offset) | [optional] [default to 0] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.Int**| Maximum number of items to return (max: 100) | [optional] [default to 20] |

### Return type

[**PaginatedResponseUnionMedicalStaffEquipmentManager**](PaginatedResponseUnionMedicalStaffEquipmentManager.md)

### Authorization


Configure HTTPBearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="listTeamMembersTeamMembersGet"></a>
# **listTeamMembersTeamMembersGet**
> PaginatedResponseAnnotatedUnionPlayerCoachMedicalStaffEquipmentManagerFieldInfoAnnotationNoneTypeRequiredTrueDiscriminatorMemberType listTeamMembersTeamMembersGet(memberType, teamId, skip, limit)

List all team members

Get a paginated list of all team members.  This endpoint demonstrates **union types (oneOf)** in the response. Each team member can be one of: Player, Coach, MedicalStaff, or EquipmentManager. The &#x60;member_type&#x60; field acts as a discriminator to determine the shape of each object.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = TeamMembersApi()
val memberType : MemberType =  // MemberType | Filter by member type
val teamId : kotlin.String = teamId_example // kotlin.String | Filter by team ID
val skip : kotlin.Int = 56 // kotlin.Int | Number of items to skip (offset)
val limit : kotlin.Int = 56 // kotlin.Int | Maximum number of items to return (max: 100)
try {
    val result : PaginatedResponseAnnotatedUnionPlayerCoachMedicalStaffEquipmentManagerFieldInfoAnnotationNoneTypeRequiredTrueDiscriminatorMemberType = apiInstance.listTeamMembersTeamMembersGet(memberType, teamId, skip, limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TeamMembersApi#listTeamMembersTeamMembersGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TeamMembersApi#listTeamMembersTeamMembersGet")
    e.printStackTrace()
}
```

### Parameters
| **memberType** | [**MemberType**](.md)| Filter by member type | [optional] [enum: player, coach, medical_staff, equipment_manager] |
| **teamId** | **kotlin.String**| Filter by team ID | [optional] |
| **skip** | **kotlin.Int**| Number of items to skip (offset) | [optional] [default to 0] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.Int**| Maximum number of items to return (max: 100) | [optional] [default to 20] |

### Return type

[**PaginatedResponseAnnotatedUnionPlayerCoachMedicalStaffEquipmentManagerFieldInfoAnnotationNoneTypeRequiredTrueDiscriminatorMemberType**](PaginatedResponseAnnotatedUnionPlayerCoachMedicalStaffEquipmentManagerFieldInfoAnnotationNoneTypeRequiredTrueDiscriminatorMemberType.md)

### Authorization


Configure HTTPBearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="updateTeamMemberTeamMembersMemberIdPatch"></a>
# **updateTeamMemberTeamMembersMemberIdPatch**
> ResponseUpdateTeamMemberTeamMembersMemberIdPatch updateTeamMemberTeamMembersMemberIdPatch(memberId, updates)

Update a team member

Update specific fields of an existing team member. Fields vary by member type.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = TeamMembersApi()
val memberId : kotlin.String = memberId_example // kotlin.String | 
val updates : Updates =  // Updates | 
try {
    val result : ResponseUpdateTeamMemberTeamMembersMemberIdPatch = apiInstance.updateTeamMemberTeamMembersMemberIdPatch(memberId, updates)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TeamMembersApi#updateTeamMemberTeamMembersMemberIdPatch")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TeamMembersApi#updateTeamMemberTeamMembersMemberIdPatch")
    e.printStackTrace()
}
```

### Parameters
| **memberId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **updates** | [**Updates**](Updates.md)|  | |

### Return type

[**ResponseUpdateTeamMemberTeamMembersMemberIdPatch**](ResponseUpdateTeamMemberTeamMembersMemberIdPatch.md)

### Authorization


Configure HTTPBearer:
    ApiClient.accessToken = ""

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

