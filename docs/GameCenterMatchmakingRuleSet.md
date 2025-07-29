# GameCenterMatchmakingRuleSet


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**GameCenterMatchmakingRuleSetAttributes**](GameCenterMatchmakingRuleSetAttributes.md) |  | [optional] 
**relationships** | [**GameCenterMatchmakingRuleSetRelationships**](GameCenterMatchmakingRuleSetRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_matchmaking_rule_set import GameCenterMatchmakingRuleSet

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterMatchmakingRuleSet from a JSON string
game_center_matchmaking_rule_set_instance = GameCenterMatchmakingRuleSet.from_json(json)
# print the JSON string representation of the object
print(GameCenterMatchmakingRuleSet.to_json())

# convert the object into a dict
game_center_matchmaking_rule_set_dict = game_center_matchmaking_rule_set_instance.to_dict()
# create an instance of GameCenterMatchmakingRuleSet from a dict
game_center_matchmaking_rule_set_from_dict = GameCenterMatchmakingRuleSet.from_dict(game_center_matchmaking_rule_set_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


