# OpenAPI\Client\CharactersApi

Operations related to Ted Lasso characters

All URIs are relative to https://believe.cjav.dev, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createCharacterCharactersPost()**](CharactersApi.md#createCharacterCharactersPost) | **POST** /characters | Create a new character |
| [**deleteCharacterCharactersCharacterIdDelete()**](CharactersApi.md#deleteCharacterCharactersCharacterIdDelete) | **DELETE** /characters/{character_id} | Delete a character |
| [**getCharacterCharactersCharacterIdGet()**](CharactersApi.md#getCharacterCharactersCharacterIdGet) | **GET** /characters/{character_id} | Get a character by ID |
| [**getCharacterQuotesCharactersCharacterIdQuotesGet()**](CharactersApi.md#getCharacterQuotesCharactersCharacterIdQuotesGet) | **GET** /characters/{character_id}/quotes | Get character&#39;s signature quotes |
| [**listCharactersCharactersGet()**](CharactersApi.md#listCharactersCharactersGet) | **GET** /characters | List all characters |
| [**updateCharacterCharactersCharacterIdPatch()**](CharactersApi.md#updateCharacterCharactersCharacterIdPatch) | **PATCH** /characters/{character_id} | Update a character |


## `createCharacterCharactersPost()`

```php
createCharacterCharactersPost($character_create): \OpenAPI\Client\Model\Character
```

Create a new character

Add a new character to the Ted Lasso universe.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: HTTPBearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\CharactersApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$character_create = new \OpenAPI\Client\Model\CharacterCreate(); // \OpenAPI\Client\Model\CharacterCreate

try {
    $result = $apiInstance->createCharacterCharactersPost($character_create);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CharactersApi->createCharacterCharactersPost: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **character_create** | [**\OpenAPI\Client\Model\CharacterCreate**](../Model/CharacterCreate.md)|  | |

### Return type

[**\OpenAPI\Client\Model\Character**](../Model/Character.md)

### Authorization

[HTTPBearer](../../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `deleteCharacterCharactersCharacterIdDelete()`

```php
deleteCharacterCharactersCharacterIdDelete($character_id)
```

Delete a character

Remove a character from the database.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: HTTPBearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\CharactersApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$character_id = 'character_id_example'; // string

try {
    $apiInstance->deleteCharacterCharactersCharacterIdDelete($character_id);
} catch (Exception $e) {
    echo 'Exception when calling CharactersApi->deleteCharacterCharactersCharacterIdDelete: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **character_id** | **string**|  | |

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

## `getCharacterCharactersCharacterIdGet()`

```php
getCharacterCharactersCharacterIdGet($character_id): \OpenAPI\Client\Model\Character
```

Get a character by ID

Retrieve detailed information about a specific character.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: HTTPBearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\CharactersApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$character_id = 'character_id_example'; // string

try {
    $result = $apiInstance->getCharacterCharactersCharacterIdGet($character_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CharactersApi->getCharacterCharactersCharacterIdGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **character_id** | **string**|  | |

### Return type

[**\OpenAPI\Client\Model\Character**](../Model/Character.md)

### Authorization

[HTTPBearer](../../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getCharacterQuotesCharactersCharacterIdQuotesGet()`

```php
getCharacterQuotesCharactersCharacterIdQuotesGet($character_id): string[]
```

Get character's signature quotes

Get all signature quotes from a specific character.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: HTTPBearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\CharactersApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$character_id = 'character_id_example'; // string

try {
    $result = $apiInstance->getCharacterQuotesCharactersCharacterIdQuotesGet($character_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CharactersApi->getCharacterQuotesCharactersCharacterIdQuotesGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **character_id** | **string**|  | |

### Return type

**string[]**

### Authorization

[HTTPBearer](../../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `listCharactersCharactersGet()`

```php
listCharactersCharactersGet($role, $team_id, $min_optimism, $skip, $limit): \OpenAPI\Client\Model\PaginatedResponseCharacter
```

List all characters

Get a paginated list of Ted Lasso characters.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: HTTPBearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\CharactersApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$role = new \OpenAPI\Client\Model\\OpenAPIClientModelCharacterRole(); // \OpenAPIClientModelCharacterRole | Filter by role
$team_id = 'team_id_example'; // string | Filter by team ID
$min_optimism = 56; // int | Minimum optimism score
$skip = 0; // int | Number of items to skip (offset)
$limit = 20; // int | Maximum number of items to return (max: 100)

try {
    $result = $apiInstance->listCharactersCharactersGet($role, $team_id, $min_optimism, $skip, $limit);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CharactersApi->listCharactersCharactersGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **role** | [**\OpenAPIClientModelCharacterRole**](../Model/.md)| Filter by role | [optional] |
| **team_id** | **string**| Filter by team ID | [optional] |
| **min_optimism** | **int**| Minimum optimism score | [optional] |
| **skip** | **int**| Number of items to skip (offset) | [optional] [default to 0] |
| **limit** | **int**| Maximum number of items to return (max: 100) | [optional] [default to 20] |

### Return type

[**\OpenAPI\Client\Model\PaginatedResponseCharacter**](../Model/PaginatedResponseCharacter.md)

### Authorization

[HTTPBearer](../../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `updateCharacterCharactersCharacterIdPatch()`

```php
updateCharacterCharactersCharacterIdPatch($character_id, $character_update): \OpenAPI\Client\Model\Character
```

Update a character

Update specific fields of an existing character.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: HTTPBearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\CharactersApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$character_id = 'character_id_example'; // string
$character_update = new \OpenAPI\Client\Model\CharacterUpdate(); // \OpenAPI\Client\Model\CharacterUpdate

try {
    $result = $apiInstance->updateCharacterCharactersCharacterIdPatch($character_id, $character_update);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CharactersApi->updateCharacterCharactersCharacterIdPatch: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **character_id** | **string**|  | |
| **character_update** | [**\OpenAPI\Client\Model\CharacterUpdate**](../Model/CharacterUpdate.md)|  | |

### Return type

[**\OpenAPI\Client\Model\Character**](../Model/Character.md)

### Authorization

[HTTPBearer](../../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
