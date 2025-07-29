# GameCenterMatchmakingRuleSetUpdateRequestDataAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**min_players** | **int** |  | [optional] 
**max_players** | **int** |  | [optional] 

## Example

```python
from openapi_client.models.game_center_matchmaking_rule_set_update_request_data_attributes import GameCenterMatchmakingRuleSetUpdateRequestDataAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterMatchmakingRuleSetUpdateRequestDataAttributes from a JSON string
game_center_matchmaking_rule_set_update_request_data_attributes_instance = GameCenterMatchmakingRuleSetUpdateRequestDataAttributes.from_json(json)
# print the JSON string representation of the object
print(GameCenterMatchmakingRuleSetUpdateRequestDataAttributes.to_json())

# convert the object into a dict
game_center_matchmaking_rule_set_update_request_data_attributes_dict = game_center_matchmaking_rule_set_update_request_data_attributes_instance.to_dict()
# create an instance of GameCenterMatchmakingRuleSetUpdateRequestDataAttributes from a dict
game_center_matchmaking_rule_set_update_request_data_attributes_from_dict = GameCenterMatchmakingRuleSetUpdateRequestDataAttributes.from_dict(game_center_matchmaking_rule_set_update_request_data_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


