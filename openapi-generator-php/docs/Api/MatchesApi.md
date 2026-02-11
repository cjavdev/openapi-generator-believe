# OpenAPI\Client\MatchesApi

Operations related to football matches

All URIs are relative to https://believe.cjav.dev, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createMatchMatchesPost()**](MatchesApi.md#createMatchMatchesPost) | **POST** /matches | Create a new match |
| [**deleteMatchMatchesMatchIdDelete()**](MatchesApi.md#deleteMatchMatchesMatchIdDelete) | **DELETE** /matches/{match_id} | Delete a match |
| [**getMatchLessonMatchesMatchIdLessonGet()**](MatchesApi.md#getMatchLessonMatchesMatchIdLessonGet) | **GET** /matches/{match_id}/lesson | Get match lesson |
| [**getMatchMatchesMatchIdGet()**](MatchesApi.md#getMatchMatchesMatchIdGet) | **GET** /matches/{match_id} | Get a match by ID |
| [**getTurningPointsMatchesMatchIdTurningPointsGet()**](MatchesApi.md#getTurningPointsMatchesMatchIdTurningPointsGet) | **GET** /matches/{match_id}/turning-points | Get match turning points |
| [**listMatchesMatchesGet()**](MatchesApi.md#listMatchesMatchesGet) | **GET** /matches | List all matches |
| [**updateMatchMatchesMatchIdPatch()**](MatchesApi.md#updateMatchMatchesMatchIdPatch) | **PATCH** /matches/{match_id} | Update a match |


## `createMatchMatchesPost()`

```php
createMatchMatchesPost($match_create): \OpenAPI\Client\Model\Match
```

Create a new match

Schedule a new match.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: HTTPBearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\MatchesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$match_create = new \OpenAPI\Client\Model\MatchCreate(); // \OpenAPI\Client\Model\MatchCreate

try {
    $result = $apiInstance->createMatchMatchesPost($match_create);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling MatchesApi->createMatchMatchesPost: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **match_create** | [**\OpenAPI\Client\Model\MatchCreate**](../Model/MatchCreate.md)|  | |

### Return type

[**\OpenAPI\Client\Model\Match**](../Model/Match.md)

### Authorization

[HTTPBearer](../../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `deleteMatchMatchesMatchIdDelete()`

```php
deleteMatchMatchesMatchIdDelete($match_id)
```

Delete a match

Remove a match from the database.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: HTTPBearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\MatchesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$match_id = 'match_id_example'; // string

try {
    $apiInstance->deleteMatchMatchesMatchIdDelete($match_id);
} catch (Exception $e) {
    echo 'Exception when calling MatchesApi->deleteMatchMatchesMatchIdDelete: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **match_id** | **string**|  | |

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

## `getMatchLessonMatchesMatchIdLessonGet()`

```php
getMatchLessonMatchesMatchIdLessonGet($match_id): array<string,mixed>
```

Get match lesson

Get the life lesson learned from a specific match.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: HTTPBearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\MatchesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$match_id = 'match_id_example'; // string

try {
    $result = $apiInstance->getMatchLessonMatchesMatchIdLessonGet($match_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling MatchesApi->getMatchLessonMatchesMatchIdLessonGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **match_id** | **string**|  | |

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

## `getMatchMatchesMatchIdGet()`

```php
getMatchMatchesMatchIdGet($match_id): \OpenAPI\Client\Model\Match
```

Get a match by ID

Retrieve detailed information about a specific match.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: HTTPBearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\MatchesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$match_id = 'match_id_example'; // string

try {
    $result = $apiInstance->getMatchMatchesMatchIdGet($match_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling MatchesApi->getMatchMatchesMatchIdGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **match_id** | **string**|  | |

### Return type

[**\OpenAPI\Client\Model\Match**](../Model/Match.md)

### Authorization

[HTTPBearer](../../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getTurningPointsMatchesMatchIdTurningPointsGet()`

```php
getTurningPointsMatchesMatchIdTurningPointsGet($match_id): array<string,mixed>[]
```

Get match turning points

Get all turning points from a specific match.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: HTTPBearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\MatchesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$match_id = 'match_id_example'; // string

try {
    $result = $apiInstance->getTurningPointsMatchesMatchIdTurningPointsGet($match_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling MatchesApi->getTurningPointsMatchesMatchIdTurningPointsGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **match_id** | **string**|  | |

### Return type

**array<string,mixed>[]**

### Authorization

[HTTPBearer](../../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `listMatchesMatchesGet()`

```php
listMatchesMatchesGet($team_id, $result, $match_type, $skip, $limit): \OpenAPI\Client\Model\PaginatedResponseMatch
```

List all matches

Get a paginated list of all matches with optional filtering.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: HTTPBearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\MatchesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$team_id = 'team_id_example'; // string | Filter by team (home or away)
$result = new \OpenAPI\Client\Model\\OpenAPIClientModelMatchResult(); // \OpenAPIClientModelMatchResult | Filter by result
$match_type = new \OpenAPI\Client\Model\\OpenAPIClientModelMatchType(); // \OpenAPIClientModelMatchType | Filter by match type
$skip = 0; // int | Number of items to skip (offset)
$limit = 20; // int | Maximum number of items to return (max: 100)

try {
    $result = $apiInstance->listMatchesMatchesGet($team_id, $result, $match_type, $skip, $limit);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling MatchesApi->listMatchesMatchesGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **team_id** | **string**| Filter by team (home or away) | [optional] |
| **result** | [**\OpenAPIClientModelMatchResult**](../Model/.md)| Filter by result | [optional] |
| **match_type** | [**\OpenAPIClientModelMatchType**](../Model/.md)| Filter by match type | [optional] |
| **skip** | **int**| Number of items to skip (offset) | [optional] [default to 0] |
| **limit** | **int**| Maximum number of items to return (max: 100) | [optional] [default to 20] |

### Return type

[**\OpenAPI\Client\Model\PaginatedResponseMatch**](../Model/PaginatedResponseMatch.md)

### Authorization

[HTTPBearer](../../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `updateMatchMatchesMatchIdPatch()`

```php
updateMatchMatchesMatchIdPatch($match_id, $match_update): \OpenAPI\Client\Model\Match
```

Update a match

Update specific fields of an existing match (e.g., update score).

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: HTTPBearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\MatchesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$match_id = 'match_id_example'; // string
$match_update = new \OpenAPI\Client\Model\MatchUpdate(); // \OpenAPI\Client\Model\MatchUpdate

try {
    $result = $apiInstance->updateMatchMatchesMatchIdPatch($match_id, $match_update);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling MatchesApi->updateMatchMatchesMatchIdPatch: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **match_id** | **string**|  | |
| **match_update** | [**\OpenAPI\Client\Model\MatchUpdate**](../Model/MatchUpdate.md)|  | |

### Return type

[**\OpenAPI\Client\Model\Match**](../Model/Match.md)

### Authorization

[HTTPBearer](../../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
