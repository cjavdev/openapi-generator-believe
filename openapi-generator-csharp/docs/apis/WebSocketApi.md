# Org.OpenAPITools.Api.WebSocketApi

All URIs are relative to *https://believe.cjav.dev*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**LiveMatchWebsocket**](WebSocketApi.md#livematchwebsocket) | **GET** /matches/live | Live Match Simulation WebSocket |
| [**WebsocketTest**](WebSocketApi.md#websockettest) | **GET** /ws/test | WebSocket Test Endpoint |

<a id="livematchwebsocket"></a>
# **LiveMatchWebsocket**
> void LiveMatchWebsocket (string homeTeam = null, string awayTeam = null, decimal speed = null, int excitementLevel = null)

Live Match Simulation WebSocket

WebSocket endpoint for real-time live match simulation.  Connect to receive a stream of match events as they happen in a simulated football match.  ## Connection  Connect via WebSocket with optional query parameters to customize the simulation.  ## Example WebSocket URL  ``` ws://localhost:8000/matches/live?home_team=AFC%20Richmond&away_team=Manchester%20City&speed=2.0&excitement_level=7 ```  ## Server Messages  The server sends JSON messages with these types: - `match_start` - When the match begins - `match_event` - For each match event (goals, fouls, cards, etc.) - `match_end` - When the match concludes - `error` - If an error occurs - `pong` - Response to client ping  ## Client Messages  Send JSON to control the simulation: - `{\"action\": \"ping\"}` - Keep-alive, server responds with `{\"type\": \"pong\"}` - `{\"action\": \"pause\"}` - Pause the simulation - `{\"action\": \"resume\"}` - Resume a paused simulation - `{\"action\": \"set_speed\", \"speed\": 2.0}` - Change playback speed (0.1-10.0) - `{\"action\": \"get_status\"}` - Request current match status 


### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **homeTeam** | **string** | Home team name | [optional] [default to &quot;AFC Richmond&quot;] |
| **awayTeam** | **string** | Away team name | [optional] [default to &quot;West Ham United&quot;] |
| **speed** | **decimal** | Simulation speed multiplier (1.0 &#x3D; real-time) | [optional] [default to 1.0M] |
| **excitementLevel** | **int** | How eventful the match should be (1&#x3D;boring, 10&#x3D;chaos) | [optional] [default to 5] |

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
| **101** | Switching Protocols - WebSocket connection established |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

<a id="websockettest"></a>
# **WebsocketTest**
> void WebsocketTest ()

WebSocket Test Endpoint

Simple WebSocket test endpoint for connectivity testing.  Connect to test WebSocket functionality. The server will: 1. Send a welcome message on connection 2. Echo back any message you send  ## Example  ```javascript const ws = new WebSocket('ws://localhost:8000/ws/test'); ws.onmessage = (event) => console.log(event.data); ws.send('Hello!');  // Server responds with echo ``` 


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
| **101** | Switching Protocols - WebSocket connection established |  -  |

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

