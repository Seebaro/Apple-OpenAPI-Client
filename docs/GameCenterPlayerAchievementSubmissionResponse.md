# GameCenterPlayerAchievementSubmissionResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**GameCenterPlayerAchievementSubmission**](GameCenterPlayerAchievementSubmission.md) |  | 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.game_center_player_achievement_submission_response import GameCenterPlayerAchievementSubmissionResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterPlayerAchievementSubmissionResponse from a JSON string
game_center_player_achievement_submission_response_instance = GameCenterPlayerAchievementSubmissionResponse.from_json(json)
# print the JSON string representation of the object
print(GameCenterPlayerAchievementSubmissionResponse.to_json())

# convert the object into a dict
game_center_player_achievement_submission_response_dict = game_center_player_achievement_submission_response_instance.to_dict()
# create an instance of GameCenterPlayerAchievementSubmissionResponse from a dict
game_center_player_achievement_submission_response_from_dict = GameCenterPlayerAchievementSubmissionResponse.from_dict(game_center_player_achievement_submission_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


