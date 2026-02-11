# Org.OpenAPITools.Model.Team
Full team model with ID.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**CultureScore** | **int** | Team culture/morale score (0-100) | 
**FoundedYear** | **int** | Year the club was founded | 
**Id** | **string** | Unique identifier | 
**League** | **League** | Current league | 
**Name** | **string** | Team name | 
**Stadium** | **string** | Home stadium name | 
**Values** | [**TeamValues**](TeamValues.md) | Team&#39;s core values | 
**AnnualBudgetGbp** | **string** |  | [optional] 
**AverageAttendance** | **decimal** |  | [optional] 
**ContactEmail** | **string** |  | [optional] 
**IsActive** | **bool** | Whether the team is currently active | [optional] [default to true]
**Nickname** | **string** |  | [optional] 
**PrimaryColor** | **string** |  | [optional] 
**RivalTeams** | **List&lt;string&gt;** | List of rival team IDs | [optional] 
**SecondaryColor** | **string** |  | [optional] 
**StadiumLocation** | [**GeoLocation**](GeoLocation.md) |  | [optional] 
**Website** | **string** |  | [optional] 
**WinPercentage** | **decimal** |  | [optional] 

[[Back to Model list]](../../README.md#documentation-for-models) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to README]](../../README.md)

