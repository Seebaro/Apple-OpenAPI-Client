# GameCenterAchievementLocalization


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**GameCenterAchievementLocalizationAttributes**](GameCenterAchievementLocalizationAttributes.md) |  | [optional] 
**relationships** | [**GameCenterAchievementLocalizationRelationships**](GameCenterAchievementLocalizationRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_achievement_localization import GameCenterAchievementLocalization

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterAchievementLocalization from a JSON string
game_center_achievement_localization_instance = GameCenterAchievementLocalization.from_json(json)
# print the JSON string representation of the object
print(GameCenterAchievementLocalization.to_json())

# convert the object into a dict
game_center_achievement_localization_dict = game_center_achievement_localization_instance.to_dict()
# create an instance of GameCenterAchievementLocalization from a dict
game_center_achievement_localization_from_dict = GameCenterAchievementLocalization.from_dict(game_center_achievement_localization_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


