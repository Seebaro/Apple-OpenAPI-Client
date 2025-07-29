# GameCenterMatchmakingRuleSetRelationshipsRules


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 
**data** | [**List[GameCenterMatchmakingRuleSetRelationshipsRulesDataInner]**](GameCenterMatchmakingRuleSetRelationshipsRulesDataInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_matchmaking_rule_set_relationships_rules import GameCenterMatchmakingRuleSetRelationshipsRules

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterMatchmakingRuleSetRelationshipsRules from a JSON string
game_center_matchmaking_rule_set_relationships_rules_instance = GameCenterMatchmakingRuleSetRelationshipsRules.from_json(json)
# print the JSON string representation of the object
print(GameCenterMatchmakingRuleSetRelationshipsRules.to_json())

# convert the object into a dict
game_center_matchmaking_rule_set_relationships_rules_dict = game_center_matchmaking_rule_set_relationships_rules_instance.to_dict()
# create an instance of GameCenterMatchmakingRuleSetRelationshipsRules from a dict
game_center_matchmaking_rule_set_relationships_rules_from_dict = GameCenterMatchmakingRuleSetRelationshipsRules.from_dict(game_center_matchmaking_rule_set_relationships_rules_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


