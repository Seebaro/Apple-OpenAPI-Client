# GameCenterAchievementRelationshipsReleases


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[GameCenterAchievementRelationshipsReleasesDataInner]**](GameCenterAchievementRelationshipsReleasesDataInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_achievement_relationships_releases import GameCenterAchievementRelationshipsReleases

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterAchievementRelationshipsReleases from a JSON string
game_center_achievement_relationships_releases_instance = GameCenterAchievementRelationshipsReleases.from_json(json)
# print the JSON string representation of the object
print(GameCenterAchievementRelationshipsReleases.to_json())

# convert the object into a dict
game_center_achievement_relationships_releases_dict = game_center_achievement_relationships_releases_instance.to_dict()
# create an instance of GameCenterAchievementRelationshipsReleases from a dict
game_center_achievement_relationships_releases_from_dict = GameCenterAchievementRelationshipsReleases.from_dict(game_center_achievement_relationships_releases_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


