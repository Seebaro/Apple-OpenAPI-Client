# GameCenterMatchmakingRuleAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**reference_name** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**type** | **str** |  | [optional] 
**expression** | **str** |  | [optional] 
**weight** | **float** |  | [optional] 

## Example

```python
from openapi_client.models.game_center_matchmaking_rule_attributes import GameCenterMatchmakingRuleAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterMatchmakingRuleAttributes from a JSON string
game_center_matchmaking_rule_attributes_instance = GameCenterMatchmakingRuleAttributes.from_json(json)
# print the JSON string representation of the object
print(GameCenterMatchmakingRuleAttributes.to_json())

# convert the object into a dict
game_center_matchmaking_rule_attributes_dict = game_center_matchmaking_rule_attributes_instance.to_dict()
# create an instance of GameCenterMatchmakingRuleAttributes from a dict
game_center_matchmaking_rule_attributes_from_dict = GameCenterMatchmakingRuleAttributes.from_dict(game_center_matchmaking_rule_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


