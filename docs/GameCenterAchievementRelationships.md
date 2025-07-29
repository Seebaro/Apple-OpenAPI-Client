# GameCenterAchievementRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**game_center_detail** | [**GameCenterAchievementReleaseRelationshipsGameCenterDetail**](GameCenterAchievementReleaseRelationshipsGameCenterDetail.md) |  | [optional] 
**game_center_group** | [**GameCenterAchievementRelationshipsGameCenterGroup**](GameCenterAchievementRelationshipsGameCenterGroup.md) |  | [optional] 
**group_achievement** | [**GameCenterAchievementRelationshipsGroupAchievement**](GameCenterAchievementRelationshipsGroupAchievement.md) |  | [optional] 
**localizations** | [**GameCenterAchievementRelationshipsLocalizations**](GameCenterAchievementRelationshipsLocalizations.md) |  | [optional] 
**releases** | [**GameCenterAchievementRelationshipsReleases**](GameCenterAchievementRelationshipsReleases.md) |  | [optional] 
**activity** | [**GameCenterAchievementRelationshipsActivity**](GameCenterAchievementRelationshipsActivity.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_achievement_relationships import GameCenterAchievementRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterAchievementRelationships from a JSON string
game_center_achievement_relationships_instance = GameCenterAchievementRelationships.from_json(json)
# print the JSON string representation of the object
print(GameCenterAchievementRelationships.to_json())

# convert the object into a dict
game_center_achievement_relationships_dict = game_center_achievement_relationships_instance.to_dict()
# create an instance of GameCenterAchievementRelationships from a dict
game_center_achievement_relationships_from_dict = GameCenterAchievementRelationships.from_dict(game_center_achievement_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


