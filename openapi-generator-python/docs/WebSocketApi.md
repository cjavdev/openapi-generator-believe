# openapi_client.WebSocketApi

All URIs are relative to *https://believe.cjav.dev*

Method | HTTP request | Description
------------- | ------------- | -------------
[**live_match_websocket**](WebSocketApi.md#live_match_websocket) | **GET** /matches/live | Live Match Simulation WebSocket
[**websocket_test**](WebSocketApi.md#websocket_test) | **GET** /ws/test | WebSocket Test Endpoint


# **live_match_websocket**
> live_match_websocket(home_team=home_team, away_team=away_team, speed=speed, excitement_level=excitement_level)

Live Match Simulation WebSocket

WebSocket endpoint for real-time live match simulation.

Connect to receive a stream of match events as they happen in a simulated football match.

## Connection

Connect via WebSocket with optional query parameters to customize the simulation.

## Example WebSocket URL

```
ws://localhost:8000/matches/live?home_team=AFC%20Richmond&away_team=Manchester%20City&speed=2.0&excitement_level=7
```

## Server Messages

The server sends JSON messages with these types:
- `match_start` - When the match begins
- `match_event` - For each match event (goals, fouls, cards, etc.)
- `match_end` - When the match concludes
- `error` - If an error occurs
- `pong` - Response to client ping

## Client Messages

Send JSON to control the simulation:
- `{"action": "ping"}` - Keep-alive, server responds with `{"type": "pong"}`
- `{"action": "pause"}` - Pause the simulation
- `{"action": "resume"}` - Resume a paused simulation
- `{"action": "set_speed", "speed": 2.0}` - Change playback speed (0.1-10.0)
- `{"action": "get_status"}` - Request current match status


### Example


```python
import openapi_client
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://believe.cjav.dev
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://believe.cjav.dev"
)


# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.WebSocketApi(api_client)
    home_team = 'AFC Richmond' # str | Home team name (optional) (default to 'AFC Richmond')
    away_team = 'West Ham United' # str | Away team name (optional) (default to 'West Ham United')
    speed = 1.0 # float | Simulation speed multiplier (1.0 = real-time) (optional) (default to 1.0)
    excitement_level = 5 # int | How eventful the match should be (1=boring, 10=chaos) (optional) (default to 5)

    try:
        # Live Match Simulation WebSocket
        api_instance.live_match_websocket(home_team=home_team, away_team=away_team, speed=speed, excitement_level=excitement_level)
    except Exception as e:
        print("Exception when calling WebSocketApi->live_match_websocket: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **home_team** | **str**| Home team name | [optional] [default to &#39;AFC Richmond&#39;]
 **away_team** | **str**| Away team name | [optional] [default to &#39;West Ham United&#39;]
 **speed** | **float**| Simulation speed multiplier (1.0 &#x3D; real-time) | [optional] [default to 1.0]
 **excitement_level** | **int**| How eventful the match should be (1&#x3D;boring, 10&#x3D;chaos) | [optional] [default to 5]

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**101** | Switching Protocols - WebSocket connection established |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **websocket_test**
> websocket_test()

WebSocket Test Endpoint

Simple WebSocket test endpoint for connectivity testing.

Connect to test WebSocket functionality. The server will:
1. Send a welcome message on connection
2. Echo back any message you send

## Example

```javascript
const ws = new WebSocket('ws://localhost:8000/ws/test');
ws.onmessage = (event) => console.log(event.data);
ws.send('Hello!');  // Server responds with echo
```


### Example


```python
import openapi_client
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://believe.cjav.dev
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "https://believe.cjav.dev"
)


# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.WebSocketApi(api_client)

    try:
        # WebSocket Test Endpoint
        api_instance.websocket_test()
    except Exception as e:
        print("Exception when calling WebSocketApi->websocket_test: %s\n" % e)
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

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**101** | Switching Protocols - WebSocket connection established |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

