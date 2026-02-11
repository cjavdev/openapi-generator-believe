# OpenAPI\Client\TeamMembersApi



All URIs are relative to https://believe.cjav.dev, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createTeamMemberTeamMembersPost()**](TeamMembersApi.md#createTeamMemberTeamMembersPost) | **POST** /team-members | Create a new team member |
| [**deleteTeamMemberTeamMembersMemberIdDelete()**](TeamMembersApi.md#deleteTeamMemberTeamMembersMemberIdDelete) | **DELETE** /team-members/{member_id} | Delete a team member |
| [**getTeamMemberTeamMembersMemberIdGet()**](TeamMembersApi.md#getTeamMemberTeamMembersMemberIdGet) | **GET** /team-members/{member_id} | Get a team member by ID |
| [**listCoachesTeamMembersCoachesGet()**](TeamMembersApi.md#listCoachesTeamMembersCoachesGet) | **GET** /team-members/coaches/ | List all coaches |
| [**listPlayersTeamMembersPlayersGet()**](TeamMembersApi.md#listPlayersTeamMembersPlayersGet) | **GET** /team-members/players/ | List all players |
| [**listStaffTeamMembersStaffGet()**](TeamMembersApi.md#listStaffTeamMembersStaffGet) | **GET** /team-members/staff/ | List all staff (non-player, non-coach) |
| [**listTeamMembersTeamMembersGet()**](TeamMembersApi.md#listTeamMembersTeamMembersGet) | **GET** /team-members | List all team members |
| [**updateTeamMemberTeamMembersMemberIdPatch()**](TeamMembersApi.md#updateTeamMemberTeamMembersMemberIdPatch) | **PATCH** /team-members/{member_id} | Update a team member |


## `createTeamMemberTeamMembersPost()`

```php
createTeamMemberTeamMembersPost($member): \OpenAPI\Client\Model\ResponseCreateTeamMemberTeamMembersPost
```

Create a new team member

Add a new team member to a team.  The request body is a **union type (oneOf)** - you must include the `member_type` discriminator field: - `\"member_type\": \"player\"` - Creates a player (requires position, jersey_number, etc.) - `\"member_type\": \"coach\"` - Creates a coach (requires specialty, etc.) - `\"member_type\": \"medical_staff\"` - Creates medical staff (requires medical specialty, etc.) - `\"member_type\": \"equipment_manager\"` - Creates equipment manager (requires responsibilities, etc.)  The `character_id` field references an existing character from `/characters/{id}`.  **Example for creating a player:** ```json {   \"member_type\": \"player\",   \"character_id\": \"sam-obisanya\",   \"team_id\": \"afc-richmond\",   \"years_with_team\": 2,   \"position\": \"midfielder\",   \"jersey_number\": 24,   \"goals_scored\": 12,   \"assists\": 15 } ```

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: HTTPBearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\TeamMembersApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$member = new \OpenAPI\Client\Model\Member(); // \OpenAPI\Client\Model\Member

try {
    $result = $apiInstance->createTeamMemberTeamMembersPost($member);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling TeamMembersApi->createTeamMemberTeamMembersPost: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **member** | [**\OpenAPI\Client\Model\Member**](../Model/Member.md)|  | |

### Return type

[**\OpenAPI\Client\Model\ResponseCreateTeamMemberTeamMembersPost**](../Model/ResponseCreateTeamMemberTeamMembersPost.md)

### Authorization

[HTTPBearer](../../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `deleteTeamMemberTeamMembersMemberIdDelete()`

```php
deleteTeamMemberTeamMembersMemberIdDelete($member_id)
```

Delete a team member

Remove a team member from the roster.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: HTTPBearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\TeamMembersApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$member_id = 'member_id_example'; // string

try {
    $apiInstance->deleteTeamMemberTeamMembersMemberIdDelete($member_id);
} catch (Exception $e) {
    echo 'Exception when calling TeamMembersApi->deleteTeamMemberTeamMembersMemberIdDelete: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **member_id** | **string**|  | |

### Return type

void (empty response body)

### Authorization

[HTTPBearer](../../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getTeamMemberTeamMembersMemberIdGet()`

```php
getTeamMemberTeamMembersMemberIdGet($member_id): \OpenAPI\Client\Model\ResponseGetTeamMemberTeamMembersMemberIdGet
```

Get a team member by ID

Retrieve detailed information about a specific team member.  The response is a **union type (oneOf)** - the actual shape depends on the member's type: - **player**: Includes position, jersey_number, goals_scored, assists, is_captain - **coach**: Includes specialty, certifications, win_rate - **medical_staff**: Includes specialty, qualifications, license_number - **equipment_manager**: Includes responsibilities, is_head_kitman  Use `character_id` to fetch full character details from `/characters/{character_id}`.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: HTTPBearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\TeamMembersApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$member_id = 'member_id_example'; // string

try {
    $result = $apiInstance->getTeamMemberTeamMembersMemberIdGet($member_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling TeamMembersApi->getTeamMemberTeamMembersMemberIdGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **member_id** | **string**|  | |

### Return type

[**\OpenAPI\Client\Model\ResponseGetTeamMemberTeamMembersMemberIdGet**](../Model/ResponseGetTeamMemberTeamMembersMemberIdGet.md)

### Authorization

[HTTPBearer](../../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `listCoachesTeamMembersCoachesGet()`

```php
listCoachesTeamMembersCoachesGet($specialty, $team_id, $skip, $limit): \OpenAPI\Client\Model\PaginatedResponseCoach
```

List all coaches

Get only coaches (filtered subset of team members).

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: HTTPBearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\TeamMembersApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$specialty = new \OpenAPI\Client\Model\\OpenAPIClientModelCoachSpecialty(); // \OpenAPIClientModelCoachSpecialty | Filter by specialty
$team_id = 'team_id_example'; // string | Filter by team ID
$skip = 0; // int | Number of items to skip (offset)
$limit = 20; // int | Maximum number of items to return (max: 100)

try {
    $result = $apiInstance->listCoachesTeamMembersCoachesGet($specialty, $team_id, $skip, $limit);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling TeamMembersApi->listCoachesTeamMembersCoachesGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **specialty** | [**\OpenAPIClientModelCoachSpecialty**](../Model/.md)| Filter by specialty | [optional] |
| **team_id** | **string**| Filter by team ID | [optional] |
| **skip** | **int**| Number of items to skip (offset) | [optional] [default to 0] |
| **limit** | **int**| Maximum number of items to return (max: 100) | [optional] [default to 20] |

### Return type

[**\OpenAPI\Client\Model\PaginatedResponseCoach**](../Model/PaginatedResponseCoach.md)

### Authorization

[HTTPBearer](../../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `listPlayersTeamMembersPlayersGet()`

```php
listPlayersTeamMembersPlayersGet($position, $team_id, $skip, $limit): \OpenAPI\Client\Model\PaginatedResponsePlayer
```

List all players

Get only players (filtered subset of team members).

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: HTTPBearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\TeamMembersApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$position = new \OpenAPI\Client\Model\\OpenAPIClientModelPosition(); // \OpenAPIClientModelPosition | Filter by position
$team_id = 'team_id_example'; // string | Filter by team ID
$skip = 0; // int | Number of items to skip (offset)
$limit = 20; // int | Maximum number of items to return (max: 100)

try {
    $result = $apiInstance->listPlayersTeamMembersPlayersGet($position, $team_id, $skip, $limit);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling TeamMembersApi->listPlayersTeamMembersPlayersGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **position** | [**\OpenAPIClientModelPosition**](../Model/.md)| Filter by position | [optional] |
| **team_id** | **string**| Filter by team ID | [optional] |
| **skip** | **int**| Number of items to skip (offset) | [optional] [default to 0] |
| **limit** | **int**| Maximum number of items to return (max: 100) | [optional] [default to 20] |

### Return type

[**\OpenAPI\Client\Model\PaginatedResponsePlayer**](../Model/PaginatedResponsePlayer.md)

### Authorization

[HTTPBearer](../../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `listStaffTeamMembersStaffGet()`

```php
listStaffTeamMembersStaffGet($team_id, $skip, $limit): \OpenAPI\Client\Model\PaginatedResponseUnionMedicalStaffEquipmentManager
```

List all staff (non-player, non-coach)

Get all staff members (medical staff and equipment managers).  This demonstrates a **narrower union type** - the response is oneOf MedicalStaff or EquipmentManager.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: HTTPBearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\TeamMembersApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$team_id = 'team_id_example'; // string | Filter by team ID
$skip = 0; // int | Number of items to skip (offset)
$limit = 20; // int | Maximum number of items to return (max: 100)

try {
    $result = $apiInstance->listStaffTeamMembersStaffGet($team_id, $skip, $limit);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling TeamMembersApi->listStaffTeamMembersStaffGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **team_id** | **string**| Filter by team ID | [optional] |
| **skip** | **int**| Number of items to skip (offset) | [optional] [default to 0] |
| **limit** | **int**| Maximum number of items to return (max: 100) | [optional] [default to 20] |

### Return type

[**\OpenAPI\Client\Model\PaginatedResponseUnionMedicalStaffEquipmentManager**](../Model/PaginatedResponseUnionMedicalStaffEquipmentManager.md)

### Authorization

[HTTPBearer](../../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `listTeamMembersTeamMembersGet()`

```php
listTeamMembersTeamMembersGet($member_type, $team_id, $skip, $limit): \OpenAPI\Client\Model\PaginatedResponseAnnotatedUnionPlayerCoachMedicalStaffEquipmentManagerFieldInfoAnnotationNoneTypeRequiredTrueDiscriminatorMemberType
```

List all team members

Get a paginated list of all team members.  This endpoint demonstrates **union types (oneOf)** in the response. Each team member can be one of: Player, Coach, MedicalStaff, or EquipmentManager. The `member_type` field acts as a discriminator to determine the shape of each object.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: HTTPBearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\TeamMembersApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$member_type = new \OpenAPI\Client\Model\\OpenAPIClientModelMemberType(); // \OpenAPIClientModelMemberType | Filter by member type
$team_id = 'team_id_example'; // string | Filter by team ID
$skip = 0; // int | Number of items to skip (offset)
$limit = 20; // int | Maximum number of items to return (max: 100)

try {
    $result = $apiInstance->listTeamMembersTeamMembersGet($member_type, $team_id, $skip, $limit);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling TeamMembersApi->listTeamMembersTeamMembersGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **member_type** | [**\OpenAPIClientModelMemberType**](../Model/.md)| Filter by member type | [optional] |
| **team_id** | **string**| Filter by team ID | [optional] |
| **skip** | **int**| Number of items to skip (offset) | [optional] [default to 0] |
| **limit** | **int**| Maximum number of items to return (max: 100) | [optional] [default to 20] |

### Return type

[**\OpenAPI\Client\Model\PaginatedResponseAnnotatedUnionPlayerCoachMedicalStaffEquipmentManagerFieldInfoAnnotationNoneTypeRequiredTrueDiscriminatorMemberType**](../Model/PaginatedResponseAnnotatedUnionPlayerCoachMedicalStaffEquipmentManagerFieldInfoAnnotationNoneTypeRequiredTrueDiscriminatorMemberType.md)

### Authorization

[HTTPBearer](../../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `updateTeamMemberTeamMembersMemberIdPatch()`

```php
updateTeamMemberTeamMembersMemberIdPatch($member_id, $updates): \OpenAPI\Client\Model\ResponseUpdateTeamMemberTeamMembersMemberIdPatch
```

Update a team member

Update specific fields of an existing team member. Fields vary by member type.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: HTTPBearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\TeamMembersApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$member_id = 'member_id_example'; // string
$updates = new \OpenAPI\Client\Model\Updates(); // \OpenAPI\Client\Model\Updates

try {
    $result = $apiInstance->updateTeamMemberTeamMembersMemberIdPatch($member_id, $updates);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling TeamMembersApi->updateTeamMemberTeamMembersMemberIdPatch: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **member_id** | **string**|  | |
| **updates** | [**\OpenAPI\Client\Model\Updates**](../Model/Updates.md)|  | |

### Return type

[**\OpenAPI\Client\Model\ResponseUpdateTeamMemberTeamMembersMemberIdPatch**](../Model/ResponseUpdateTeamMemberTeamMembersMemberIdPatch.md)

### Authorization

[HTTPBearer](../../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
