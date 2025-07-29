# GameCenterDetailRelationshipsGameCenterLeaderboardSets


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[GameCenterDetailRelationshipsGameCenterLeaderboardSetsDataInner]**](GameCenterDetailRelationshipsGameCenterLeaderboardSetsDataInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_detail_relationships_game_center_leaderboard_sets import GameCenterDetailRelationshipsGameCenterLeaderboardSets

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterDetailRelationshipsGameCenterLeaderboardSets from a JSON string
game_center_detail_relationships_game_center_leaderboard_sets_instance = GameCenterDetailRelationshipsGameCenterLeaderboardSets.from_json(json)
# print the JSON string representation of the object
print(GameCenterDetailRelationshipsGameCenterLeaderboardSets.to_json())

# convert the object into a dict
game_center_detail_relationships_game_center_leaderboard_sets_dict = game_center_detail_relationships_game_center_leaderboard_sets_instance.to_dict()
# create an instance of GameCenterDetailRelationshipsGameCenterLeaderboardSets from a dict
game_center_detail_relationships_game_center_leaderboard_sets_from_dict = GameCenterDetailRelationshipsGameCenterLeaderboardSets.from_dict(game_center_detail_relationships_game_center_leaderboard_sets_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


