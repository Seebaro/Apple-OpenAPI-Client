# GameCenterActivityRelationshipsAchievements


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[GameCenterAchievementLocalizationRelationshipsGameCenterAchievementData]**](GameCenterAchievementLocalizationRelationshipsGameCenterAchievementData.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_activity_relationships_achievements import GameCenterActivityRelationshipsAchievements

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterActivityRelationshipsAchievements from a JSON string
game_center_activity_relationships_achievements_instance = GameCenterActivityRelationshipsAchievements.from_json(json)
# print the JSON string representation of the object
print(GameCenterActivityRelationshipsAchievements.to_json())

# convert the object into a dict
game_center_activity_relationships_achievements_dict = game_center_activity_relationships_achievements_instance.to_dict()
# create an instance of GameCenterActivityRelationshipsAchievements from a dict
game_center_activity_relationships_achievements_from_dict = GameCenterActivityRelationshipsAchievements.from_dict(game_center_activity_relationships_achievements_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


