# # TeamCreate

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**annual_budget_gbp** | [**\OpenAPI\Client\Model\AnnualBudgetGbp**](AnnualBudgetGbp.md) |  | [optional]
**average_attendance** | **float** |  | [optional]
**contact_email** | **string** |  | [optional]
**culture_score** | **int** | Team culture/morale score (0-100) |
**founded_year** | **int** | Year the club was founded |
**is_active** | **bool** | Whether the team is currently active | [optional] [default to true]
**league** | [**\OpenAPI\Client\Model\League**](League.md) | Current league |
**name** | **string** | Team name |
**nickname** | **string** |  | [optional]
**primary_color** | **string** |  | [optional]
**rival_teams** | **string[]** | List of rival team IDs | [optional]
**secondary_color** | **string** |  | [optional]
**stadium** | **string** | Home stadium name |
**stadium_location** | [**\OpenAPI\Client\Model\GeoLocation**](GeoLocation.md) |  | [optional]
**values** | [**\OpenAPI\Client\Model\TeamValues**](TeamValues.md) | Team&#39;s core values |
**website** | **string** |  | [optional]
**win_percentage** | **float** |  | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
