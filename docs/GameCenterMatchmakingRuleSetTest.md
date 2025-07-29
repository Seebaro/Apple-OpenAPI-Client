# GameCenterMatchmakingRuleSetTest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**GameCenterMatchmakingRuleSetTestAttributes**](GameCenterMatchmakingRuleSetTestAttributes.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_matchmaking_rule_set_test import GameCenterMatchmakingRuleSetTest

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterMatchmakingRuleSetTest from a JSON string
game_center_matchmaking_rule_set_test_instance = GameCenterMatchmakingRuleSetTest.from_json(json)
# print the JSON string representation of the object
print(GameCenterMatchmakingRuleSetTest.to_json())

# convert the object into a dict
game_center_matchmaking_rule_set_test_dict = game_center_matchmaking_rule_set_test_instance.to_dict()
# create an instance of GameCenterMatchmakingRuleSetTest from a dict
game_center_matchmaking_rule_set_test_from_dict = GameCenterMatchmakingRuleSetTest.from_dict(game_center_matchmaking_rule_set_test_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


