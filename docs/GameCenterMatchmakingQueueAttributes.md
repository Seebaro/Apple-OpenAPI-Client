# GameCenterMatchmakingQueueAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**reference_name** | **str** |  | [optional] 
**classic_matchmaking_bundle_ids** | **List[str]** |  | [optional] 

## Example

```python
from openapi_client.models.game_center_matchmaking_queue_attributes import GameCenterMatchmakingQueueAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterMatchmakingQueueAttributes from a JSON string
game_center_matchmaking_queue_attributes_instance = GameCenterMatchmakingQueueAttributes.from_json(json)
# print the JSON string representation of the object
print(GameCenterMatchmakingQueueAttributes.to_json())

# convert the object into a dict
game_center_matchmaking_queue_attributes_dict = game_center_matchmaking_queue_attributes_instance.to_dict()
# create an instance of GameCenterMatchmakingQueueAttributes from a dict
game_center_matchmaking_queue_attributes_from_dict = GameCenterMatchmakingQueueAttributes.from_dict(game_center_matchmaking_queue_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


