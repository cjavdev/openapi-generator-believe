# OpenAPI\Client\QuotesApi

Memorable quotes from the show

All URIs are relative to https://believe.cjav.dev, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createQuoteQuotesPost()**](QuotesApi.md#createQuoteQuotesPost) | **POST** /quotes | Create a new quote |
| [**deleteQuoteQuotesQuoteIdDelete()**](QuotesApi.md#deleteQuoteQuotesQuoteIdDelete) | **DELETE** /quotes/{quote_id} | Delete a quote |
| [**getCharacterQuotesQuotesCharactersCharacterIdGet()**](QuotesApi.md#getCharacterQuotesQuotesCharactersCharacterIdGet) | **GET** /quotes/characters/{character_id} | Get all quotes by a character |
| [**getQuoteQuotesQuoteIdGet()**](QuotesApi.md#getQuoteQuotesQuoteIdGet) | **GET** /quotes/{quote_id} | Get a quote by ID |
| [**getQuotesByThemeQuotesThemesThemeGet()**](QuotesApi.md#getQuotesByThemeQuotesThemesThemeGet) | **GET** /quotes/themes/{theme} | Get quotes by theme |
| [**getRandomQuoteQuotesRandomGet()**](QuotesApi.md#getRandomQuoteQuotesRandomGet) | **GET** /quotes/random | Get a random quote |
| [**listQuotesQuotesGet()**](QuotesApi.md#listQuotesQuotesGet) | **GET** /quotes | List all quotes |
| [**updateQuoteQuotesQuoteIdPatch()**](QuotesApi.md#updateQuoteQuotesQuoteIdPatch) | **PATCH** /quotes/{quote_id} | Update a quote |


## `createQuoteQuotesPost()`

```php
createQuoteQuotesPost($quote_create): \OpenAPI\Client\Model\Quote
```

Create a new quote

Add a new memorable quote to the collection.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: HTTPBearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\QuotesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$quote_create = new \OpenAPI\Client\Model\QuoteCreate(); // \OpenAPI\Client\Model\QuoteCreate

try {
    $result = $apiInstance->createQuoteQuotesPost($quote_create);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling QuotesApi->createQuoteQuotesPost: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **quote_create** | [**\OpenAPI\Client\Model\QuoteCreate**](../Model/QuoteCreate.md)|  | |

### Return type

[**\OpenAPI\Client\Model\Quote**](../Model/Quote.md)

### Authorization

[HTTPBearer](../../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `deleteQuoteQuotesQuoteIdDelete()`

```php
deleteQuoteQuotesQuoteIdDelete($quote_id)
```

Delete a quote

Remove a quote from the collection.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: HTTPBearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\QuotesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$quote_id = 'quote_id_example'; // string

try {
    $apiInstance->deleteQuoteQuotesQuoteIdDelete($quote_id);
} catch (Exception $e) {
    echo 'Exception when calling QuotesApi->deleteQuoteQuotesQuoteIdDelete: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **quote_id** | **string**|  | |

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

## `getCharacterQuotesQuotesCharactersCharacterIdGet()`

```php
getCharacterQuotesQuotesCharactersCharacterIdGet($character_id, $skip, $limit): \OpenAPI\Client\Model\PaginatedResponseQuote
```

Get all quotes by a character

Get a paginated list of quotes from a specific character.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: HTTPBearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\QuotesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$character_id = 'character_id_example'; // string
$skip = 0; // int | Number of items to skip (offset)
$limit = 20; // int | Maximum number of items to return (max: 100)

try {
    $result = $apiInstance->getCharacterQuotesQuotesCharactersCharacterIdGet($character_id, $skip, $limit);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling QuotesApi->getCharacterQuotesQuotesCharactersCharacterIdGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **character_id** | **string**|  | |
| **skip** | **int**| Number of items to skip (offset) | [optional] [default to 0] |
| **limit** | **int**| Maximum number of items to return (max: 100) | [optional] [default to 20] |

### Return type

[**\OpenAPI\Client\Model\PaginatedResponseQuote**](../Model/PaginatedResponseQuote.md)

### Authorization

[HTTPBearer](../../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getQuoteQuotesQuoteIdGet()`

```php
getQuoteQuotesQuoteIdGet($quote_id): \OpenAPI\Client\Model\Quote
```

Get a quote by ID

Retrieve a specific quote by its ID.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: HTTPBearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\QuotesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$quote_id = 'quote_id_example'; // string

try {
    $result = $apiInstance->getQuoteQuotesQuoteIdGet($quote_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling QuotesApi->getQuoteQuotesQuoteIdGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **quote_id** | **string**|  | |

### Return type

[**\OpenAPI\Client\Model\Quote**](../Model/Quote.md)

### Authorization

[HTTPBearer](../../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getQuotesByThemeQuotesThemesThemeGet()`

```php
getQuotesByThemeQuotesThemesThemeGet($theme, $skip, $limit): \OpenAPI\Client\Model\PaginatedResponseQuote
```

Get quotes by theme

Get a paginated list of quotes related to a specific theme.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: HTTPBearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\QuotesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$theme = new \OpenAPI\Client\Model\\OpenAPI\Client\Model\QuoteTheme(); // \OpenAPI\Client\Model\QuoteTheme
$skip = 0; // int | Number of items to skip (offset)
$limit = 20; // int | Maximum number of items to return (max: 100)

try {
    $result = $apiInstance->getQuotesByThemeQuotesThemesThemeGet($theme, $skip, $limit);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling QuotesApi->getQuotesByThemeQuotesThemesThemeGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **theme** | [**\OpenAPI\Client\Model\QuoteTheme**](../Model/.md)|  | |
| **skip** | **int**| Number of items to skip (offset) | [optional] [default to 0] |
| **limit** | **int**| Maximum number of items to return (max: 100) | [optional] [default to 20] |

### Return type

[**\OpenAPI\Client\Model\PaginatedResponseQuote**](../Model/PaginatedResponseQuote.md)

### Authorization

[HTTPBearer](../../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getRandomQuoteQuotesRandomGet()`

```php
getRandomQuoteQuotesRandomGet($character_id, $theme, $inspirational): \OpenAPI\Client\Model\Quote
```

Get a random quote

Get a random Ted Lasso quote, optionally filtered.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: HTTPBearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\QuotesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$character_id = 'character_id_example'; // string | Filter by character
$theme = new \OpenAPI\Client\Model\\OpenAPIClientModelQuoteTheme(); // \OpenAPIClientModelQuoteTheme | Filter by theme
$inspirational = True; // bool | Filter inspirational quotes

try {
    $result = $apiInstance->getRandomQuoteQuotesRandomGet($character_id, $theme, $inspirational);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling QuotesApi->getRandomQuoteQuotesRandomGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **character_id** | **string**| Filter by character | [optional] |
| **theme** | [**\OpenAPIClientModelQuoteTheme**](../Model/.md)| Filter by theme | [optional] |
| **inspirational** | **bool**| Filter inspirational quotes | [optional] |

### Return type

[**\OpenAPI\Client\Model\Quote**](../Model/Quote.md)

### Authorization

[HTTPBearer](../../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `listQuotesQuotesGet()`

```php
listQuotesQuotesGet($character_id, $theme, $moment_type, $inspirational, $funny, $skip, $limit): \OpenAPI\Client\Model\PaginatedResponseQuote
```

List all quotes

Get a paginated list of all memorable Ted Lasso quotes with optional filtering.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: HTTPBearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\QuotesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$character_id = 'character_id_example'; // string | Filter by character
$theme = new \OpenAPI\Client\Model\\OpenAPIClientModelQuoteTheme(); // \OpenAPIClientModelQuoteTheme | Filter by theme
$moment_type = new \OpenAPI\Client\Model\\OpenAPIClientModelQuoteMoment(); // \OpenAPIClientModelQuoteMoment | Filter by moment type
$inspirational = True; // bool | Filter inspirational quotes
$funny = True; // bool | Filter funny quotes
$skip = 0; // int | Number of items to skip (offset)
$limit = 20; // int | Maximum number of items to return (max: 100)

try {
    $result = $apiInstance->listQuotesQuotesGet($character_id, $theme, $moment_type, $inspirational, $funny, $skip, $limit);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling QuotesApi->listQuotesQuotesGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **character_id** | **string**| Filter by character | [optional] |
| **theme** | [**\OpenAPIClientModelQuoteTheme**](../Model/.md)| Filter by theme | [optional] |
| **moment_type** | [**\OpenAPIClientModelQuoteMoment**](../Model/.md)| Filter by moment type | [optional] |
| **inspirational** | **bool**| Filter inspirational quotes | [optional] |
| **funny** | **bool**| Filter funny quotes | [optional] |
| **skip** | **int**| Number of items to skip (offset) | [optional] [default to 0] |
| **limit** | **int**| Maximum number of items to return (max: 100) | [optional] [default to 20] |

### Return type

[**\OpenAPI\Client\Model\PaginatedResponseQuote**](../Model/PaginatedResponseQuote.md)

### Authorization

[HTTPBearer](../../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `updateQuoteQuotesQuoteIdPatch()`

```php
updateQuoteQuotesQuoteIdPatch($quote_id, $quote_update): \OpenAPI\Client\Model\Quote
```

Update a quote

Update specific fields of an existing quote.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: HTTPBearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\QuotesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$quote_id = 'quote_id_example'; // string
$quote_update = new \OpenAPI\Client\Model\QuoteUpdate(); // \OpenAPI\Client\Model\QuoteUpdate

try {
    $result = $apiInstance->updateQuoteQuotesQuoteIdPatch($quote_id, $quote_update);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling QuotesApi->updateQuoteQuotesQuoteIdPatch: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **quote_id** | **string**|  | |
| **quote_update** | [**\OpenAPI\Client\Model\QuoteUpdate**](../Model/QuoteUpdate.md)|  | |

### Return type

[**\OpenAPI\Client\Model\Quote**](../Model/Quote.md)

### Authorization

[HTTPBearer](../../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
