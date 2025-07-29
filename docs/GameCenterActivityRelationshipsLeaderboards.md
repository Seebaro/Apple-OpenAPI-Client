# GameCenterActivityRelationshipsLeaderboards


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[GameCenterActivityRelationshipsLeaderboardsDataInner]**](GameCenterActivityRelationshipsLeaderboardsDataInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_activity_relationships_leaderboards import GameCenterActivityRelationshipsLeaderboards

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterActivityRelationshipsLeaderboards from a JSON string
game_center_activity_relationships_leaderboards_instance = GameCenterActivityRelationshipsLeaderboards.from_json(json)
# print the JSON string representation of the object
print(GameCenterActivityRelationshipsLeaderboards.to_json())

# convert the object into a dict
game_center_activity_relationships_leaderboards_dict = game_center_activity_relationships_leaderboards_instance.to_dict()
# create an instance of GameCenterActivityRelationshipsLeaderboards from a dict
game_center_activity_relationships_leaderboards_from_dict = GameCenterActivityRelationshipsLeaderboards.from_dict(game_center_activity_relationships_leaderboards_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


