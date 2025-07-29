# GameCenterMatchmakingRuleSetCreateRequestDataAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**reference_name** | **str** |  | 
**rule_language_version** | **int** |  | 
**min_players** | **int** |  | 
**max_players** | **int** |  | 

## Example

```python
from openapi_client.models.game_center_matchmaking_rule_set_create_request_data_attributes import GameCenterMatchmakingRuleSetCreateRequestDataAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterMatchmakingRuleSetCreateRequestDataAttributes from a JSON string
game_center_matchmaking_rule_set_create_request_data_attributes_instance = GameCenterMatchmakingRuleSetCreateRequestDataAttributes.from_json(json)
# print the JSON string representation of the object
print(GameCenterMatchmakingRuleSetCreateRequestDataAttributes.to_json())

# convert the object into a dict
game_center_matchmaking_rule_set_create_request_data_attributes_dict = game_center_matchmaking_rule_set_create_request_data_attributes_instance.to_dict()
# create an instance of GameCenterMatchmakingRuleSetCreateRequestDataAttributes from a dict
game_center_matchmaking_rule_set_create_request_data_attributes_from_dict = GameCenterMatchmakingRuleSetCreateRequestDataAttributes.from_dict(game_center_matchmaking_rule_set_create_request_data_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


