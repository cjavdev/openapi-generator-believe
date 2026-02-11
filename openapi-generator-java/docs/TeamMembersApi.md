# TeamMembersApi

All URIs are relative to *https://believe.cjav.dev*

| Method | HTTP request | Description |
|------------- | ------------- | -------------|
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
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.TeamMembersApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://believe.cjav.dev");
    
    // Configure HTTP bearer authorization: HTTPBearer
    HttpBearerAuth HTTPBearer = (HttpBearerAuth) defaultClient.getAuthentication("HTTPBearer");
    HTTPBearer.setBearerToken("BEARER TOKEN");

    TeamMembersApi apiInstance = new TeamMembersApi(defaultClient);
    Member member = new Member(); // Member | 
    try {
      ResponseCreateTeamMemberTeamMembersPost result = apiInstance.createTeamMemberTeamMembersPost(member);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling TeamMembersApi#createTeamMemberTeamMembersPost");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **member** | [**Member**](Member.md)|  | |

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

<a id="deleteTeamMemberTeamMembersMemberIdDelete"></a>
# **deleteTeamMemberTeamMembersMemberIdDelete**
> deleteTeamMemberTeamMembersMemberIdDelete(memberId)

Delete a team member

Remove a team member from the roster.

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.TeamMembersApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://believe.cjav.dev");
    
    // Configure HTTP bearer authorization: HTTPBearer
    HttpBearerAuth HTTPBearer = (HttpBearerAuth) defaultClient.getAuthentication("HTTPBearer");
    HTTPBearer.setBearerToken("BEARER TOKEN");

    TeamMembersApi apiInstance = new TeamMembersApi(defaultClient);
    String memberId = "memberId_example"; // String | 
    try {
      apiInstance.deleteTeamMemberTeamMembersMemberIdDelete(memberId);
    } catch (ApiException e) {
      System.err.println("Exception when calling TeamMembersApi#deleteTeamMemberTeamMembersMemberIdDelete");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **memberId** | **String**|  | |

### Return type

null (empty response body)

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

<a id="getTeamMemberTeamMembersMemberIdGet"></a>
# **getTeamMemberTeamMembersMemberIdGet**
> ResponseGetTeamMemberTeamMembersMemberIdGet getTeamMemberTeamMembersMemberIdGet(memberId)

Get a team member by ID

Retrieve detailed information about a specific team member.  The response is a **union type (oneOf)** - the actual shape depends on the member&#39;s type: - **player**: Includes position, jersey_number, goals_scored, assists, is_captain - **coach**: Includes specialty, certifications, win_rate - **medical_staff**: Includes specialty, qualifications, license_number - **equipment_manager**: Includes responsibilities, is_head_kitman  Use &#x60;character_id&#x60; to fetch full character details from &#x60;/characters/{character_id}&#x60;.

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.TeamMembersApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://believe.cjav.dev");
    
    // Configure HTTP bearer authorization: HTTPBearer
    HttpBearerAuth HTTPBearer = (HttpBearerAuth) defaultClient.getAuthentication("HTTPBearer");
    HTTPBearer.setBearerToken("BEARER TOKEN");

    TeamMembersApi apiInstance = new TeamMembersApi(defaultClient);
    String memberId = "memberId_example"; // String | 
    try {
      ResponseGetTeamMemberTeamMembersMemberIdGet result = apiInstance.getTeamMemberTeamMembersMemberIdGet(memberId);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling TeamMembersApi#getTeamMemberTeamMembersMemberIdGet");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **memberId** | **String**|  | |

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

<a id="listCoachesTeamMembersCoachesGet"></a>
# **listCoachesTeamMembersCoachesGet**
> PaginatedResponseCoach listCoachesTeamMembersCoachesGet(specialty, teamId, skip, limit)

List all coaches

Get only coaches (filtered subset of team members).

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.TeamMembersApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://believe.cjav.dev");
    
    // Configure HTTP bearer authorization: HTTPBearer
    HttpBearerAuth HTTPBearer = (HttpBearerAuth) defaultClient.getAuthentication("HTTPBearer");
    HTTPBearer.setBearerToken("BEARER TOKEN");

    TeamMembersApi apiInstance = new TeamMembersApi(defaultClient);
    CoachSpecialty specialty = CoachSpecialty.fromValue("head_coach"); // CoachSpecialty | Filter by specialty
    String teamId = "teamId_example"; // String | Filter by team ID
    Integer skip = 0; // Integer | Number of items to skip (offset)
    Integer limit = 20; // Integer | Maximum number of items to return (max: 100)
    try {
      PaginatedResponseCoach result = apiInstance.listCoachesTeamMembersCoachesGet(specialty, teamId, skip, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling TeamMembersApi#listCoachesTeamMembersCoachesGet");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **specialty** | [**CoachSpecialty**](.md)| Filter by specialty | [optional] [enum: head_coach, assistant_coach, goalkeeping_coach, fitness_coach, tactical_analyst] |
| **teamId** | **String**| Filter by team ID | [optional] |
| **skip** | **Integer**| Number of items to skip (offset) | [optional] [default to 0] |
| **limit** | **Integer**| Maximum number of items to return (max: 100) | [optional] [default to 20] |

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

<a id="listPlayersTeamMembersPlayersGet"></a>
# **listPlayersTeamMembersPlayersGet**
> PaginatedResponsePlayer listPlayersTeamMembersPlayersGet(position, teamId, skip, limit)

List all players

Get only players (filtered subset of team members).

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.TeamMembersApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://believe.cjav.dev");
    
    // Configure HTTP bearer authorization: HTTPBearer
    HttpBearerAuth HTTPBearer = (HttpBearerAuth) defaultClient.getAuthentication("HTTPBearer");
    HTTPBearer.setBearerToken("BEARER TOKEN");

    TeamMembersApi apiInstance = new TeamMembersApi(defaultClient);
    Position position = Position.fromValue("goalkeeper"); // Position | Filter by position
    String teamId = "teamId_example"; // String | Filter by team ID
    Integer skip = 0; // Integer | Number of items to skip (offset)
    Integer limit = 20; // Integer | Maximum number of items to return (max: 100)
    try {
      PaginatedResponsePlayer result = apiInstance.listPlayersTeamMembersPlayersGet(position, teamId, skip, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling TeamMembersApi#listPlayersTeamMembersPlayersGet");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **position** | [**Position**](.md)| Filter by position | [optional] [enum: goalkeeper, defender, midfielder, forward] |
| **teamId** | **String**| Filter by team ID | [optional] |
| **skip** | **Integer**| Number of items to skip (offset) | [optional] [default to 0] |
| **limit** | **Integer**| Maximum number of items to return (max: 100) | [optional] [default to 20] |

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

<a id="listStaffTeamMembersStaffGet"></a>
# **listStaffTeamMembersStaffGet**
> PaginatedResponseUnionMedicalStaffEquipmentManager listStaffTeamMembersStaffGet(teamId, skip, limit)

List all staff (non-player, non-coach)

Get all staff members (medical staff and equipment managers).  This demonstrates a **narrower union type** - the response is oneOf MedicalStaff or EquipmentManager.

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.TeamMembersApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://believe.cjav.dev");
    
    // Configure HTTP bearer authorization: HTTPBearer
    HttpBearerAuth HTTPBearer = (HttpBearerAuth) defaultClient.getAuthentication("HTTPBearer");
    HTTPBearer.setBearerToken("BEARER TOKEN");

    TeamMembersApi apiInstance = new TeamMembersApi(defaultClient);
    String teamId = "teamId_example"; // String | Filter by team ID
    Integer skip = 0; // Integer | Number of items to skip (offset)
    Integer limit = 20; // Integer | Maximum number of items to return (max: 100)
    try {
      PaginatedResponseUnionMedicalStaffEquipmentManager result = apiInstance.listStaffTeamMembersStaffGet(teamId, skip, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling TeamMembersApi#listStaffTeamMembersStaffGet");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **teamId** | **String**| Filter by team ID | [optional] |
| **skip** | **Integer**| Number of items to skip (offset) | [optional] [default to 0] |
| **limit** | **Integer**| Maximum number of items to return (max: 100) | [optional] [default to 20] |

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

<a id="listTeamMembersTeamMembersGet"></a>
# **listTeamMembersTeamMembersGet**
> PaginatedResponseAnnotatedUnionPlayerCoachMedicalStaffEquipmentManagerFieldInfoAnnotationNoneTypeRequiredTrueDiscriminatorMemberType listTeamMembersTeamMembersGet(memberType, teamId, skip, limit)

List all team members

Get a paginated list of all team members.  This endpoint demonstrates **union types (oneOf)** in the response. Each team member can be one of: Player, Coach, MedicalStaff, or EquipmentManager. The &#x60;member_type&#x60; field acts as a discriminator to determine the shape of each object.

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.TeamMembersApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://believe.cjav.dev");
    
    // Configure HTTP bearer authorization: HTTPBearer
    HttpBearerAuth HTTPBearer = (HttpBearerAuth) defaultClient.getAuthentication("HTTPBearer");
    HTTPBearer.setBearerToken("BEARER TOKEN");

    TeamMembersApi apiInstance = new TeamMembersApi(defaultClient);
    MemberType memberType = MemberType.fromValue("player"); // MemberType | Filter by member type
    String teamId = "teamId_example"; // String | Filter by team ID
    Integer skip = 0; // Integer | Number of items to skip (offset)
    Integer limit = 20; // Integer | Maximum number of items to return (max: 100)
    try {
      PaginatedResponseAnnotatedUnionPlayerCoachMedicalStaffEquipmentManagerFieldInfoAnnotationNoneTypeRequiredTrueDiscriminatorMemberType result = apiInstance.listTeamMembersTeamMembersGet(memberType, teamId, skip, limit);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling TeamMembersApi#listTeamMembersTeamMembersGet");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **memberType** | [**MemberType**](.md)| Filter by member type | [optional] [enum: player, coach, medical_staff, equipment_manager] |
| **teamId** | **String**| Filter by team ID | [optional] |
| **skip** | **Integer**| Number of items to skip (offset) | [optional] [default to 0] |
| **limit** | **Integer**| Maximum number of items to return (max: 100) | [optional] [default to 20] |

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

<a id="updateTeamMemberTeamMembersMemberIdPatch"></a>
# **updateTeamMemberTeamMembersMemberIdPatch**
> ResponseUpdateTeamMemberTeamMembersMemberIdPatch updateTeamMemberTeamMembersMemberIdPatch(memberId, updates)

Update a team member

Update specific fields of an existing team member. Fields vary by member type.

### Example
```java
// Import classes:
import org.openapitools.client.ApiClient;
import org.openapitools.client.ApiException;
import org.openapitools.client.Configuration;
import org.openapitools.client.auth.*;
import org.openapitools.client.models.*;
import org.openapitools.client.api.TeamMembersApi;

public class Example {
  public static void main(String[] args) {
    ApiClient defaultClient = Configuration.getDefaultApiClient();
    defaultClient.setBasePath("https://believe.cjav.dev");
    
    // Configure HTTP bearer authorization: HTTPBearer
    HttpBearerAuth HTTPBearer = (HttpBearerAuth) defaultClient.getAuthentication("HTTPBearer");
    HTTPBearer.setBearerToken("BEARER TOKEN");

    TeamMembersApi apiInstance = new TeamMembersApi(defaultClient);
    String memberId = "memberId_example"; // String | 
    Updates updates = new Updates(); // Updates | 
    try {
      ResponseUpdateTeamMemberTeamMembersMemberIdPatch result = apiInstance.updateTeamMemberTeamMembersMemberIdPatch(memberId, updates);
      System.out.println(result);
    } catch (ApiException e) {
      System.err.println("Exception when calling TeamMembersApi#updateTeamMemberTeamMembersMemberIdPatch");
      System.err.println("Status code: " + e.getCode());
      System.err.println("Reason: " + e.getResponseBody());
      System.err.println("Response headers: " + e.getResponseHeaders());
      e.printStackTrace();
    }
  }
}
```

### Parameters

| Name | Type | Description  | Notes |
|------------- | ------------- | ------------- | -------------|
| **memberId** | **String**|  | |
| **updates** | [**Updates**](Updates.md)|  | |

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

