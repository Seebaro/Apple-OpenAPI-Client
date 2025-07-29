# GameCenterAchievement


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**GameCenterAchievementAttributes**](GameCenterAchievementAttributes.md) |  | [optional] 
**relationships** | [**GameCenterAchievementRelationships**](GameCenterAchievementRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_achievement import GameCenterAchievement

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterAchievement from a JSON string
game_center_achievement_instance = GameCenterAchievement.from_json(json)
# print the JSON string representation of the object
print(GameCenterAchievement.to_json())

# convert the object into a dict
game_center_achievement_dict = game_center_achievement_instance.to_dict()
# create an instance of GameCenterAchievement from a dict
game_center_achievement_from_dict = GameCenterAchievement.from_dict(game_center_achievement_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


