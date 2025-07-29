# GameCenterPlayerAchievementSubmissionCreateRequestDataAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**bundle_id** | **str** |  | 
**challenge_ids** | **List[str]** |  | [optional] 
**percentage_achieved** | **int** |  | 
**scoped_player_id** | **str** |  | 
**submitted_date** | **datetime** |  | [optional] 
**vendor_identifier** | **str** |  | 

## Example

```python
from openapi_client.models.game_center_player_achievement_submission_create_request_data_attributes import GameCenterPlayerAchievementSubmissionCreateRequestDataAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterPlayerAchievementSubmissionCreateRequestDataAttributes from a JSON string
game_center_player_achievement_submission_create_request_data_attributes_instance = GameCenterPlayerAchievementSubmissionCreateRequestDataAttributes.from_json(json)
# print the JSON string representation of the object
print(GameCenterPlayerAchievementSubmissionCreateRequestDataAttributes.to_json())

# convert the object into a dict
game_center_player_achievement_submission_create_request_data_attributes_dict = game_center_player_achievement_submission_create_request_data_attributes_instance.to_dict()
# create an instance of GameCenterPlayerAchievementSubmissionCreateRequestDataAttributes from a dict
game_center_player_achievement_submission_create_request_data_attributes_from_dict = GameCenterPlayerAchievementSubmissionCreateRequestDataAttributes.from_dict(game_center_player_achievement_submission_create_request_data_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


