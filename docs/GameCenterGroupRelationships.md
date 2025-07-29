# GameCenterGroupRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**game_center_details** | [**GameCenterGroupRelationshipsGameCenterDetails**](GameCenterGroupRelationshipsGameCenterDetails.md) |  | [optional] 
**game_center_leaderboards** | [**GameCenterActivityRelationshipsLeaderboards**](GameCenterActivityRelationshipsLeaderboards.md) |  | [optional] 
**game_center_leaderboard_sets** | [**GameCenterDetailRelationshipsGameCenterLeaderboardSets**](GameCenterDetailRelationshipsGameCenterLeaderboardSets.md) |  | [optional] 
**game_center_achievements** | [**GameCenterActivityRelationshipsAchievements**](GameCenterActivityRelationshipsAchievements.md) |  | [optional] 
**game_center_activities** | [**GameCenterDetailRelationshipsGameCenterActivities**](GameCenterDetailRelationshipsGameCenterActivities.md) |  | [optional] 
**game_center_challenges** | [**GameCenterDetailRelationshipsGameCenterChallenges**](GameCenterDetailRelationshipsGameCenterChallenges.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_group_relationships import GameCenterGroupRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterGroupRelationships from a JSON string
game_center_group_relationships_instance = GameCenterGroupRelationships.from_json(json)
# print the JSON string representation of the object
print(GameCenterGroupRelationships.to_json())

# convert the object into a dict
game_center_group_relationships_dict = game_center_group_relationships_instance.to_dict()
# create an instance of GameCenterGroupRelationships from a dict
game_center_group_relationships_from_dict = GameCenterGroupRelationships.from_dict(game_center_group_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


