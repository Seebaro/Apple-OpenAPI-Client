# GameCenterAchievementRelease


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**GameCenterAchievementReleaseAttributes**](GameCenterAchievementReleaseAttributes.md) |  | [optional] 
**relationships** | [**GameCenterAchievementReleaseRelationships**](GameCenterAchievementReleaseRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_achievement_release import GameCenterAchievementRelease

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterAchievementRelease from a JSON string
game_center_achievement_release_instance = GameCenterAchievementRelease.from_json(json)
# print the JSON string representation of the object
print(GameCenterAchievementRelease.to_json())

# convert the object into a dict
game_center_achievement_release_dict = game_center_achievement_release_instance.to_dict()
# create an instance of GameCenterAchievementRelease from a dict
game_center_achievement_release_from_dict = GameCenterAchievementRelease.from_dict(game_center_achievement_release_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


