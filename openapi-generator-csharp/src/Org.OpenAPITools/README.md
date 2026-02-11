# Created with Openapi Generator

<a id="cli"></a>
## Creating the library
Create a config.yaml file similar to what is below, then run the following powershell command to generate the library `java -jar "<path>/openapi-generator/modules/openapi-generator-cli/target/openapi-generator-cli.jar" generate -c config.yaml`

```yaml
generatorName: csharp
inputSpec: ./openapi.json
outputDir: out

# https://openapi-generator.tech/docs/generators/csharp
additionalProperties:
  packageGuid: '{A0FA20A7-A999-4BF7-960D-6CEE9E52E197}'

# https://openapi-generator.tech/docs/integrations/#github-integration
# gitHost:
# gitUserId:
# gitRepoId:

# https://openapi-generator.tech/docs/globals
# globalProperties:

# https://openapi-generator.tech/docs/customization/#inline-schema-naming
# inlineSchemaOptions:

# https://openapi-generator.tech/docs/customization/#name-mapping
# modelNameMappings:
# nameMappings:

# https://openapi-generator.tech/docs/customization/#openapi-normalizer
# openapiNormalizer:

# templateDir: https://openapi-generator.tech/docs/templating/#modifying-templates

# releaseNote:
```

<a id="usage"></a>
## Using the library in your project

```cs
using Microsoft.Extensions.Hosting;
using Microsoft.Extensions.DependencyInjection;
using Org.OpenAPITools.Api;
using Org.OpenAPITools.Client;
using Org.OpenAPITools.Model;
using Org.OpenAPITools.Extensions;

namespace YourProject
{
    public class Program
    {
        public static async Task Main(string[] args)
        {
            var host = CreateHostBuilder(args).Build();
            var api = host.Services.GetRequiredService<ICharactersApi>();
            ICreateCharacterCharactersPostApiResponse apiResponse = await api.CreateCharacterCharactersPostAsync("todo");
            Character? model = apiResponse.Ok();
        }

        public static IHostBuilder CreateHostBuilder(string[] args) => Host.CreateDefaultBuilder(args)
          .ConfigureApi((context, services, options) =>
          {
              // The type of token here depends on the api security specifications
              // Available token types are ApiKeyToken, BasicToken, BearerToken, HttpSigningToken, and OAuthToken.
              BearerToken token = new("<your token>");
              options.AddTokens(token);

              // optionally choose the method the tokens will be provided with, default is RateLimitProvider
              options.UseProvider<RateLimitProvider<BearerToken>, BearerToken>();

              options.ConfigureJsonOptions((jsonOptions) =>
              {
                  // your custom converters if any
              });

              options.AddApiHttpClients(client =>
              {
                  // client configuration
              }, builder =>
              {
                  builder
                      .AddRetryPolicy(2)
                      .AddTimeoutPolicy(TimeSpan.FromSeconds(5))
                      .AddCircuitBreakerPolicy(10, TimeSpan.FromSeconds(30));
                      // add whatever middleware you prefer
                  }
              );
          });
    }
}
```
<a id="questions"></a>
## Questions

- What about HttpRequest failures and retries?
  Configure Polly in the IHttpClientBuilder
- How are tokens used?
  Tokens are provided by a TokenProvider class. The default is RateLimitProvider which will perform client side rate limiting.
  Other providers can be used with the UseProvider method.
- Does an HttpRequest throw an error when the server response is not Ok?
  It depends how you made the request. If the return type is ApiResponse<T> no error will be thrown, though the Content property will be null.
  StatusCode and ReasonPhrase will contain information about the error.
  If the return type is T, then it will throw. If the return type is TOrDefault, it will return null.
- How do I validate requests and process responses?
  Use the provided On and After partial methods in the api classes.

## Api Information
- appName: Ted Lasso API
- appVersion: 2026-01-20
- appDescription:  ## Believe in the Power of Positivity!  A comprehensive API celebrating the wisdom, humor, and heart of Ted Lasso. Perfect for SDK demos showcasing various REST API features.  ### Features  - **CRUD Operations**: Full Create, Read, Update, Delete for all resources - **Rich Data Models**: Characters, Teams, Matches, Episodes, and Quotes - **Union Types (oneOf)**: Team Members demonstrate discriminated unions - **Interactive Endpoints**: Believe Engine, Conflict Resolution, and more - **SSE Streaming**: Real-time pep talks and match commentary - **Custom Easter Eggs**: Special HTTP status codes for fun  ### Core Resources  - **Characters**: Ted, Roy Kent, Rebecca, Jamie, and the whole gang - **Teams**: AFC Richmond, Manchester City, West Ham, and more - **Matches**: Historic matches with turning points and lessons learned - **Episodes**: Full episode guide with Ted&#39;s wisdom - **Quotes**: Searchable collection of memorable quotes  ### Interactive Endpoints  - **POST /believe**: The Believe Engine - get motivational guidance - **POST /conflicts/resolve**: Diamond Dogs-style conflict resolution - **POST /reframe**: Transform negative thoughts positively - **POST /press**: Press conference simulator - **GET /coaching/principles**: Ted&#39;s coaching philosophy - **GET /biscuits**: Biscuits as a Service!  ### Streaming (Server-Sent Events)  - **GET /pep-talk**: Pep talk from Ted (add &#x60;?stream&#x3D;true&#x60; for SSE) - **POST /matches/{id}/commentary/stream**: Live match commentary  ### WebSocket (Real-time)  - **WS /matches/live**: Live match simulation with real-time events (goals, fouls, cards, etc.) - **WS /ws/test**: Simple WebSocket echo test endpoint  ### Data Types Coverage  All common API data types are integrated across our models: - **Characters**: date (birth), float (height), decimal (salary), email, URL (profile image) - **Teams**: float (attendance, win %), decimal (budget), URL (website), email, GeoLocation (lat/long) - **Episodes**: date (air date), float (viewer rating, viewers in millions) - **Matches**: datetime, float (possession, temperature), decimal (revenue) - **Quotes**: float (popularity score), int (shares) - **File uploads**: POST /teams/{id}/logo for image uploads  ### Easter Eggs  - **429**: \&quot;Too Much Negativity\&quot; - when you need to be more positive - **403**: \&quot;Judgment Without Curiosity\&quot; - be curious, not judgmental - **418**: \&quot;I&#39;m a Believer!\&quot; - when you believe too much (is that possible?)  ### API Versioning  This API supports header-based versioning using date format (YYYY-MM-DD). Include one of these headers in your request:  - &#x60;X-API-Version: 2026-01-20&#x60; (preferred) - &#x60;API-Version: 2026-01-20&#x60;  Response headers will include: - &#x60;X-API-Version&#x60;: The version used for the request - &#x60;X-API-Supported-Versions&#x60;: List of all supported versions  If no version header is provided, the API defaults to the latest stable version.  *\&quot;Be curious, not judgmental.\&quot;* - Ted Lasso     

## Build
This C# SDK is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project.

- SDK version: 1.0.0
- Generator version: 7.19.0
- Build package: org.openapitools.codegen.languages.CSharpClientCodegen
