# GameCenterMatchmakingRuleSetTestCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**relationships** | [**GameCenterMatchmakingRuleSetTestCreateRequestDataRelationships**](GameCenterMatchmakingRuleSetTestCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.game_center_matchmaking_rule_set_test_create_request_data import GameCenterMatchmakingRuleSetTestCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterMatchmakingRuleSetTestCreateRequestData from a JSON string
game_center_matchmaking_rule_set_test_create_request_data_instance = GameCenterMatchmakingRuleSetTestCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(GameCenterMatchmakingRuleSetTestCreateRequestData.to_json())

# convert the object into a dict
game_center_matchmaking_rule_set_test_create_request_data_dict = game_center_matchmaking_rule_set_test_create_request_data_instance.to_dict()
# create an instance of GameCenterMatchmakingRuleSetTestCreateRequestData from a dict
game_center_matchmaking_rule_set_test_create_request_data_from_dict = GameCenterMatchmakingRuleSetTestCreateRequestData.from_dict(game_center_matchmaking_rule_set_test_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


