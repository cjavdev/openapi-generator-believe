# \TeamMembersAPI

All URIs are relative to *https://believe.cjav.dev*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateTeamMemberTeamMembersPost**](TeamMembersAPI.md#CreateTeamMemberTeamMembersPost) | **Post** /team-members | Create a new team member
[**DeleteTeamMemberTeamMembersMemberIdDelete**](TeamMembersAPI.md#DeleteTeamMemberTeamMembersMemberIdDelete) | **Delete** /team-members/{member_id} | Delete a team member
[**GetTeamMemberTeamMembersMemberIdGet**](TeamMembersAPI.md#GetTeamMemberTeamMembersMemberIdGet) | **Get** /team-members/{member_id} | Get a team member by ID
[**ListCoachesTeamMembersCoachesGet**](TeamMembersAPI.md#ListCoachesTeamMembersCoachesGet) | **Get** /team-members/coaches/ | List all coaches
[**ListPlayersTeamMembersPlayersGet**](TeamMembersAPI.md#ListPlayersTeamMembersPlayersGet) | **Get** /team-members/players/ | List all players
[**ListStaffTeamMembersStaffGet**](TeamMembersAPI.md#ListStaffTeamMembersStaffGet) | **Get** /team-members/staff/ | List all staff (non-player, non-coach)
[**ListTeamMembersTeamMembersGet**](TeamMembersAPI.md#ListTeamMembersTeamMembersGet) | **Get** /team-members | List all team members
[**UpdateTeamMemberTeamMembersMemberIdPatch**](TeamMembersAPI.md#UpdateTeamMemberTeamMembersMemberIdPatch) | **Patch** /team-members/{member_id} | Update a team member



## CreateTeamMemberTeamMembersPost

> ResponseCreateTeamMemberTeamMembersPost CreateTeamMemberTeamMembersPost(ctx).Member(member).Execute()

Create a new team member



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	member := openapiclient.Member{CoachBase: openapiclient.NewCoachBase("jamie-tartt", openapiclient.CoachSpecialty("head_coach"), "afc-richmond", int32(3))} // Member | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TeamMembersAPI.CreateTeamMemberTeamMembersPost(context.Background()).Member(member).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TeamMembersAPI.CreateTeamMemberTeamMembersPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateTeamMemberTeamMembersPost`: ResponseCreateTeamMemberTeamMembersPost
	fmt.Fprintf(os.Stdout, "Response from `TeamMembersAPI.CreateTeamMemberTeamMembersPost`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateTeamMemberTeamMembersPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **member** | [**Member**](Member.md) |  | 

### Return type

[**ResponseCreateTeamMemberTeamMembersPost**](ResponseCreateTeamMemberTeamMembersPost.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteTeamMemberTeamMembersMemberIdDelete

> DeleteTeamMemberTeamMembersMemberIdDelete(ctx, memberId).Execute()

Delete a team member



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	memberId := "memberId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.TeamMembersAPI.DeleteTeamMemberTeamMembersMemberIdDelete(context.Background(), memberId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TeamMembersAPI.DeleteTeamMemberTeamMembersMemberIdDelete``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**memberId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteTeamMemberTeamMembersMemberIdDeleteRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

 (empty response body)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetTeamMemberTeamMembersMemberIdGet

> ResponseGetTeamMemberTeamMembersMemberIdGet GetTeamMemberTeamMembersMemberIdGet(ctx, memberId).Execute()

Get a team member by ID



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	memberId := "memberId_example" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TeamMembersAPI.GetTeamMemberTeamMembersMemberIdGet(context.Background(), memberId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TeamMembersAPI.GetTeamMemberTeamMembersMemberIdGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetTeamMemberTeamMembersMemberIdGet`: ResponseGetTeamMemberTeamMembersMemberIdGet
	fmt.Fprintf(os.Stdout, "Response from `TeamMembersAPI.GetTeamMemberTeamMembersMemberIdGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**memberId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetTeamMemberTeamMembersMemberIdGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**ResponseGetTeamMemberTeamMembersMemberIdGet**](ResponseGetTeamMemberTeamMembersMemberIdGet.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListCoachesTeamMembersCoachesGet

> PaginatedResponseCoach ListCoachesTeamMembersCoachesGet(ctx).Specialty(specialty).TeamId(teamId).Skip(skip).Limit(limit).Execute()

List all coaches



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	specialty := openapiclient.CoachSpecialty("head_coach") // CoachSpecialty | Filter by specialty (optional)
	teamId := "teamId_example" // string | Filter by team ID (optional)
	skip := int32(56) // int32 | Number of items to skip (offset) (optional) (default to 0)
	limit := int32(56) // int32 | Maximum number of items to return (max: 100) (optional) (default to 20)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TeamMembersAPI.ListCoachesTeamMembersCoachesGet(context.Background()).Specialty(specialty).TeamId(teamId).Skip(skip).Limit(limit).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TeamMembersAPI.ListCoachesTeamMembersCoachesGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListCoachesTeamMembersCoachesGet`: PaginatedResponseCoach
	fmt.Fprintf(os.Stdout, "Response from `TeamMembersAPI.ListCoachesTeamMembersCoachesGet`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListCoachesTeamMembersCoachesGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **specialty** | [**CoachSpecialty**](CoachSpecialty.md) | Filter by specialty | 
 **teamId** | **string** | Filter by team ID | 
 **skip** | **int32** | Number of items to skip (offset) | [default to 0]
 **limit** | **int32** | Maximum number of items to return (max: 100) | [default to 20]

### Return type

[**PaginatedResponseCoach**](PaginatedResponseCoach.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListPlayersTeamMembersPlayersGet

> PaginatedResponsePlayer ListPlayersTeamMembersPlayersGet(ctx).Position(position).TeamId(teamId).Skip(skip).Limit(limit).Execute()

List all players



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	position := openapiclient.Position("goalkeeper") // Position | Filter by position (optional)
	teamId := "teamId_example" // string | Filter by team ID (optional)
	skip := int32(56) // int32 | Number of items to skip (offset) (optional) (default to 0)
	limit := int32(56) // int32 | Maximum number of items to return (max: 100) (optional) (default to 20)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TeamMembersAPI.ListPlayersTeamMembersPlayersGet(context.Background()).Position(position).TeamId(teamId).Skip(skip).Limit(limit).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TeamMembersAPI.ListPlayersTeamMembersPlayersGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListPlayersTeamMembersPlayersGet`: PaginatedResponsePlayer
	fmt.Fprintf(os.Stdout, "Response from `TeamMembersAPI.ListPlayersTeamMembersPlayersGet`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListPlayersTeamMembersPlayersGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **position** | [**Position**](Position.md) | Filter by position | 
 **teamId** | **string** | Filter by team ID | 
 **skip** | **int32** | Number of items to skip (offset) | [default to 0]
 **limit** | **int32** | Maximum number of items to return (max: 100) | [default to 20]

### Return type

[**PaginatedResponsePlayer**](PaginatedResponsePlayer.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListStaffTeamMembersStaffGet

> PaginatedResponseUnionMedicalStaffEquipmentManager ListStaffTeamMembersStaffGet(ctx).TeamId(teamId).Skip(skip).Limit(limit).Execute()

List all staff (non-player, non-coach)



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	teamId := "teamId_example" // string | Filter by team ID (optional)
	skip := int32(56) // int32 | Number of items to skip (offset) (optional) (default to 0)
	limit := int32(56) // int32 | Maximum number of items to return (max: 100) (optional) (default to 20)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TeamMembersAPI.ListStaffTeamMembersStaffGet(context.Background()).TeamId(teamId).Skip(skip).Limit(limit).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TeamMembersAPI.ListStaffTeamMembersStaffGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListStaffTeamMembersStaffGet`: PaginatedResponseUnionMedicalStaffEquipmentManager
	fmt.Fprintf(os.Stdout, "Response from `TeamMembersAPI.ListStaffTeamMembersStaffGet`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListStaffTeamMembersStaffGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **teamId** | **string** | Filter by team ID | 
 **skip** | **int32** | Number of items to skip (offset) | [default to 0]
 **limit** | **int32** | Maximum number of items to return (max: 100) | [default to 20]

### Return type

[**PaginatedResponseUnionMedicalStaffEquipmentManager**](PaginatedResponseUnionMedicalStaffEquipmentManager.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListTeamMembersTeamMembersGet

> PaginatedResponseAnnotatedUnionPlayerCoachMedicalStaffEquipmentManagerFieldInfoAnnotationNoneTypeRequiredTrueDiscriminatorMemberType ListTeamMembersTeamMembersGet(ctx).MemberType(memberType).TeamId(teamId).Skip(skip).Limit(limit).Execute()

List all team members



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	memberType := openapiclient.MemberType("player") // MemberType | Filter by member type (optional)
	teamId := "teamId_example" // string | Filter by team ID (optional)
	skip := int32(56) // int32 | Number of items to skip (offset) (optional) (default to 0)
	limit := int32(56) // int32 | Maximum number of items to return (max: 100) (optional) (default to 20)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TeamMembersAPI.ListTeamMembersTeamMembersGet(context.Background()).MemberType(memberType).TeamId(teamId).Skip(skip).Limit(limit).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TeamMembersAPI.ListTeamMembersTeamMembersGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListTeamMembersTeamMembersGet`: PaginatedResponseAnnotatedUnionPlayerCoachMedicalStaffEquipmentManagerFieldInfoAnnotationNoneTypeRequiredTrueDiscriminatorMemberType
	fmt.Fprintf(os.Stdout, "Response from `TeamMembersAPI.ListTeamMembersTeamMembersGet`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListTeamMembersTeamMembersGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **memberType** | [**MemberType**](MemberType.md) | Filter by member type | 
 **teamId** | **string** | Filter by team ID | 
 **skip** | **int32** | Number of items to skip (offset) | [default to 0]
 **limit** | **int32** | Maximum number of items to return (max: 100) | [default to 20]

### Return type

[**PaginatedResponseAnnotatedUnionPlayerCoachMedicalStaffEquipmentManagerFieldInfoAnnotationNoneTypeRequiredTrueDiscriminatorMemberType**](PaginatedResponseAnnotatedUnionPlayerCoachMedicalStaffEquipmentManagerFieldInfoAnnotationNoneTypeRequiredTrueDiscriminatorMemberType.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateTeamMemberTeamMembersMemberIdPatch

> ResponseUpdateTeamMemberTeamMembersMemberIdPatch UpdateTeamMemberTeamMembersMemberIdPatch(ctx, memberId).Updates(updates).Execute()

Update a team member



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	memberId := "memberId_example" // string | 
	updates := *openapiclient.NewUpdates() // Updates | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.TeamMembersAPI.UpdateTeamMemberTeamMembersMemberIdPatch(context.Background(), memberId).Updates(updates).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TeamMembersAPI.UpdateTeamMemberTeamMembersMemberIdPatch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateTeamMemberTeamMembersMemberIdPatch`: ResponseUpdateTeamMemberTeamMembersMemberIdPatch
	fmt.Fprintf(os.Stdout, "Response from `TeamMembersAPI.UpdateTeamMemberTeamMembersMemberIdPatch`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**memberId** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateTeamMemberTeamMembersMemberIdPatchRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **updates** | [**Updates**](Updates.md) |  | 

### Return type

[**ResponseUpdateTeamMemberTeamMembersMemberIdPatch**](ResponseUpdateTeamMemberTeamMembersMemberIdPatch.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

