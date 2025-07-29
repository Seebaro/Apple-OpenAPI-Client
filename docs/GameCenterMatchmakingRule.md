# GameCenterMatchmakingRule


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**GameCenterMatchmakingRuleAttributes**](GameCenterMatchmakingRuleAttributes.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_matchmaking_rule import GameCenterMatchmakingRule

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterMatchmakingRule from a JSON string
game_center_matchmaking_rule_instance = GameCenterMatchmakingRule.from_json(json)
# print the JSON string representation of the object
print(GameCenterMatchmakingRule.to_json())

# convert the object into a dict
game_center_matchmaking_rule_dict = game_center_matchmaking_rule_instance.to_dict()
# create an instance of GameCenterMatchmakingRule from a dict
game_center_matchmaking_rule_from_dict = GameCenterMatchmakingRule.from_dict(game_center_matchmaking_rule_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


