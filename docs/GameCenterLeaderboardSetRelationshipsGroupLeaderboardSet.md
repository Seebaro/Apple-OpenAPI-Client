# GameCenterLeaderboardSetRelationshipsGroupLeaderboardSet


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**data** | [**GameCenterDetailRelationshipsGameCenterLeaderboardSetsDataInner**](GameCenterDetailRelationshipsGameCenterLeaderboardSetsDataInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_leaderboard_set_relationships_group_leaderboard_set import GameCenterLeaderboardSetRelationshipsGroupLeaderboardSet

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterLeaderboardSetRelationshipsGroupLeaderboardSet from a JSON string
game_center_leaderboard_set_relationships_group_leaderboard_set_instance = GameCenterLeaderboardSetRelationshipsGroupLeaderboardSet.from_json(json)
# print the JSON string representation of the object
print(GameCenterLeaderboardSetRelationshipsGroupLeaderboardSet.to_json())

# convert the object into a dict
game_center_leaderboard_set_relationships_group_leaderboard_set_dict = game_center_leaderboard_set_relationships_group_leaderboard_set_instance.to_dict()
# create an instance of GameCenterLeaderboardSetRelationshipsGroupLeaderboardSet from a dict
game_center_leaderboard_set_relationships_group_leaderboard_set_from_dict = GameCenterLeaderboardSetRelationshipsGroupLeaderboardSet.from_dict(game_center_leaderboard_set_relationships_group_leaderboard_set_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


