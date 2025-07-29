# GameCenterMatchmakingRuleSetCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**GameCenterMatchmakingRuleSetCreateRequestDataAttributes**](GameCenterMatchmakingRuleSetCreateRequestDataAttributes.md) |  | 

## Example

```python
from openapi_client.models.game_center_matchmaking_rule_set_create_request_data import GameCenterMatchmakingRuleSetCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterMatchmakingRuleSetCreateRequestData from a JSON string
game_center_matchmaking_rule_set_create_request_data_instance = GameCenterMatchmakingRuleSetCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(GameCenterMatchmakingRuleSetCreateRequestData.to_json())

# convert the object into a dict
game_center_matchmaking_rule_set_create_request_data_dict = game_center_matchmaking_rule_set_create_request_data_instance.to_dict()
# create an instance of GameCenterMatchmakingRuleSetCreateRequestData from a dict
game_center_matchmaking_rule_set_create_request_data_from_dict = GameCenterMatchmakingRuleSetCreateRequestData.from_dict(game_center_matchmaking_rule_set_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


