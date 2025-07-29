# GameCenterAchievementLocalizationUpdateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**GameCenterAchievementLocalizationUpdateRequestDataAttributes**](GameCenterAchievementLocalizationUpdateRequestDataAttributes.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_achievement_localization_update_request_data import GameCenterAchievementLocalizationUpdateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterAchievementLocalizationUpdateRequestData from a JSON string
game_center_achievement_localization_update_request_data_instance = GameCenterAchievementLocalizationUpdateRequestData.from_json(json)
# print the JSON string representation of the object
print(GameCenterAchievementLocalizationUpdateRequestData.to_json())

# convert the object into a dict
game_center_achievement_localization_update_request_data_dict = game_center_achievement_localization_update_request_data_instance.to_dict()
# create an instance of GameCenterAchievementLocalizationUpdateRequestData from a dict
game_center_achievement_localization_update_request_data_from_dict = GameCenterAchievementLocalizationUpdateRequestData.from_dict(game_center_achievement_localization_update_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


