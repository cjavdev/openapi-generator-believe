# WebSocketApi

All URIs are relative to *https://believe.cjav.dev*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**liveMatchWebsocket**](WebSocketApi.md#liveMatchWebsocket) | **GET** /matches/live | Live Match Simulation WebSocket |
| [**websocketTest**](WebSocketApi.md#websocketTest) | **GET** /ws/test | WebSocket Test Endpoint |


<a id="liveMatchWebsocket"></a>
# **liveMatchWebsocket**
> liveMatchWebsocket(homeTeam, awayTeam, speed, excitementLevel)

Live Match Simulation WebSocket

WebSocket endpoint for real-time live match simulation.  Connect to receive a stream of match events as they happen in a simulated football match.  ## Connection  Connect via WebSocket with optional query parameters to customize the simulation.  ## Example WebSocket URL  &#x60;&#x60;&#x60; ws://localhost:8000/matches/live?home_team&#x3D;AFC%20Richmond&amp;away_team&#x3D;Manchester%20City&amp;speed&#x3D;2.0&amp;excitement_level&#x3D;7 &#x60;&#x60;&#x60;  ## Server Messages  The server sends JSON messages with these types: - &#x60;match_start&#x60; - When the match begins - &#x60;match_event&#x60; - For each match event (goals, fouls, cards, etc.) - &#x60;match_end&#x60; - When the match concludes - &#x60;error&#x60; - If an error occurs - &#x60;pong&#x60; - Response to client ping  ## Client Messages  Send JSON to control the simulation: - &#x60;{\&quot;action\&quot;: \&quot;ping\&quot;}&#x60; - Keep-alive, server responds with &#x60;{\&quot;type\&quot;: \&quot;pong\&quot;}&#x60; - &#x60;{\&quot;action\&quot;: \&quot;pause\&quot;}&#x60; - Pause the simulation - &#x60;{\&quot;action\&quot;: \&quot;resume\&quot;}&#x60; - Resume a paused simulation - &#x60;{\&quot;action\&quot;: \&quot;set_speed\&quot;, \&quot;speed\&quot;: 2.0}&#x60; - Change playback speed (0.1-10.0) - &#x60;{\&quot;action\&quot;: \&quot;get_status\&quot;}&#x60; - Request current match status 

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = WebSocketApi()
val homeTeam : kotlin.String = homeTeam_example // kotlin.String | Home team name
val awayTeam : kotlin.String = awayTeam_example // kotlin.String | Away team name
val speed : java.math.BigDecimal = 8.14 // java.math.BigDecimal | Simulation speed multiplier (1.0 = real-time)
val excitementLevel : kotlin.Int = 56 // kotlin.Int | How eventful the match should be (1=boring, 10=chaos)
try {
    apiInstance.liveMatchWebsocket(homeTeam, awayTeam, speed, excitementLevel)
} catch (e: ClientException) {
    println("4xx response calling WebSocketApi#liveMatchWebsocket")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WebSocketApi#liveMatchWebsocket")
    e.printStackTrace()
}
```

### Parameters
| **homeTeam** | **kotlin.String**| Home team name | [optional] [default to &quot;AFC Richmond&quot;] |
| **awayTeam** | **kotlin.String**| Away team name | [optional] [default to &quot;West Ham United&quot;] |
| **speed** | **java.math.BigDecimal**| Simulation speed multiplier (1.0 &#x3D; real-time) | [optional] [default to 1.0] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **excitementLevel** | **kotlin.Int**| How eventful the match should be (1&#x3D;boring, 10&#x3D;chaos) | [optional] [default to 5] |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="websocketTest"></a>
# **websocketTest**
> websocketTest()

WebSocket Test Endpoint

Simple WebSocket test endpoint for connectivity testing.  Connect to test WebSocket functionality. The server will: 1. Send a welcome message on connection 2. Echo back any message you send  ## Example  &#x60;&#x60;&#x60;javascript const ws &#x3D; new WebSocket(&#39;ws://localhost:8000/ws/test&#39;); ws.onmessage &#x3D; (event) &#x3D;&gt; console.log(event.data); ws.send(&#39;Hello!&#39;);  // Server responds with echo &#x60;&#x60;&#x60; 

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = WebSocketApi()
try {
    apiInstance.websocketTest()
} catch (e: ClientException) {
    println("4xx response calling WebSocketApi#websocketTest")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WebSocketApi#websocketTest")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

