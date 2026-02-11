# OpenAPI\Client\StreamingApi

Server-Sent Events (SSE) streaming endpoints

All URIs are relative to https://believe.cjav.dev, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**getPepTalkPepTalkGet()**](StreamingApi.md#getPepTalkPepTalkGet) | **GET** /pep-talk | Get a Pep Talk |
| [**streamMatchCommentaryMatchesMatchIdCommentaryStreamPost()**](StreamingApi.md#streamMatchCommentaryMatchesMatchIdCommentaryStreamPost) | **POST** /matches/{match_id}/commentary/stream | Stream Match Commentary |
| [**testStreamStreamTestGet()**](StreamingApi.md#testStreamStreamTestGet) | **GET** /stream/test | Test SSE Connection |


## `getPepTalkPepTalkGet()`

```php
getPepTalkPepTalkGet($stream): \OpenAPI\Client\Model\PepTalkResponse
```

Get a Pep Talk

Get a motivational pep talk from Ted Lasso himself. By default returns the complete pep talk. Add `?stream=true` to get Server-Sent Events (SSE) streaming the pep talk chunk by chunk.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: HTTPBearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\StreamingApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$stream = false; // bool | If true, returns SSE stream instead of full response

try {
    $result = $apiInstance->getPepTalkPepTalkGet($stream);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling StreamingApi->getPepTalkPepTalkGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **stream** | **bool**| If true, returns SSE stream instead of full response | [optional] [default to false] |

### Return type

[**\OpenAPI\Client\Model\PepTalkResponse**](../Model/PepTalkResponse.md)

### Authorization

[HTTPBearer](../../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `text/event-stream`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `streamMatchCommentaryMatchesMatchIdCommentaryStreamPost()`

```php
streamMatchCommentaryMatchesMatchIdCommentaryStreamPost($match_id): mixed
```

Stream Match Commentary

Stream live match commentary for a specific match. Uses Server-Sent Events (SSE) to stream commentary events in real-time.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: HTTPBearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\StreamingApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$match_id = 'match_id_example'; // string

try {
    $result = $apiInstance->streamMatchCommentaryMatchesMatchIdCommentaryStreamPost($match_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling StreamingApi->streamMatchCommentaryMatchesMatchIdCommentaryStreamPost: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **match_id** | **string**|  | |

### Return type

**mixed**

### Authorization

[HTTPBearer](../../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `text/event-stream`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `testStreamStreamTestGet()`

```php
testStreamStreamTestGet(): mixed
```

Test SSE Connection

A simple SSE test endpoint that streams numbers 1-5.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: HTTPBearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\StreamingApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $result = $apiInstance->testStreamStreamTestGet();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling StreamingApi->testStreamStreamTestGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

**mixed**

### Authorization

[HTTPBearer](../../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`, `text/event-stream`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
