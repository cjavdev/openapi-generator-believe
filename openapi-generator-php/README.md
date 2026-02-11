# OpenAPIClient-php


## Believe in the Power of Positivity!

A comprehensive API celebrating the wisdom, humor, and heart of Ted Lasso.
Perfect for SDK demos showcasing various REST API features.

### Features

- **CRUD Operations**: Full Create, Read, Update, Delete for all resources
- **Rich Data Models**: Characters, Teams, Matches, Episodes, and Quotes
- **Union Types (oneOf)**: Team Members demonstrate discriminated unions
- **Interactive Endpoints**: Believe Engine, Conflict Resolution, and more
- **SSE Streaming**: Real-time pep talks and match commentary
- **Custom Easter Eggs**: Special HTTP status codes for fun

### Core Resources

- **Characters**: Ted, Roy Kent, Rebecca, Jamie, and the whole gang
- **Teams**: AFC Richmond, Manchester City, West Ham, and more
- **Matches**: Historic matches with turning points and lessons learned
- **Episodes**: Full episode guide with Ted's wisdom
- **Quotes**: Searchable collection of memorable quotes

### Interactive Endpoints

- **POST /believe**: The Believe Engine - get motivational guidance
- **POST /conflicts/resolve**: Diamond Dogs-style conflict resolution
- **POST /reframe**: Transform negative thoughts positively
- **POST /press**: Press conference simulator
- **GET /coaching/principles**: Ted's coaching philosophy
- **GET /biscuits**: Biscuits as a Service!

### Streaming (Server-Sent Events)

- **GET /pep-talk**: Pep talk from Ted (add `?stream=true` for SSE)
- **POST /matches/{id}/commentary/stream**: Live match commentary

### WebSocket (Real-time)

- **WS /matches/live**: Live match simulation with real-time events (goals, fouls, cards, etc.)
- **WS /ws/test**: Simple WebSocket echo test endpoint

### Data Types Coverage

All common API data types are integrated across our models:
- **Characters**: date (birth), float (height), decimal (salary), email, URL (profile image)
- **Teams**: float (attendance, win %), decimal (budget), URL (website), email, GeoLocation (lat/long)
- **Episodes**: date (air date), float (viewer rating, viewers in millions)
- **Matches**: datetime, float (possession, temperature), decimal (revenue)
- **Quotes**: float (popularity score), int (shares)
- **File uploads**: POST /teams/{id}/logo for image uploads

### Easter Eggs

- **429**: \"Too Much Negativity\" - when you need to be more positive
- **403**: \"Judgment Without Curiosity\" - be curious, not judgmental
- **418**: \"I'm a Believer!\" - when you believe too much (is that possible?)

### API Versioning

This API supports header-based versioning using date format (YYYY-MM-DD).
Include one of these headers in your request:

- `X-API-Version: 2026-01-20` (preferred)
- `API-Version: 2026-01-20`

Response headers will include:
- `X-API-Version`: The version used for the request
- `X-API-Supported-Versions`: List of all supported versions

If no version header is provided, the API defaults to the latest stable version.

*\"Be curious, not judgmental.\"* - Ted Lasso
    


## Installation & Usage

### Requirements

PHP 8.1 and later.

### Composer

