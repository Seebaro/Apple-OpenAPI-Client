# GameCenterMatchmakingRuleSetTestCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**GameCenterMatchmakingRuleSetTestCreateRequestData**](GameCenterMatchmakingRuleSetTestCreateRequestData.md) |  | 
**included** | [**List[GameCenterMatchmakingRuleSetTestCreateRequestIncludedInner]**](GameCenterMatchmakingRuleSetTestCreateRequestIncludedInner.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_matchmaking_rule_set_test_create_request import GameCenterMatchmakingRuleSetTestCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterMatchmakingRuleSetTestCreateRequest from a JSON string
game_center_matchmaking_rule_set_test_create_request_instance = GameCenterMatchmakingRuleSetTestCreateRequest.from_json(json)
# print the JSON string representation of the object
print(GameCenterMatchmakingRuleSetTestCreateRequest.to_json())

# convert the object into a dict
game_center_matchmaking_rule_set_test_create_request_dict = game_center_matchmaking_rule_set_test_create_request_instance.to_dict()
# create an instance of GameCenterMatchmakingRuleSetTestCreateRequest from a dict
game_center_matchmaking_rule_set_test_create_request_from_dict = GameCenterMatchmakingRuleSetTestCreateRequest.from_dict(game_center_matchmaking_rule_set_test_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


