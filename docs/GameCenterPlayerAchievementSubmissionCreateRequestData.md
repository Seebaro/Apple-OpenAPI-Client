# GameCenterPlayerAchievementSubmissionCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**GameCenterPlayerAchievementSubmissionCreateRequestDataAttributes**](GameCenterPlayerAchievementSubmissionCreateRequestDataAttributes.md) |  | 

## Example

```python
from openapi_client.models.game_center_player_achievement_submission_create_request_data import GameCenterPlayerAchievementSubmissionCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterPlayerAchievementSubmissionCreateRequestData from a JSON string
game_center_player_achievement_submission_create_request_data_instance = GameCenterPlayerAchievementSubmissionCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(GameCenterPlayerAchievementSubmissionCreateRequestData.to_json())

# convert the object into a dict
game_center_player_achievement_submission_create_request_data_dict = game_center_player_achievement_submission_create_request_data_instance.to_dict()
# create an instance of GameCenterPlayerAchievementSubmissionCreateRequestData from a dict
game_center_player_achievement_submission_create_request_data_from_dict = GameCenterPlayerAchievementSubmissionCreateRequestData.from_dict(game_center_player_achievement_submission_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


