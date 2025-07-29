# GameCenterMatchmakingRuleSetRelationshipsTeams


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[GameCenterMatchmakingRuleSetRelationshipsTeamsDataInner]**](GameCenterMatchmakingRuleSetRelationshipsTeamsDataInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_matchmaking_rule_set_relationships_teams import GameCenterMatchmakingRuleSetRelationshipsTeams

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterMatchmakingRuleSetRelationshipsTeams from a JSON string
game_center_matchmaking_rule_set_relationships_teams_instance = GameCenterMatchmakingRuleSetRelationshipsTeams.from_json(json)
# print the JSON string representation of the object
print(GameCenterMatchmakingRuleSetRelationshipsTeams.to_json())

# convert the object into a dict
game_center_matchmaking_rule_set_relationships_teams_dict = game_center_matchmaking_rule_set_relationships_teams_instance.to_dict()
# create an instance of GameCenterMatchmakingRuleSetRelationshipsTeams from a dict
game_center_matchmaking_rule_set_relationships_teams_from_dict = GameCenterMatchmakingRuleSetRelationshipsTeams.from_dict(game_center_matchmaking_rule_set_relationships_teams_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


