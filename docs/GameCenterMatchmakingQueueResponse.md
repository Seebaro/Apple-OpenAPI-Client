# GameCenterMatchmakingQueueResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**GameCenterMatchmakingQueue**](GameCenterMatchmakingQueue.md) |  | 
**included** | [**List[GameCenterMatchmakingRuleSet]**](GameCenterMatchmakingRuleSet.md) |  | [optional] 
**links** | [**DocumentLinks**](DocumentLinks.md) |  | 

## Example

```python
from openapi_client.models.game_center_matchmaking_queue_response import GameCenterMatchmakingQueueResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterMatchmakingQueueResponse from a JSON string
game_center_matchmaking_queue_response_instance = GameCenterMatchmakingQueueResponse.from_json(json)
# print the JSON string representation of the object
print(GameCenterMatchmakingQueueResponse.to_json())

# convert the object into a dict
game_center_matchmaking_queue_response_dict = game_center_matchmaking_queue_response_instance.to_dict()
# create an instance of GameCenterMatchmakingQueueResponse from a dict
game_center_matchmaking_queue_response_from_dict = GameCenterMatchmakingQueueResponse.from_dict(game_center_matchmaking_queue_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


