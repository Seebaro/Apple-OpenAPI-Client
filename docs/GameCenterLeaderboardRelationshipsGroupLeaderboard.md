# GameCenterLeaderboardRelationshipsGroupLeaderboard


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**data** | [**GameCenterActivityRelationshipsLeaderboardsDataInner**](GameCenterActivityRelationshipsLeaderboardsDataInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_leaderboard_relationships_group_leaderboard import GameCenterLeaderboardRelationshipsGroupLeaderboard

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterLeaderboardRelationshipsGroupLeaderboard from a JSON string
game_center_leaderboard_relationships_group_leaderboard_instance = GameCenterLeaderboardRelationshipsGroupLeaderboard.from_json(json)
# print the JSON string representation of the object
print(GameCenterLeaderboardRelationshipsGroupLeaderboard.to_json())

# convert the object into a dict
game_center_leaderboard_relationships_group_leaderboard_dict = game_center_leaderboard_relationships_group_leaderboard_instance.to_dict()
# create an instance of GameCenterLeaderboardRelationshipsGroupLeaderboard from a dict
game_center_leaderboard_relationships_group_leaderboard_from_dict = GameCenterLeaderboardRelationshipsGroupLeaderboard.from_dict(game_center_leaderboard_relationships_group_leaderboard_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


