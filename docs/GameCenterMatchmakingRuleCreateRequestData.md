# GameCenterMatchmakingRuleCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**GameCenterMatchmakingRuleCreateRequestDataAttributes**](GameCenterMatchmakingRuleCreateRequestDataAttributes.md) |  | 
**relationships** | [**GameCenterMatchmakingRuleCreateRequestDataRelationships**](GameCenterMatchmakingRuleCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.game_center_matchmaking_rule_create_request_data import GameCenterMatchmakingRuleCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterMatchmakingRuleCreateRequestData from a JSON string
game_center_matchmaking_rule_create_request_data_instance = GameCenterMatchmakingRuleCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(GameCenterMatchmakingRuleCreateRequestData.to_json())

# convert the object into a dict
game_center_matchmaking_rule_create_request_data_dict = game_center_matchmaking_rule_create_request_data_instance.to_dict()
# create an instance of GameCenterMatchmakingRuleCreateRequestData from a dict
game_center_matchmaking_rule_create_request_data_from_dict = GameCenterMatchmakingRuleCreateRequestData.from_dict(game_center_matchmaking_rule_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


