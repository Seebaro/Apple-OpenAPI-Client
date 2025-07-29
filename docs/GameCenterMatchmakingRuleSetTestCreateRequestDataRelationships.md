# GameCenterMatchmakingRuleSetTestCreateRequestDataRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**matchmaking_rule_set** | [**GameCenterMatchmakingQueueCreateRequestDataRelationshipsRuleSet**](GameCenterMatchmakingQueueCreateRequestDataRelationshipsRuleSet.md) |  | 
**matchmaking_requests** | [**GameCenterMatchmakingRuleSetTestCreateRequestDataRelationshipsMatchmakingRequests**](GameCenterMatchmakingRuleSetTestCreateRequestDataRelationshipsMatchmakingRequests.md) |  | 

## Example

```python
from openapi_client.models.game_center_matchmaking_rule_set_test_create_request_data_relationships import GameCenterMatchmakingRuleSetTestCreateRequestDataRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterMatchmakingRuleSetTestCreateRequestDataRelationships from a JSON string
game_center_matchmaking_rule_set_test_create_request_data_relationships_instance = GameCenterMatchmakingRuleSetTestCreateRequestDataRelationships.from_json(json)
# print the JSON string representation of the object
print(GameCenterMatchmakingRuleSetTestCreateRequestDataRelationships.to_json())

# convert the object into a dict
game_center_matchmaking_rule_set_test_create_request_data_relationships_dict = game_center_matchmaking_rule_set_test_create_request_data_relationships_instance.to_dict()
# create an instance of GameCenterMatchmakingRuleSetTestCreateRequestDataRelationships from a dict
game_center_matchmaking_rule_set_test_create_request_data_relationships_from_dict = GameCenterMatchmakingRuleSetTestCreateRequestDataRelationships.from_dict(game_center_matchmaking_rule_set_test_create_request_data_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


