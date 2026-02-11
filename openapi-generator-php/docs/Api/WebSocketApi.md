# OpenAPI\Client\WebSocketApi

WebSocket endpoints for real-time bidirectional communication - Live match simulation

All URIs are relative to https://believe.cjav.dev, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**liveMatchWebsocket()**](WebSocketApi.md#liveMatchWebsocket) | **GET** /matches/live | Live Match Simulation WebSocket |
| [**websocketTest()**](WebSocketApi.md#websocketTest) | **GET** /ws/test | WebSocket Test Endpoint |


## `liveMatchWebsocket()`

```php
liveMatchWebsocket($home_team, $away_team, $speed, $excitement_level)
```

Live Match Simulation WebSocket

WebSocket endpoint for real-time live match simulation.  Connect to receive a stream of match events as they happen in a simulated football match.  ## Connection  Connect via WebSocket with optional query parameters to customize the simulation.  ## Example WebSocket URL  ``` ws://localhost:8000/matches/live?home_team=AFC%20Richmond&away_team=Manchester%20City&speed=2.0&excitement_level=7 ```  ## Server Messages  The server sends JSON messages with these types: - `match_start` - When the match begins - `match_event` - For each match event (goals, fouls, cards, etc.) - `match_end` - When the match concludes - `error` - If an error occurs - `pong` - Response to client ping  ## Client Messages  Send JSON to control the simulation: - `{\"action\": \"ping\"}` - Keep-alive, server responds with `{\"type\": \"pong\"}` - `{\"action\": \"pause\"}` - Pause the simulation - `{\"action\": \"resume\"}` - Resume a paused simulation - `{\"action\": \"set_speed\", \"speed\": 2.0}` - Change playback speed (0.1-10.0) - `{\"action\": \"get_status\"}` - Request current match status

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new OpenAPI\Client\Api\WebSocketApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$home_team = 'AFC Richmond'; // string | Home team name
$away_team = 'West Ham United'; // string | Away team name
$speed = 1.0; // float | Simulation speed multiplier (1.0 = real-time)
$excitement_level = 5; // int | How eventful the match should be (1=boring, 10=chaos)

try {
    $apiInstance->liveMatchWebsocket($home_team, $away_team, $speed, $excitement_level);
} catch (Exception $e) {
    echo 'Exception when calling WebSocketApi->liveMatchWebsocket: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **home_team** | **string**| Home team name | [optional] [default to &#39;AFC Richmond&#39;] |
| **away_team** | **string**| Away team name | [optional] [default to &#39;West Ham United&#39;] |
| **speed** | **float**| Simulation speed multiplier (1.0 &#x3D; real-time) | [optional] [default to 1.0] |
| **excitement_level** | **int**| How eventful the match should be (1&#x3D;boring, 10&#x3D;chaos) | [optional] [default to 5] |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `websocketTest()`

```php
websocketTest()
```

WebSocket Test Endpoint

Simple WebSocket test endpoint for connectivity testing.  Connect to test WebSocket functionality. The server will: 1. Send a welcome message on connection 2. Echo back any message you send  ## Example  ```javascript const ws = new WebSocket('ws://localhost:8000/ws/test'); ws.onmessage = (event) => console.log(event.data); ws.send('Hello!');  // Server responds with echo ```

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new OpenAPI\Client\Api\WebSocketApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

try {
    $apiInstance->websocketTest();
} catch (Exception $e) {
    echo 'Exception when calling WebSocketApi->websocketTest: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
