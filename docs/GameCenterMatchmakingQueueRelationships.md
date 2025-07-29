# GameCenterMatchmakingQueueRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**rule_set** | [**GameCenterMatchmakingQueueRelationshipsRuleSet**](GameCenterMatchmakingQueueRelationshipsRuleSet.md) |  | [optional] 
**experiment_rule_set** | [**GameCenterMatchmakingQueueRelationshipsRuleSet**](GameCenterMatchmakingQueueRelationshipsRuleSet.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_matchmaking_queue_relationships import GameCenterMatchmakingQueueRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterMatchmakingQueueRelationships from a JSON string
game_center_matchmaking_queue_relationships_instance = GameCenterMatchmakingQueueRelationships.from_json(json)
# print the JSON string representation of the object
print(GameCenterMatchmakingQueueRelationships.to_json())

# convert the object into a dict
game_center_matchmaking_queue_relationships_dict = game_center_matchmaking_queue_relationships_instance.to_dict()
# create an instance of GameCenterMatchmakingQueueRelationships from a dict
game_center_matchmaking_queue_relationships_from_dict = GameCenterMatchmakingQueueRelationships.from_dict(game_center_matchmaking_queue_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


