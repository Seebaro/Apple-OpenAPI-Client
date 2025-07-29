# GameCenterMatchmakingQueue


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**GameCenterMatchmakingQueueAttributes**](GameCenterMatchmakingQueueAttributes.md) |  | [optional] 
**relationships** | [**GameCenterMatchmakingQueueRelationships**](GameCenterMatchmakingQueueRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_matchmaking_queue import GameCenterMatchmakingQueue

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterMatchmakingQueue from a JSON string
game_center_matchmaking_queue_instance = GameCenterMatchmakingQueue.from_json(json)
# print the JSON string representation of the object
print(GameCenterMatchmakingQueue.to_json())

# convert the object into a dict
game_center_matchmaking_queue_dict = game_center_matchmaking_queue_instance.to_dict()
# create an instance of GameCenterMatchmakingQueue from a dict
game_center_matchmaking_queue_from_dict = GameCenterMatchmakingQueue.from_dict(game_center_matchmaking_queue_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


