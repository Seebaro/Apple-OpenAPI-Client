# GameCenterMatchmakingRuleUpdateRequestDataAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**description** | **str** |  | [optional] 
**expression** | **str** |  | [optional] 
**weight** | **float** |  | [optional] 

## Example

```python
from openapi_client.models.game_center_matchmaking_rule_update_request_data_attributes import GameCenterMatchmakingRuleUpdateRequestDataAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterMatchmakingRuleUpdateRequestDataAttributes from a JSON string
game_center_matchmaking_rule_update_request_data_attributes_instance = GameCenterMatchmakingRuleUpdateRequestDataAttributes.from_json(json)
# print the JSON string representation of the object
print(GameCenterMatchmakingRuleUpdateRequestDataAttributes.to_json())

# convert the object into a dict
game_center_matchmaking_rule_update_request_data_attributes_dict = game_center_matchmaking_rule_update_request_data_attributes_instance.to_dict()
# create an instance of GameCenterMatchmakingRuleUpdateRequestDataAttributes from a dict
game_center_matchmaking_rule_update_request_data_attributes_from_dict = GameCenterMatchmakingRuleUpdateRequestDataAttributes.from_dict(game_center_matchmaking_rule_update_request_data_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


