# GameCenterMatchmakingRuleCreateRequestDataAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**reference_name** | **str** |  | 
**description** | **str** |  | 
**type** | **str** |  | 
**expression** | **str** |  | 
**weight** | **float** |  | [optional] 

## Example

```python
from openapi_client.models.game_center_matchmaking_rule_create_request_data_attributes import GameCenterMatchmakingRuleCreateRequestDataAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterMatchmakingRuleCreateRequestDataAttributes from a JSON string
game_center_matchmaking_rule_create_request_data_attributes_instance = GameCenterMatchmakingRuleCreateRequestDataAttributes.from_json(json)
# print the JSON string representation of the object
print(GameCenterMatchmakingRuleCreateRequestDataAttributes.to_json())

# convert the object into a dict
game_center_matchmaking_rule_create_request_data_attributes_dict = game_center_matchmaking_rule_create_request_data_attributes_instance.to_dict()
# create an instance of GameCenterMatchmakingRuleCreateRequestDataAttributes from a dict
game_center_matchmaking_rule_create_request_data_attributes_from_dict = GameCenterMatchmakingRuleCreateRequestDataAttributes.from_dict(game_center_matchmaking_rule_create_request_data_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


