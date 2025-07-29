# GameCenterMatchmakingRuleSetResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**GameCenterMatchmakingRuleSet**](GameCenterMatchmakingRuleSet.md) |  | 
**included** | [**List[GameCenterMatchmakingRuleSetsResponseIncludedInner]**](GameCenterMatchmakingRuleSetsResponseIncludedInner.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.game_center_matchmaking_rule_set_response import GameCenterMatchmakingRuleSetResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterMatchmakingRuleSetResponse from a JSON string
game_center_matchmaking_rule_set_response_instance = GameCenterMatchmakingRuleSetResponse.from_json(json)
# print the JSON string representation of the object
print(GameCenterMatchmakingRuleSetResponse.to_json())

# convert the object into a dict
game_center_matchmaking_rule_set_response_dict = game_center_matchmaking_rule_set_response_instance.to_dict()
# create an instance of GameCenterMatchmakingRuleSetResponse from a dict
game_center_matchmaking_rule_set_response_from_dict = GameCenterMatchmakingRuleSetResponse.from_dict(game_center_matchmaking_rule_set_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


