# OpenAPI\Client\InteractiveApi

Interactive endpoints for motivation and guidance

All URIs are relative to https://believe.cjav.dev, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**believeEngineBelievePost()**](InteractiveApi.md#believeEngineBelievePost) | **POST** /believe | The Believe Engine |
| [**getBiscuitBiscuitsBiscuitIdGet()**](InteractiveApi.md#getBiscuitBiscuitsBiscuitIdGet) | **GET** /biscuits/{biscuit_id} | Get a Specific Biscuit |
| [**getBiscuitsBiscuitsGet()**](InteractiveApi.md#getBiscuitsBiscuitsGet) | **GET** /biscuits | Biscuits as a Service |
| [**getCoachingPrincipleCoachingPrinciplesPrincipleIdGet()**](InteractiveApi.md#getCoachingPrincipleCoachingPrinciplesPrincipleIdGet) | **GET** /coaching/principles/{principle_id} | Get a Specific Coaching Principle |
| [**getCoachingPrinciplesCoachingPrinciplesGet()**](InteractiveApi.md#getCoachingPrinciplesCoachingPrinciplesGet) | **GET** /coaching/principles | Get Coaching Principles |
| [**getFreshBiscuitBiscuitsFreshGet()**](InteractiveApi.md#getFreshBiscuitBiscuitsFreshGet) | **GET** /biscuits/fresh | Get a Fresh Biscuit |
| [**getRandomPrincipleCoachingPrinciplesRandomGet()**](InteractiveApi.md#getRandomPrincipleCoachingPrinciplesRandomGet) | **GET** /coaching/principles/random | Get a Random Coaching Principle |
| [**pressConferencePressPost()**](InteractiveApi.md#pressConferencePressPost) | **POST** /press | Press Conference Simulator |
| [**reframeThoughtReframePost()**](InteractiveApi.md#reframeThoughtReframePost) | **POST** /reframe | Reframe Negative Thoughts |
| [**resolveConflictConflictsResolvePost()**](InteractiveApi.md#resolveConflictConflictsResolvePost) | **POST** /conflicts/resolve | Resolve Conflicts |


## `believeEngineBelievePost()`

```php
believeEngineBelievePost($believe_request): \OpenAPI\Client\Model\BelieveResponse
```

The Believe Engine

Submit your situation and receive Ted Lasso-style motivational guidance.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: HTTPBearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\InteractiveApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$believe_request = new \OpenAPI\Client\Model\BelieveRequest(); // \OpenAPI\Client\Model\BelieveRequest

try {
    $result = $apiInstance->believeEngineBelievePost($believe_request);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling InteractiveApi->believeEngineBelievePost: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **believe_request** | [**\OpenAPI\Client\Model\BelieveRequest**](../Model/BelieveRequest.md)|  | |

### Return type

[**\OpenAPI\Client\Model\BelieveResponse**](../Model/BelieveResponse.md)

### Authorization

[HTTPBearer](../../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getBiscuitBiscuitsBiscuitIdGet()`

```php
getBiscuitBiscuitsBiscuitIdGet($biscuit_id): \OpenAPI\Client\Model\Biscuit
```

Get a Specific Biscuit

Get a specific type of biscuit by ID.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: HTTPBearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\InteractiveApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$biscuit_id = 'biscuit_id_example'; // string

try {
    $result = $apiInstance->getBiscuitBiscuitsBiscuitIdGet($biscuit_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling InteractiveApi->getBiscuitBiscuitsBiscuitIdGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **biscuit_id** | **string**|  | |

### Return type

[**\OpenAPI\Client\Model\Biscuit**](../Model/Biscuit.md)

### Authorization

[HTTPBearer](../../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getBiscuitsBiscuitsGet()`

```php
getBiscuitsBiscuitsGet($skip, $limit): \OpenAPI\Client\Model\PaginatedResponseBiscuit
```

Biscuits as a Service

Get a paginated list of Ted's famous homemade biscuits! Each comes with a heartwarming message.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: HTTPBearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\InteractiveApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$skip = 0; // int | Number of items to skip (offset)
$limit = 20; // int | Maximum number of items to return (max: 100)

try {
    $result = $apiInstance->getBiscuitsBiscuitsGet($skip, $limit);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling InteractiveApi->getBiscuitsBiscuitsGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **skip** | **int**| Number of items to skip (offset) | [optional] [default to 0] |
| **limit** | **int**| Maximum number of items to return (max: 100) | [optional] [default to 20] |

### Return type

[**\OpenAPI\Client\Model\PaginatedResponseBiscuit**](../Model/PaginatedResponseBiscuit.md)

### Authorization

[HTTPBearer](../../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getCoachingPrincipleCoachingPrinciplesPrincipleIdGet()`

```php
getCoachingPrincipleCoachingPrinciplesPrincipleIdGet($principle_id): \OpenAPI\Client\Model\CoachingPrinciple
```

Get a Specific Coaching Principle

Get details about a specific coaching principle.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: HTTPBearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\InteractiveApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$principle_id = 'principle_id_example'; // string

try {
    $result = $apiInstance->getCoachingPrincipleCoachingPrinciplesPrincipleIdGet($principle_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling InteractiveApi->getCoachingPrincipleCoachingPrinciplesPrincipleIdGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **principle_id** | **string**|  | |

### Return type

[**\OpenAPI\Client\Model\CoachingPrinciple**](../Model/CoachingPrinciple.md)

### Authorization

[HTTPBearer](../../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getCoachingPrinciplesCoachingPrinciplesGet()`

```php
getCoachingPrinciplesCoachingPrinciplesGet($skip, $limit): \OpenAPI\Client\Model\PaginatedResponseCoachingPrinciple
```

Get Coaching Principles

Get a paginated list of Ted Lasso's core coaching principles and philosophy.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: HTTPBearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\InteractiveApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$skip = 0; // int | Number of items to skip (offset)
$limit = 20; // int | Maximum number of items to return (max: 100)

try {
    $result = $apiInstance->getCoachingPrinciplesCoachingPrinciplesGet($skip, $limit);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling InteractiveApi->getCoachingPrinciplesCoachingPrinciplesGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **skip** | **int**| Number of items to skip (offset) | [optional] [default to 0] |
| **limit** | **int**| Maximum number of items to return (max: 100) | [optional] [default to 20] |

### Return type

[**\OpenAPI\Client\Model\PaginatedResponseCoachingPrinciple**](../Model/PaginatedResponseCoachingPrinciple.md)

### Authorization

[HTTPBearer](../../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getFreshBiscuitBiscuitsFreshGet()`

```php
getFreshBiscuitBiscuitsFreshGet(): \OpenAPI\Client\Model\Biscuit
```

Get a Fresh Biscuit

Get a single fresh biscuit with a personalized message from Ted.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: HTTPBearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\InteractiveApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $result = $apiInstance->getFreshBiscuitBiscuitsFreshGet();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling InteractiveApi->getFreshBiscuitBiscuitsFreshGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**\OpenAPI\Client\Model\Biscuit**](../Model/Biscuit.md)

### Authorization

[HTTPBearer](../../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getRandomPrincipleCoachingPrinciplesRandomGet()`

```php
getRandomPrincipleCoachingPrinciplesRandomGet(): \OpenAPI\Client\Model\CoachingPrinciple
```

Get a Random Coaching Principle

Get a random coaching principle to inspire your day.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: HTTPBearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\InteractiveApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $result = $apiInstance->getRandomPrincipleCoachingPrinciplesRandomGet();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling InteractiveApi->getRandomPrincipleCoachingPrinciplesRandomGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**\OpenAPI\Client\Model\CoachingPrinciple**](../Model/CoachingPrinciple.md)

### Authorization

[HTTPBearer](../../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `pressConferencePressPost()`

```php
pressConferencePressPost($press_conference_request): \OpenAPI\Client\Model\PressConferenceResponse
```

Press Conference Simulator

Get Ted's response to press conference questions.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: HTTPBearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\InteractiveApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$press_conference_request = new \OpenAPI\Client\Model\PressConferenceRequest(); // \OpenAPI\Client\Model\PressConferenceRequest

try {
    $result = $apiInstance->pressConferencePressPost($press_conference_request);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling InteractiveApi->pressConferencePressPost: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **press_conference_request** | [**\OpenAPI\Client\Model\PressConferenceRequest**](../Model/PressConferenceRequest.md)|  | |

### Return type

[**\OpenAPI\Client\Model\PressConferenceResponse**](../Model/PressConferenceResponse.md)

### Authorization

[HTTPBearer](../../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `reframeThoughtReframePost()`

```php
reframeThoughtReframePost($reframe_request): \OpenAPI\Client\Model\ReframeResponse
```

Reframe Negative Thoughts

Transform negative thoughts into positive perspectives with Ted's help.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: HTTPBearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\InteractiveApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$reframe_request = new \OpenAPI\Client\Model\ReframeRequest(); // \OpenAPI\Client\Model\ReframeRequest

try {
    $result = $apiInstance->reframeThoughtReframePost($reframe_request);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling InteractiveApi->reframeThoughtReframePost: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **reframe_request** | [**\OpenAPI\Client\Model\ReframeRequest**](../Model/ReframeRequest.md)|  | |

### Return type

[**\OpenAPI\Client\Model\ReframeResponse**](../Model/ReframeResponse.md)

### Authorization

[HTTPBearer](../../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `resolveConflictConflictsResolvePost()`

```php
resolveConflictConflictsResolvePost($conflict_request): \OpenAPI\Client\Model\ConflictResolution
```

Resolve Conflicts

Get Ted Lasso-style advice for resolving conflicts.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: HTTPBearer
$config = OpenAPI\Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new OpenAPI\Client\Api\InteractiveApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$conflict_request = new \OpenAPI\Client\Model\ConflictRequest(); // \OpenAPI\Client\Model\ConflictRequest

try {
    $result = $apiInstance->resolveConflictConflictsResolvePost($conflict_request);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling InteractiveApi->resolveConflictConflictsResolvePost: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **conflict_request** | [**\OpenAPI\Client\Model\ConflictRequest**](../Model/ConflictRequest.md)|  | |

### Return type

[**\OpenAPI\Client\Model\ConflictResolution**](../Model/ConflictResolution.md)

### Authorization

[HTTPBearer](../../README.md#HTTPBearer)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
