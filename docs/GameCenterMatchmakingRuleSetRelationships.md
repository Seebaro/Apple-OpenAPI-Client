# GameCenterMatchmakingRuleSetRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**teams** | [**GameCenterMatchmakingRuleSetRelationshipsTeams**](GameCenterMatchmakingRuleSetRelationshipsTeams.md) |  | [optional] 
**rules** | [**GameCenterMatchmakingRuleSetRelationshipsRules**](GameCenterMatchmakingRuleSetRelationshipsRules.md) |  | [optional] 
**matchmaking_queues** | [**GameCenterMatchmakingRuleSetRelationshipsMatchmakingQueues**](GameCenterMatchmakingRuleSetRelationshipsMatchmakingQueues.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_matchmaking_rule_set_relationships import GameCenterMatchmakingRuleSetRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterMatchmakingRuleSetRelationships from a JSON string
game_center_matchmaking_rule_set_relationships_instance = GameCenterMatchmakingRuleSetRelationships.from_json(json)
# print the JSON string representation of the object
print(GameCenterMatchmakingRuleSetRelationships.to_json())

# convert the object into a dict
game_center_matchmaking_rule_set_relationships_dict = game_center_matchmaking_rule_set_relationships_instance.to_dict()
# create an instance of GameCenterMatchmakingRuleSetRelationships from a dict
game_center_matchmaking_rule_set_relationships_from_dict = GameCenterMatchmakingRuleSetRelationships.from_dict(game_center_matchmaking_rule_set_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


