# GameCenterPlayerAchievementSubmission


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**GameCenterPlayerAchievementSubmissionAttributes**](GameCenterPlayerAchievementSubmissionAttributes.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_player_achievement_submission import GameCenterPlayerAchievementSubmission

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterPlayerAchievementSubmission from a JSON string
game_center_player_achievement_submission_instance = GameCenterPlayerAchievementSubmission.from_json(json)
# print the JSON string representation of the object
print(GameCenterPlayerAchievementSubmission.to_json())

# convert the object into a dict
game_center_player_achievement_submission_dict = game_center_player_achievement_submission_instance.to_dict()
# create an instance of GameCenterPlayerAchievementSubmission from a dict
game_center_player_achievement_submission_from_dict = GameCenterPlayerAchievementSubmission.from_dict(game_center_player_achievement_submission_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


