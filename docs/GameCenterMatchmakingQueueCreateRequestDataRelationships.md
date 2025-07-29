# GameCenterMatchmakingQueueCreateRequestDataRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**rule_set** | [**GameCenterMatchmakingQueueCreateRequestDataRelationshipsRuleSet**](GameCenterMatchmakingQueueCreateRequestDataRelationshipsRuleSet.md) |  | 
**experiment_rule_set** | [**GameCenterMatchmakingQueueRelationshipsRuleSet**](GameCenterMatchmakingQueueRelationshipsRuleSet.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_matchmaking_queue_create_request_data_relationships import GameCenterMatchmakingQueueCreateRequestDataRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterMatchmakingQueueCreateRequestDataRelationships from a JSON string
game_center_matchmaking_queue_create_request_data_relationships_instance = GameCenterMatchmakingQueueCreateRequestDataRelationships.from_json(json)
# print the JSON string representation of the object
print(GameCenterMatchmakingQueueCreateRequestDataRelationships.to_json())

# convert the object into a dict
game_center_matchmaking_queue_create_request_data_relationships_dict = game_center_matchmaking_queue_create_request_data_relationships_instance.to_dict()
# create an instance of GameCenterMatchmakingQueueCreateRequestDataRelationships from a dict
game_center_matchmaking_queue_create_request_data_relationships_from_dict = GameCenterMatchmakingQueueCreateRequestDataRelationships.from_dict(game_center_matchmaking_queue_create_request_data_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


