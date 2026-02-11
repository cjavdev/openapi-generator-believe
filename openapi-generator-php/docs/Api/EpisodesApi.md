# OpenAPI\Client\EpisodesApi

Operations related to TV episodes

All URIs are relative to https://believe.cjav.dev, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createEpisodeEpisodesPost()**](EpisodesApi.md#createEpisodeEpisodesPost) | **POST** /episodes | Create a new episode |
| [**deleteEpisodeEpisodesEpisodeIdDelete()**](EpisodesApi.md#deleteEpisodeEpisodesEpisodeIdDelete) | **DELETE** /episodes/{episode_id} | Delete an episode |
| [**getEpisodeEpisodesEpisodeIdGet()**](EpisodesApi.md#getEpisodeEpisodesEpisodeIdGet) | **GET** /episodes/{episode_id} | Get an episode by ID |
| [**getEpisodeWisdomEpisodesEpisodeIdWisdomGet()**](EpisodesApi.md#getEpisodeWisdomEpisodesEpisodeIdWisdomGet) | **GET** /episodes/{episode_id}/wisdom | Get episode wisdom |
| [**getSeasonEpisodesEpisodesSeasonsSeasonNumberGet()**](EpisodesApi.md#getSeasonEpisodesEpisodesSeasonsSeasonNumberGet) | **GET** /episodes/seasons/{season_number} | Get all episodes from a season |
| [**listEpisodesEpisodesGet()**](EpisodesApi.md#listEpisodesEpisodesGet) | **GET** /episodes | List all episodes |
| [**updateEpisodeEpisodesEpisodeIdPatch()**](EpisodesApi.md#updateEpisodeEpisodesEpisodeIdPatch) | **PATCH** /episodes/{episode_id} | Update an episode |


## `createEpisodeEpisodesPost()`

```php
createEpisodeEpisodesPost($episode_create): \OpenAPI\Client\Model\Episode
```

Create a new episode

Add a new episode to the series.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: HTTPBearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\EpisodesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$episode_create = new \OpenAPI\Client\Model\EpisodeCreate(); // \OpenAPI\Client\Model\EpisodeCreate

try {
    $result = $apiInstance->createEpisodeEpisodesPost($episode_create);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling EpisodesApi->createEpisodeEpisodesPost: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **episode_create** | [**\OpenAPI\Client\Model\EpisodeCreate**](../Model/EpisodeCreate.md)|  | |

### Return type

[**\OpenAPI\Client\Model\Episode**](../Model/Episode.md)

### Authorization

[HTTPBearer](../../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `deleteEpisodeEpisodesEpisodeIdDelete()`

```php
deleteEpisodeEpisodesEpisodeIdDelete($episode_id)
```

Delete an episode

Remove an episode from the database.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: HTTPBearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\EpisodesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$episode_id = 'episode_id_example'; // string

try {
    $apiInstance->deleteEpisodeEpisodesEpisodeIdDelete($episode_id);
} catch (Exception $e) {
    echo 'Exception when calling EpisodesApi->deleteEpisodeEpisodesEpisodeIdDelete: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **episode_id** | **string**|  | |

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

## `getEpisodeEpisodesEpisodeIdGet()`

```php
getEpisodeEpisodesEpisodeIdGet($episode_id): \OpenAPI\Client\Model\Episode
```

Get an episode by ID

Retrieve detailed information about a specific episode.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: HTTPBearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\EpisodesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$episode_id = 'episode_id_example'; // string

try {
    $result = $apiInstance->getEpisodeEpisodesEpisodeIdGet($episode_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling EpisodesApi->getEpisodeEpisodesEpisodeIdGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **episode_id** | **string**|  | |

### Return type

[**\OpenAPI\Client\Model\Episode**](../Model/Episode.md)

### Authorization

[HTTPBearer](../../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getEpisodeWisdomEpisodesEpisodeIdWisdomGet()`

```php
getEpisodeWisdomEpisodesEpisodeIdWisdomGet($episode_id): array<string,mixed>
```

Get episode wisdom

Get Ted's wisdom and memorable moments from a specific episode.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: HTTPBearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\EpisodesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$episode_id = 'episode_id_example'; // string

try {
    $result = $apiInstance->getEpisodeWisdomEpisodesEpisodeIdWisdomGet($episode_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling EpisodesApi->getEpisodeWisdomEpisodesEpisodeIdWisdomGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **episode_id** | **string**|  | |

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

## `getSeasonEpisodesEpisodesSeasonsSeasonNumberGet()`

```php
getSeasonEpisodesEpisodesSeasonsSeasonNumberGet($season_number, $skip, $limit): \OpenAPI\Client\Model\PaginatedResponseEpisode
```

Get all episodes from a season

Get a paginated list of episodes from a specific season.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: HTTPBearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\EpisodesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$season_number = 56; // int
$skip = 0; // int | Number of items to skip (offset)
$limit = 20; // int | Maximum number of items to return (max: 100)

try {
    $result = $apiInstance->getSeasonEpisodesEpisodesSeasonsSeasonNumberGet($season_number, $skip, $limit);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling EpisodesApi->getSeasonEpisodesEpisodesSeasonsSeasonNumberGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **season_number** | **int**|  | |
| **skip** | **int**| Number of items to skip (offset) | [optional] [default to 0] |
| **limit** | **int**| Maximum number of items to return (max: 100) | [optional] [default to 20] |

### Return type

[**\OpenAPI\Client\Model\PaginatedResponseEpisode**](../Model/PaginatedResponseEpisode.md)

### Authorization

[HTTPBearer](../../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `listEpisodesEpisodesGet()`

```php
listEpisodesEpisodesGet($season, $character_focus, $skip, $limit): \OpenAPI\Client\Model\PaginatedResponseEpisode
```

List all episodes

Get a paginated list of all Ted Lasso episodes with optional filtering by season.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: HTTPBearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\EpisodesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$season = 56; // int | Filter by season
$character_focus = 'character_focus_example'; // string | Filter by character focus (character ID)
$skip = 0; // int | Number of items to skip (offset)
$limit = 20; // int | Maximum number of items to return (max: 100)

try {
    $result = $apiInstance->listEpisodesEpisodesGet($season, $character_focus, $skip, $limit);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling EpisodesApi->listEpisodesEpisodesGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **season** | **int**| Filter by season | [optional] |
| **character_focus** | **string**| Filter by character focus (character ID) | [optional] |
| **skip** | **int**| Number of items to skip (offset) | [optional] [default to 0] |
| **limit** | **int**| Maximum number of items to return (max: 100) | [optional] [default to 20] |

### Return type

[**\OpenAPI\Client\Model\PaginatedResponseEpisode**](../Model/PaginatedResponseEpisode.md)

### Authorization

[HTTPBearer](../../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `updateEpisodeEpisodesEpisodeIdPatch()`

```php
updateEpisodeEpisodesEpisodeIdPatch($episode_id, $episode_update): \OpenAPI\Client\Model\Episode
```

Update an episode

Update specific fields of an existing episode.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: HTTPBearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\EpisodesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$episode_id = 'episode_id_example'; // string
$episode_update = new \OpenAPI\Client\Model\EpisodeUpdate(); // \OpenAPI\Client\Model\EpisodeUpdate

try {
    $result = $apiInstance->updateEpisodeEpisodesEpisodeIdPatch($episode_id, $episode_update);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling EpisodesApi->updateEpisodeEpisodesEpisodeIdPatch: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **episode_id** | **string**|  | |
| **episode_update** | [**\OpenAPI\Client\Model\EpisodeUpdate**](../Model/EpisodeUpdate.md)|  | |

### Return type

[**\OpenAPI\Client\Model\Episode**](../Model/Episode.md)

### Authorization

[HTTPBearer](../../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
