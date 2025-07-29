# GameCenterMatchmakingRuleUpdateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**GameCenterMatchmakingRuleUpdateRequestDataAttributes**](GameCenterMatchmakingRuleUpdateRequestDataAttributes.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_matchmaking_rule_update_request_data import GameCenterMatchmakingRuleUpdateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterMatchmakingRuleUpdateRequestData from a JSON string
game_center_matchmaking_rule_update_request_data_instance = GameCenterMatchmakingRuleUpdateRequestData.from_json(json)
# print the JSON string representation of the object
print(GameCenterMatchmakingRuleUpdateRequestData.to_json())

# convert the object into a dict
game_center_matchmaking_rule_update_request_data_dict = game_center_matchmaking_rule_update_request_data_instance.to_dict()
# create an instance of GameCenterMatchmakingRuleUpdateRequestData from a dict
game_center_matchmaking_rule_update_request_data_from_dict = GameCenterMatchmakingRuleUpdateRequestData.from_dict(game_center_matchmaking_rule_update_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


