# GameCenterMatchmakingRuleSetTestCreateRequestIncludedInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | [optional] 
**attributes** | [**GameCenterMatchmakingTestRequestInlineCreateAttributes**](GameCenterMatchmakingTestRequestInlineCreateAttributes.md) |  | 
**relationships** | [**GameCenterMatchmakingTestRequestInlineCreateRelationships**](GameCenterMatchmakingTestRequestInlineCreateRelationships.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_matchmaking_rule_set_test_create_request_included_inner import GameCenterMatchmakingRuleSetTestCreateRequestIncludedInner

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterMatchmakingRuleSetTestCreateRequestIncludedInner from a JSON string
game_center_matchmaking_rule_set_test_create_request_included_inner_instance = GameCenterMatchmakingRuleSetTestCreateRequestIncludedInner.from_json(json)
# print the JSON string representation of the object
print(GameCenterMatchmakingRuleSetTestCreateRequestIncludedInner.to_json())

# convert the object into a dict
game_center_matchmaking_rule_set_test_create_request_included_inner_dict = game_center_matchmaking_rule_set_test_create_request_included_inner_instance.to_dict()
# create an instance of GameCenterMatchmakingRuleSetTestCreateRequestIncludedInner from a dict
game_center_matchmaking_rule_set_test_create_request_included_inner_from_dict = GameCenterMatchmakingRuleSetTestCreateRequestIncludedInner.from_dict(game_center_matchmaking_rule_set_test_create_request_included_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


