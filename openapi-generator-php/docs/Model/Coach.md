# # Coach

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**certifications** | **string[]** | Coaching certifications and licenses | [optional]
**character_id** | **string** | ID of the character (references /characters/{id}) |
**id** | **string** | Unique identifier for this team membership |
**member_type** | **string** | Discriminator field indicating this is a coach | [optional] [default to 'coach']
**specialty** | [**\OpenAPI\Client\Model\CoachSpecialty**](CoachSpecialty.md) | Coaching specialty/role |
**team_id** | **string** | ID of the team they belong to |
**win_rate** | **float** |  | [optional]
**years_with_team** | **int** | Number of years with the current team |

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
