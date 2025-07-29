# GameCenterAchievementRelationshipsGroupAchievement


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**data** | [**GameCenterAchievementLocalizationRelationshipsGameCenterAchievementData**](GameCenterAchievementLocalizationRelationshipsGameCenterAchievementData.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_achievement_relationships_group_achievement import GameCenterAchievementRelationshipsGroupAchievement

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterAchievementRelationshipsGroupAchievement from a JSON string
game_center_achievement_relationships_group_achievement_instance = GameCenterAchievementRelationshipsGroupAchievement.from_json(json)
# print the JSON string representation of the object
print(GameCenterAchievementRelationshipsGroupAchievement.to_json())

# convert the object into a dict
game_center_achievement_relationships_group_achievement_dict = game_center_achievement_relationships_group_achievement_instance.to_dict()
# create an instance of GameCenterAchievementRelationshipsGroupAchievement from a dict
game_center_achievement_relationships_group_achievement_from_dict = GameCenterAchievementRelationshipsGroupAchievement.from_dict(game_center_achievement_relationships_group_achievement_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