To install the bindings via [Composer](https://getcomposer.org/), add the following to `composer.json`:

```json
{
  "repositories": [
    {
      "type": "vcs",
      "url": "https://github.com/GIT_USER_ID/GIT_REPO_ID.git"
    }
  ],
  "require": {
    "GIT_USER_ID/GIT_REPO_ID": "*@dev"
  }
}
```

Then run `composer install`

### Manual Installation

Download the files and include `autoload.php`:

```php
<?php
require_once('/path/to/OpenAPIClient-php/vendor/autoload.php');
```

## Getting Started

Please follow the [installation procedure](#installation--usage) and then run the following:

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

## API Endpoints

All URIs are relative to *https://believe.cjav.dev*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*CharactersApi* | [**createCharacterCharactersPost**](docs/Api/CharactersApi.md#createcharactercharacterspost) | **POST** /characters | Create a new character
*CharactersApi* | [**deleteCharacterCharactersCharacterIdDelete**](docs/Api/CharactersApi.md#deletecharactercharacterscharacteriddelete) | **DELETE** /characters/{character_id} | Delete a character
*CharactersApi* | [**getCharacterCharactersCharacterIdGet**](docs/Api/CharactersApi.md#getcharactercharacterscharacteridget) | **GET** /characters/{character_id} | Get a character by ID
*CharactersApi* | [**getCharacterQuotesCharactersCharacterIdQuotesGet**](docs/Api/CharactersApi.md#getcharacterquotescharacterscharacteridquotesget) | **GET** /characters/{character_id}/quotes | Get character&#39;s signature quotes
*CharactersApi* | [**listCharactersCharactersGet**](docs/Api/CharactersApi.md#listcharacterscharactersget) | **GET** /characters | List all characters
*CharactersApi* | [**updateCharacterCharactersCharacterIdPatch**](docs/Api/CharactersApi.md#updatecharactercharacterscharacteridpatch) | **PATCH** /characters/{character_id} | Update a character
*EpisodesApi* | [**createEpisodeEpisodesPost**](docs/Api/EpisodesApi.md#createepisodeepisodespost) | **POST** /episodes | Create a new episode
*EpisodesApi* | [**deleteEpisodeEpisodesEpisodeIdDelete**](docs/Api/EpisodesApi.md#deleteepisodeepisodesepisodeiddelete) | **DELETE** /episodes/{episode_id} | Delete an episode
*EpisodesApi* | [**getEpisodeEpisodesEpisodeIdGet**](docs/Api/EpisodesApi.md#getepisodeepisodesepisodeidget) | **GET** /episodes/{episode_id} | Get an episode by ID
*EpisodesApi* | [**getEpisodeWisdomEpisodesEpisodeIdWisdomGet**](docs/Api/EpisodesApi.md#getepisodewisdomepisodesepisodeidwisdomget) | **GET** /episodes/{episode_id}/wisdom | Get episode wisdom
*EpisodesApi* | [**getSeasonEpisodesEpisodesSeasonsSeasonNumberGet**](docs/Api/EpisodesApi.md#getseasonepisodesepisodesseasonsseasonnumberget) | **GET** /episodes/seasons/{season_number} | Get all episodes from a season
*EpisodesApi* | [**listEpisodesEpisodesGet**](docs/Api/EpisodesApi.md#listepisodesepisodesget) | **GET** /episodes | List all episodes
*EpisodesApi* | [**updateEpisodeEpisodesEpisodeIdPatch**](docs/Api/EpisodesApi.md#updateepisodeepisodesepisodeidpatch) | **PATCH** /episodes/{episode_id} | Update an episode
*InteractiveApi* | [**believeEngineBelievePost**](docs/Api/InteractiveApi.md#believeenginebelievepost) | **POST** /believe | The Believe Engine
*InteractiveApi* | [**getBiscuitBiscuitsBiscuitIdGet**](docs/Api/InteractiveApi.md#getbiscuitbiscuitsbiscuitidget) | **GET** /biscuits/{biscuit_id} | Get a Specific Biscuit
*InteractiveApi* | [**getBiscuitsBiscuitsGet**](docs/Api/InteractiveApi.md#getbiscuitsbiscuitsget) | **GET** /biscuits | Biscuits as a Service
*InteractiveApi* | [**getCoachingPrincipleCoachingPrinciplesPrincipleIdGet**](docs/Api/InteractiveApi.md#getcoachingprinciplecoachingprinciplesprincipleidget) | **GET** /coaching/principles/{principle_id} | Get a Specific Coaching Principle
*InteractiveApi* | [**getCoachingPrinciplesCoachingPrinciplesGet**](docs/Api/InteractiveApi.md#getcoachingprinciplescoachingprinciplesget) | **GET** /coaching/principles | Get Coaching Principles
*InteractiveApi* | [**getFreshBiscuitBiscuitsFreshGet**](docs/Api/InteractiveApi.md#getfreshbiscuitbiscuitsfreshget) | **GET** /biscuits/fresh | Get a Fresh Biscuit
*InteractiveApi* | [**getRandomPrincipleCoachingPrinciplesRandomGet**](docs/Api/InteractiveApi.md#getrandomprinciplecoachingprinciplesrandomget) | **GET** /coaching/principles/random | Get a Random Coaching Principle
*InteractiveApi* | [**pressConferencePressPost**](docs/Api/InteractiveApi.md#pressconferencepresspost) | **POST** /press | Press Conference Simulator
*InteractiveApi* | [**reframeThoughtReframePost**](docs/Api/InteractiveApi.md#reframethoughtreframepost) | **POST** /reframe | Reframe Negative Thoughts
*InteractiveApi* | [**resolveConflictConflictsResolvePost**](docs/Api/InteractiveApi.md#resolveconflictconflictsresolvepost) | **POST** /conflicts/resolve | Resolve Conflicts
*MatchesApi* | [**createMatchMatchesPost**](docs/Api/MatchesApi.md#creatematchmatchespost) | **POST** /matches | Create a new match
*MatchesApi* | [**deleteMatchMatchesMatchIdDelete**](docs/Api/MatchesApi.md#deletematchmatchesmatchiddelete) | **DELETE** /matches/{match_id} | Delete a match
*MatchesApi* | [**getMatchLessonMatchesMatchIdLessonGet**](docs/Api/MatchesApi.md#getmatchlessonmatchesmatchidlessonget) | **GET** /matches/{match_id}/lesson | Get match lesson
*MatchesApi* | [**getMatchMatchesMatchIdGet**](docs/Api/MatchesApi.md#getmatchmatchesmatchidget) | **GET** /matches/{match_id} | Get a match by ID
*MatchesApi* | [**getTurningPointsMatchesMatchIdTurningPointsGet**](docs/Api/MatchesApi.md#getturningpointsmatchesmatchidturningpointsget) | **GET** /matches/{match_id}/turning-points | Get match turning points
*MatchesApi* | [**listMatchesMatchesGet**](docs/Api/MatchesApi.md#listmatchesmatchesget) | **GET** /matches | List all matches
*MatchesApi* | [**updateMatchMatchesMatchIdPatch**](docs/Api/MatchesApi.md#updatematchmatchesmatchidpatch) | **PATCH** /matches/{match_id} | Update a match
*QuotesApi* | [**createQuoteQuotesPost**](docs/Api/QuotesApi.md#createquotequotespost) | **POST** /quotes | Create a new quote
*QuotesApi* | [**deleteQuoteQuotesQuoteIdDelete**](docs/Api/QuotesApi.md#deletequotequotesquoteiddelete) | **DELETE** /quotes/{quote_id} | Delete a quote
*QuotesApi* | [**getCharacterQuotesQuotesCharactersCharacterIdGet**](docs/Api/QuotesApi.md#getcharacterquotesquotescharacterscharacteridget) | **GET** /quotes/characters/{character_id} | Get all quotes by a character
*QuotesApi* | [**getQuoteQuotesQuoteIdGet**](docs/Api/QuotesApi.md#getquotequotesquoteidget) | **GET** /quotes/{quote_id} | Get a quote by ID
*QuotesApi* | [**getQuotesByThemeQuotesThemesThemeGet**](docs/Api/QuotesApi.md#getquotesbythemequotesthemesthemeget) | **GET** /quotes/themes/{theme} | Get quotes by theme
*QuotesApi* | [**getRandomQuoteQuotesRandomGet**](docs/Api/QuotesApi.md#getrandomquotequotesrandomget) | **GET** /quotes/random | Get a random quote
*QuotesApi* | [**listQuotesQuotesGet**](docs/Api/QuotesApi.md#listquotesquotesget) | **GET** /quotes | List all quotes
*QuotesApi* | [**updateQuoteQuotesQuoteIdPatch**](docs/Api/QuotesApi.md#updatequotequotesquoteidpatch) | **PATCH** /quotes/{quote_id} | Update a quote
*RootApi* | [**healthCheckHealthGet**](docs/Api/RootApi.md#healthcheckhealthget) | **GET** /health | Health Check
*RootApi* | [**rootGet**](docs/Api/RootApi.md#rootget) | **GET** / | Welcome to the Ted Lasso API
*RootApi* | [**versionInfoVersionGet**](docs/Api/RootApi.md#versioninfoversionget) | **GET** /version | API Version Information
*StreamingApi* | [**getPepTalkPepTalkGet**](docs/Api/StreamingApi.md#getpeptalkpeptalkget) | **GET** /pep-talk | Get a Pep Talk
*StreamingApi* | [**streamMatchCommentaryMatchesMatchIdCommentaryStreamPost**](docs/Api/StreamingApi.md#streammatchcommentarymatchesmatchidcommentarystreampost) | **POST** /matches/{match_id}/commentary/stream | Stream Match Commentary
*StreamingApi* | [**testStreamStreamTestGet**](docs/Api/StreamingApi.md#teststreamstreamtestget) | **GET** /stream/test | Test SSE Connection
*TeamMembersApi* | [**createTeamMemberTeamMembersPost**](docs/Api/TeamMembersApi.md#createteammemberteammemberspost) | **POST** /team-members | Create a new team member
*TeamMembersApi* | [**deleteTeamMemberTeamMembersMemberIdDelete**](docs/Api/TeamMembersApi.md#deleteteammemberteammembersmemberiddelete) | **DELETE** /team-members/{member_id} | Delete a team member
*TeamMembersApi* | [**getTeamMemberTeamMembersMemberIdGet**](docs/Api/TeamMembersApi.md#getteammemberteammembersmemberidget) | **GET** /team-members/{member_id} | Get a team member by ID
*TeamMembersApi* | [**listCoachesTeamMembersCoachesGet**](docs/Api/TeamMembersApi.md#listcoachesteammemberscoachesget) | **GET** /team-members/coaches/ | List all coaches
*TeamMembersApi* | [**listPlayersTeamMembersPlayersGet**](docs/Api/TeamMembersApi.md#listplayersteammembersplayersget) | **GET** /team-members/players/ | List all players
*TeamMembersApi* | [**listStaffTeamMembersStaffGet**](docs/Api/TeamMembersApi.md#liststaffteammembersstaffget) | **GET** /team-members/staff/ | List all staff (non-player, non-coach)
*TeamMembersApi* | [**listTeamMembersTeamMembersGet**](docs/Api/TeamMembersApi.md#listteammembersteammembersget) | **GET** /team-members | List all team members
*TeamMembersApi* | [**updateTeamMemberTeamMembersMemberIdPatch**](docs/Api/TeamMembersApi.md#updateteammemberteammembersmemberidpatch) | **PATCH** /team-members/{member_id} | Update a team member
*TeamsApi* | [**createTeamTeamsPost**](docs/Api/TeamsApi.md#createteamteamspost) | **POST** /teams | Create a new team
*TeamsApi* | [**deleteTeamLogoTeamsTeamIdLogoFileIdDelete**](docs/Api/TeamsApi.md#deleteteamlogoteamsteamidlogofileiddelete) | **DELETE** /teams/{team_id}/logo/{file_id} | Delete team logo
*TeamsApi* | [**deleteTeamTeamsTeamIdDelete**](docs/Api/TeamsApi.md#deleteteamteamsteamiddelete) | **DELETE** /teams/{team_id} | Delete a team
*TeamsApi* | [**downloadTeamLogoTeamsTeamIdLogoFileIdGet**](docs/Api/TeamsApi.md#downloadteamlogoteamsteamidlogofileidget) | **GET** /teams/{team_id}/logo/{file_id} | Download team logo
*TeamsApi* | [**getTeamCultureTeamsTeamIdCultureGet**](docs/Api/TeamsApi.md#getteamcultureteamsteamidcultureget) | **GET** /teams/{team_id}/culture | Get team culture details
*TeamsApi* | [**getTeamRivalsTeamsTeamIdRivalsGet**](docs/Api/TeamsApi.md#getteamrivalsteamsteamidrivalsget) | **GET** /teams/{team_id}/rivals | Get team&#39;s rivals
*TeamsApi* | [**getTeamTeamsTeamIdGet**](docs/Api/TeamsApi.md#getteamteamsteamidget) | **GET** /teams/{team_id} | Get a team by ID
*TeamsApi* | [**listTeamLogosTeamsTeamIdLogosGet**](docs/Api/TeamsApi.md#listteamlogosteamsteamidlogosget) | **GET** /teams/{team_id}/logos | List team logos
*TeamsApi* | [**listTeamsTeamsGet**](docs/Api/TeamsApi.md#listteamsteamsget) | **GET** /teams | List all teams
*TeamsApi* | [**updateTeamTeamsTeamIdPatch**](docs/Api/TeamsApi.md#updateteamteamsteamidpatch) | **PATCH** /teams/{team_id} | Update a team
*TeamsApi* | [**uploadTeamLogoTeamsTeamIdLogoPost**](docs/Api/TeamsApi.md#uploadteamlogoteamsteamidlogopost) | **POST** /teams/{team_id}/logo | Upload team logo
*WebSocketApi* | [**liveMatchWebsocket**](docs/Api/WebSocketApi.md#livematchwebsocket) | **GET** /matches/live | Live Match Simulation WebSocket
*WebSocketApi* | [**websocketTest**](docs/Api/WebSocketApi.md#websockettest) | **GET** /ws/test | WebSocket Test Endpoint
*WebhooksApi* | [**deleteWebhookWebhooksWebhookIdDelete**](docs/Api/WebhooksApi.md#deletewebhookwebhookswebhookiddelete) | **DELETE** /webhooks/{webhook_id} | Delete a webhook
*WebhooksApi* | [**getWebhookWebhooksWebhookIdGet**](docs/Api/WebhooksApi.md#getwebhookwebhookswebhookidget) | **GET** /webhooks/{webhook_id} | Get a webhook
*WebhooksApi* | [**listWebhooksWebhooksGet**](docs/Api/WebhooksApi.md#listwebhookswebhooksget) | **GET** /webhooks | List registered webhooks
*WebhooksApi* | [**registerWebhookWebhooksPost**](docs/Api/WebhooksApi.md#registerwebhookwebhookspost) | **POST** /webhooks | Register a webhook endpoint
*WebhooksApi* | [**triggerEventWebhooksTriggerPost**](docs/Api/WebhooksApi.md#triggereventwebhookstriggerpost) | **POST** /webhooks/trigger | Trigger a webhook event

## Models

- [AnnualBudgetGbp](docs/Model/AnnualBudgetGbp.md)
- [AnnualBudgetGbp1](docs/Model/AnnualBudgetGbp1.md)
- [BelieveRequest](docs/Model/BelieveRequest.md)
- [BelieveResponse](docs/Model/BelieveResponse.md)
- [Biscuit](docs/Model/Biscuit.md)
- [BiscuitType](docs/Model/BiscuitType.md)
- [Character](docs/Model/Character.md)
- [CharacterCreate](docs/Model/CharacterCreate.md)
- [CharacterRole](docs/Model/CharacterRole.md)
- [CharacterUpdate](docs/Model/CharacterUpdate.md)
- [Coach](docs/Model/Coach.md)
- [CoachBase](docs/Model/CoachBase.md)
- [CoachSpecialty](docs/Model/CoachSpecialty.md)
- [CoachUpdate](docs/Model/CoachUpdate.md)
- [CoachingPrinciple](docs/Model/CoachingPrinciple.md)
- [ConflictRequest](docs/Model/ConflictRequest.md)
- [ConflictResolution](docs/Model/ConflictResolution.md)
- [ConflictType](docs/Model/ConflictType.md)
- [DataInner](docs/Model/DataInner.md)
- [DataInner1](docs/Model/DataInner1.md)
- [EmotionalStats](docs/Model/EmotionalStats.md)
- [Episode](docs/Model/Episode.md)
- [EpisodeCreate](docs/Model/EpisodeCreate.md)
- [EpisodeUpdate](docs/Model/EpisodeUpdate.md)
- [EquipmentManager](docs/Model/EquipmentManager.md)
- [EquipmentManagerBase](docs/Model/EquipmentManagerBase.md)
- [EquipmentManagerUpdate](docs/Model/EquipmentManagerUpdate.md)
- [FileUploadResponse](docs/Model/FileUploadResponse.md)
- [GeoLocation](docs/Model/GeoLocation.md)
- [GrowthArc](docs/Model/GrowthArc.md)
- [HTTPValidationError](docs/Model/HTTPValidationError.md)
- [League](docs/Model/League.md)
- [LocationInner](docs/Model/LocationInner.md)
- [Match](docs/Model/Match.md)
- [MatchCommentaryEvent](docs/Model/MatchCommentaryEvent.md)
- [MatchCompletedData](docs/Model/MatchCompletedData.md)
- [MatchCompletedEvent](docs/Model/MatchCompletedEvent.md)
- [MatchCompletedPayload](docs/Model/MatchCompletedPayload.md)
- [MatchCreate](docs/Model/MatchCreate.md)
- [MatchResult](docs/Model/MatchResult.md)
- [MatchType](docs/Model/MatchType.md)
- [MatchUpdate](docs/Model/MatchUpdate.md)
- [MedicalSpecialty](docs/Model/MedicalSpecialty.md)
- [MedicalStaff](docs/Model/MedicalStaff.md)
- [MedicalStaffBase](docs/Model/MedicalStaffBase.md)
- [MedicalStaffUpdate](docs/Model/MedicalStaffUpdate.md)
- [Member](docs/Model/Member.md)
- [MemberType](docs/Model/MemberType.md)
- [PaginatedResponseAnnotatedUnionPlayerCoachMedicalStaffEquipmentManagerFieldInfoAnnotationNoneTypeRequiredTrueDiscriminatorMemberType](docs/Model/PaginatedResponseAnnotatedUnionPlayerCoachMedicalStaffEquipmentManagerFieldInfoAnnotationNoneTypeRequiredTrueDiscriminatorMemberType.md)
- [PaginatedResponseBiscuit](docs/Model/PaginatedResponseBiscuit.md)
- [PaginatedResponseCharacter](docs/Model/PaginatedResponseCharacter.md)
- [PaginatedResponseCoach](docs/Model/PaginatedResponseCoach.md)
- [PaginatedResponseCoachingPrinciple](docs/Model/PaginatedResponseCoachingPrinciple.md)
- [PaginatedResponseEpisode](docs/Model/PaginatedResponseEpisode.md)
- [PaginatedResponseMatch](docs/Model/PaginatedResponseMatch.md)
- [PaginatedResponsePlayer](docs/Model/PaginatedResponsePlayer.md)
- [PaginatedResponseQuote](docs/Model/PaginatedResponseQuote.md)
- [PaginatedResponseTeam](docs/Model/PaginatedResponseTeam.md)
- [PaginatedResponseUnionMedicalStaffEquipmentManager](docs/Model/PaginatedResponseUnionMedicalStaffEquipmentManager.md)
- [PepTalkChunk](docs/Model/PepTalkChunk.md)
- [PepTalkResponse](docs/Model/PepTalkResponse.md)
- [Player](docs/Model/Player.md)
- [PlayerBase](docs/Model/PlayerBase.md)
- [PlayerUpdate](docs/Model/PlayerUpdate.md)
- [Position](docs/Model/Position.md)
- [PressConferenceRequest](docs/Model/PressConferenceRequest.md)
- [PressConferenceResponse](docs/Model/PressConferenceResponse.md)
- [Quote](docs/Model/Quote.md)
- [QuoteCreate](docs/Model/QuoteCreate.md)
- [QuoteMoment](docs/Model/QuoteMoment.md)
- [QuoteTheme](docs/Model/QuoteTheme.md)
- [QuoteUpdate](docs/Model/QuoteUpdate.md)
- [ReframeRequest](docs/Model/ReframeRequest.md)
- [ReframeResponse](docs/Model/ReframeResponse.md)
- [RegisteredWebhook](docs/Model/RegisteredWebhook.md)
- [ResponseCreateTeamMemberTeamMembersPost](docs/Model/ResponseCreateTeamMemberTeamMembersPost.md)
- [ResponseGetTeamMemberTeamMembersMemberIdGet](docs/Model/ResponseGetTeamMemberTeamMembersMemberIdGet.md)
- [ResponseUpdateTeamMemberTeamMembersMemberIdPatch](docs/Model/ResponseUpdateTeamMemberTeamMembersMemberIdPatch.md)
- [SalaryGbp](docs/Model/SalaryGbp.md)
- [SalaryGbp1](docs/Model/SalaryGbp1.md)
- [SituationType](docs/Model/SituationType.md)
- [Team](docs/Model/Team.md)
- [TeamCreate](docs/Model/TeamCreate.md)
- [TeamMemberTransferredData](docs/Model/TeamMemberTransferredData.md)
- [TeamMemberTransferredEvent](docs/Model/TeamMemberTransferredEvent.md)
- [TeamMemberTransferredPayload](docs/Model/TeamMemberTransferredPayload.md)
- [TeamUpdate](docs/Model/TeamUpdate.md)
- [TeamValues](docs/Model/TeamValues.md)
- [TestStreamChunk](docs/Model/TestStreamChunk.md)
- [TicketRevenueGbp](docs/Model/TicketRevenueGbp.md)
- [TicketRevenueGbp1](docs/Model/TicketRevenueGbp1.md)
- [TriggerEventRequest](docs/Model/TriggerEventRequest.md)
- [TriggerEventRequestPayload](docs/Model/TriggerEventRequestPayload.md)
- [TriggerEventResponse](docs/Model/TriggerEventResponse.md)
- [TurningPoint](docs/Model/TurningPoint.md)
- [Updates](docs/Model/Updates.md)
- [ValidationError](docs/Model/ValidationError.md)
- [WebSocketClientGetStatusMessage](docs/Model/WebSocketClientGetStatusMessage.md)
- [WebSocketClientMessage](docs/Model/WebSocketClientMessage.md)
- [WebSocketClientPauseMessage](docs/Model/WebSocketClientPauseMessage.md)
- [WebSocketClientPingMessage](docs/Model/WebSocketClientPingMessage.md)
- [WebSocketClientResumeMessage](docs/Model/WebSocketClientResumeMessage.md)
- [WebSocketClientSetSpeedMessage](docs/Model/WebSocketClientSetSpeedMessage.md)
- [WebSocketErrorMessage](docs/Model/WebSocketErrorMessage.md)
- [WebSocketLiveMatchEvent](docs/Model/WebSocketLiveMatchEvent.md)
- [WebSocketMatchEndMessage](docs/Model/WebSocketMatchEndMessage.md)
- [WebSocketMatchEventMessage](docs/Model/WebSocketMatchEventMessage.md)
- [WebSocketMatchScore](docs/Model/WebSocketMatchScore.md)
- [WebSocketMatchStartMessage](docs/Model/WebSocketMatchStartMessage.md)
- [WebSocketMatchStats](docs/Model/WebSocketMatchStats.md)
- [WebSocketPlayerInfo](docs/Model/WebSocketPlayerInfo.md)
- [WebSocketPongMessage](docs/Model/WebSocketPongMessage.md)
- [WebSocketServerMessage](docs/Model/WebSocketServerMessage.md)
- [WebSocketTestEchoMessage](docs/Model/WebSocketTestEchoMessage.md)
- [WebSocketTestServerMessage](docs/Model/WebSocketTestServerMessage.md)
- [WebSocketTestWelcomeMessage](docs/Model/WebSocketTestWelcomeMessage.md)
- [WebhookDeliveryResult](docs/Model/WebhookDeliveryResult.md)
- [WebhookEvent](docs/Model/WebhookEvent.md)
- [WebhookRegistrationRequest](docs/Model/WebhookRegistrationRequest.md)
- [WebhookRegistrationResponse](docs/Model/WebhookRegistrationResponse.md)

## Authorization

Authentication schemes defined for the API:
### HTTPBearer

- **Type**: Bearer authentication

## Tests

To run the tests, use:

```bash
composer install
vendor/bin/phpunit
```

## Author

believe@afcrichmond.com

## About this package

This PHP package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:

- API version: `2026-01-20`
    - Generator version: `7.19.0`
- Build package: `org.openapitools.codegen.languages.PhpClientCodegen`
