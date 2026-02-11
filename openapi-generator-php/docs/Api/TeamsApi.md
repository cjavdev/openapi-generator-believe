# OpenAPI\Client\TeamsApi

Operations related to football teams

All URIs are relative to https://believe.cjav.dev, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createTeamTeamsPost()**](TeamsApi.md#createTeamTeamsPost) | **POST** /teams | Create a new team |
| [**deleteTeamLogoTeamsTeamIdLogoFileIdDelete()**](TeamsApi.md#deleteTeamLogoTeamsTeamIdLogoFileIdDelete) | **DELETE** /teams/{team_id}/logo/{file_id} | Delete team logo |
| [**deleteTeamTeamsTeamIdDelete()**](TeamsApi.md#deleteTeamTeamsTeamIdDelete) | **DELETE** /teams/{team_id} | Delete a team |
| [**downloadTeamLogoTeamsTeamIdLogoFileIdGet()**](TeamsApi.md#downloadTeamLogoTeamsTeamIdLogoFileIdGet) | **GET** /teams/{team_id}/logo/{file_id} | Download team logo |
| [**getTeamCultureTeamsTeamIdCultureGet()**](TeamsApi.md#getTeamCultureTeamsTeamIdCultureGet) | **GET** /teams/{team_id}/culture | Get team culture details |
| [**getTeamRivalsTeamsTeamIdRivalsGet()**](TeamsApi.md#getTeamRivalsTeamsTeamIdRivalsGet) | **GET** /teams/{team_id}/rivals | Get team&#39;s rivals |
| [**getTeamTeamsTeamIdGet()**](TeamsApi.md#getTeamTeamsTeamIdGet) | **GET** /teams/{team_id} | Get a team by ID |
| [**listTeamLogosTeamsTeamIdLogosGet()**](TeamsApi.md#listTeamLogosTeamsTeamIdLogosGet) | **GET** /teams/{team_id}/logos | List team logos |
| [**listTeamsTeamsGet()**](TeamsApi.md#listTeamsTeamsGet) | **GET** /teams | List all teams |
| [**updateTeamTeamsTeamIdPatch()**](TeamsApi.md#updateTeamTeamsTeamIdPatch) | **PATCH** /teams/{team_id} | Update a team |
| [**uploadTeamLogoTeamsTeamIdLogoPost()**](TeamsApi.md#uploadTeamLogoTeamsTeamIdLogoPost) | **POST** /teams/{team_id}/logo | Upload team logo |


## `createTeamTeamsPost()`

```php
createTeamTeamsPost($team_create): \OpenAPI\Client\Model\Team
```

Create a new team

Add a new team to the league.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: HTTPBearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\TeamsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$team_create = new \OpenAPI\Client\Model\TeamCreate(); // \OpenAPI\Client\Model\TeamCreate

try {
    $result = $apiInstance->createTeamTeamsPost($team_create);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling TeamsApi->createTeamTeamsPost: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **team_create** | [**\OpenAPI\Client\Model\TeamCreate**](../Model/TeamCreate.md)|  | |

### Return type

[**\OpenAPI\Client\Model\Team**](../Model/Team.md)

### Authorization

[HTTPBearer](../../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `deleteTeamLogoTeamsTeamIdLogoFileIdDelete()`

```php
deleteTeamLogoTeamsTeamIdLogoFileIdDelete($team_id, $file_id)
```

Delete team logo

Delete a team's logo.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: HTTPBearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\TeamsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$team_id = 'team_id_example'; // string
$file_id = 'file_id_example'; // string

try {
    $apiInstance->deleteTeamLogoTeamsTeamIdLogoFileIdDelete($team_id, $file_id);
} catch (Exception $e) {
    echo 'Exception when calling TeamsApi->deleteTeamLogoTeamsTeamIdLogoFileIdDelete: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **team_id** | **string**|  | |
| **file_id** | **string**|  | |

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

## `deleteTeamTeamsTeamIdDelete()`

```php
deleteTeamTeamsTeamIdDelete($team_id)
```

Delete a team

Remove a team from the database (relegation to oblivion).

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: HTTPBearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\TeamsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$team_id = 'team_id_example'; // string

try {
    $apiInstance->deleteTeamTeamsTeamIdDelete($team_id);
} catch (Exception $e) {
    echo 'Exception when calling TeamsApi->deleteTeamTeamsTeamIdDelete: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **team_id** | **string**|  | |

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

## `downloadTeamLogoTeamsTeamIdLogoFileIdGet()`

```php
downloadTeamLogoTeamsTeamIdLogoFileIdGet($team_id, $file_id): mixed
```

Download team logo

Download a team's logo by file ID.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: HTTPBearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\TeamsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$team_id = 'team_id_example'; // string
$file_id = 'file_id_example'; // string

try {
    $result = $apiInstance->downloadTeamLogoTeamsTeamIdLogoFileIdGet($team_id, $file_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling TeamsApi->downloadTeamLogoTeamsTeamIdLogoFileIdGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **team_id** | **string**|  | |
| **file_id** | **string**|  | |

### Return type

**mixed**

### Authorization

[HTTPBearer](../../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `image/*`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getTeamCultureTeamsTeamIdCultureGet()`

```php
getTeamCultureTeamsTeamIdCultureGet($team_id): array<string,mixed>
```

Get team culture details

Get detailed culture and values information for a team.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: HTTPBearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\TeamsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$team_id = 'team_id_example'; // string

try {
    $result = $apiInstance->getTeamCultureTeamsTeamIdCultureGet($team_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling TeamsApi->getTeamCultureTeamsTeamIdCultureGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **team_id** | **string**|  | |

### Return type

**array<string,mixed>**

### Authorization

[HTTPBearer](../../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getTeamRivalsTeamsTeamIdRivalsGet()`

```php
getTeamRivalsTeamsTeamIdRivalsGet($team_id): \OpenAPI\Client\Model\Team[]
```

Get team's rivals

Get all rival teams for a specific team.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: HTTPBearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\TeamsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$team_id = 'team_id_example'; // string

try {
    $result = $apiInstance->getTeamRivalsTeamsTeamIdRivalsGet($team_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling TeamsApi->getTeamRivalsTeamsTeamIdRivalsGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **team_id** | **string**|  | |

### Return type

[**\OpenAPI\Client\Model\Team[]**](../Model/Team.md)

### Authorization

[HTTPBearer](../../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getTeamTeamsTeamIdGet()`

```php
getTeamTeamsTeamIdGet($team_id): \OpenAPI\Client\Model\Team
```

Get a team by ID

Retrieve detailed information about a specific team.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: HTTPBearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\TeamsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$team_id = 'team_id_example'; // string

try {
    $result = $apiInstance->getTeamTeamsTeamIdGet($team_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling TeamsApi->getTeamTeamsTeamIdGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **team_id** | **string**|  | |

### Return type

[**\OpenAPI\Client\Model\Team**](../Model/Team.md)

### Authorization

[HTTPBearer](../../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `listTeamLogosTeamsTeamIdLogosGet()`

```php
listTeamLogosTeamsTeamIdLogosGet($team_id): \OpenAPI\Client\Model\FileUploadResponse[]
```

List team logos

List all uploaded logos for a team.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: HTTPBearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\TeamsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$team_id = 'team_id_example'; // string

try {
    $result = $apiInstance->listTeamLogosTeamsTeamIdLogosGet($team_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling TeamsApi->listTeamLogosTeamsTeamIdLogosGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **team_id** | **string**|  | |

### Return type

[**\OpenAPI\Client\Model\FileUploadResponse[]**](../Model/FileUploadResponse.md)

### Authorization

[HTTPBearer](../../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `listTeamsTeamsGet()`

```php
listTeamsTeamsGet($league, $min_culture_score, $skip, $limit): \OpenAPI\Client\Model\PaginatedResponseTeam
```

List all teams

Get a paginated list of all teams with optional filtering by league or culture score.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: HTTPBearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\TeamsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$league = new \OpenAPI\Client\Model\\OpenAPIClientModelLeague(); // \OpenAPIClientModelLeague | Filter by league
$min_culture_score = 56; // int | Minimum culture score
$skip = 0; // int | Number of items to skip (offset)
$limit = 20; // int | Maximum number of items to return (max: 100)

try {
    $result = $apiInstance->listTeamsTeamsGet($league, $min_culture_score, $skip, $limit);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling TeamsApi->listTeamsTeamsGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **league** | [**\OpenAPIClientModelLeague**](../Model/.md)| Filter by league | [optional] |
| **min_culture_score** | **int**| Minimum culture score | [optional] |
| **skip** | **int**| Number of items to skip (offset) | [optional] [default to 0] |
| **limit** | **int**| Maximum number of items to return (max: 100) | [optional] [default to 20] |

### Return type

[**\OpenAPI\Client\Model\PaginatedResponseTeam**](../Model/PaginatedResponseTeam.md)

### Authorization

[HTTPBearer](../../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `updateTeamTeamsTeamIdPatch()`

```php
updateTeamTeamsTeamIdPatch($team_id, $team_update): \OpenAPI\Client\Model\Team
```

Update a team

Update specific fields of an existing team.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: HTTPBearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\TeamsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$team_id = 'team_id_example'; // string
$team_update = new \OpenAPI\Client\Model\TeamUpdate(); // \OpenAPI\Client\Model\TeamUpdate

try {
    $result = $apiInstance->updateTeamTeamsTeamIdPatch($team_id, $team_update);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling TeamsApi->updateTeamTeamsTeamIdPatch: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **team_id** | **string**|  | |
| **team_update** | [**\OpenAPI\Client\Model\TeamUpdate**](../Model/TeamUpdate.md)|  | |

### Return type

[**\OpenAPI\Client\Model\Team**](../Model/Team.md)

### Authorization

[HTTPBearer](../../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `uploadTeamLogoTeamsTeamIdLogoPost()`

```php
uploadTeamLogoTeamsTeamIdLogoPost($team_id, $file): \OpenAPI\Client\Model\FileUploadResponse
```

Upload team logo

Upload a logo image for a team. Accepts image files (jpg, png, gif, webp).

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: HTTPBearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\TeamsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$team_id = 'team_id_example'; // string
$file = '/path/to/file.txt'; // \SplFileObject | Logo image file

try {
    $result = $apiInstance->uploadTeamLogoTeamsTeamIdLogoPost($team_id, $file);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling TeamsApi->uploadTeamLogoTeamsTeamIdLogoPost: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **team_id** | **string**|  | |
| **file** | **\SplFileObject****\SplFileObject**| Logo image file | |

### Return type

[**\OpenAPI\Client\Model\FileUploadResponse**](../Model/FileUploadResponse.md)

### Authorization

[HTTPBearer](../../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: `multipart/form-data`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
