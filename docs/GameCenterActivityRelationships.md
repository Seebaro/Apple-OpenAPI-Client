# GameCenterActivityRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**game_center_detail** | [**GameCenterAchievementReleaseRelationshipsGameCenterDetail**](GameCenterAchievementReleaseRelationshipsGameCenterDetail.md) |  | [optional] 
**game_center_group** | [**GameCenterAchievementRelationshipsGameCenterGroup**](GameCenterAchievementRelationshipsGameCenterGroup.md) |  | [optional] 
**achievements** | [**GameCenterActivityRelationshipsAchievements**](GameCenterActivityRelationshipsAchievements.md) |  | [optional] 
**leaderboards** | [**GameCenterActivityRelationshipsLeaderboards**](GameCenterActivityRelationshipsLeaderboards.md) |  | [optional] 
**versions** | [**GameCenterActivityRelationshipsVersions**](GameCenterActivityRelationshipsVersions.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_activity_relationships import GameCenterActivityRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterActivityRelationships from a JSON string
game_center_activity_relationships_instance = GameCenterActivityRelationships.from_json(json)
# print the JSON string representation of the object
print(GameCenterActivityRelationships.to_json())

# convert the object into a dict
game_center_activity_relationships_dict = game_center_activity_relationships_instance.to_dict()
# create an instance of GameCenterActivityRelationships from a dict
game_center_activity_relationships_from_dict = GameCenterActivityRelationships.from_dict(game_center_activity_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


