# GameCenterMatchmakingQueueCreateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**GameCenterMatchmakingQueueCreateRequestData**](GameCenterMatchmakingQueueCreateRequestData.md) |  | 

## Example

```python
from openapi_client.models.game_center_matchmaking_queue_create_request import GameCenterMatchmakingQueueCreateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterMatchmakingQueueCreateRequest from a JSON string
game_center_matchmaking_queue_create_request_instance = GameCenterMatchmakingQueueCreateRequest.from_json(json)
# print the JSON string representation of the object
print(GameCenterMatchmakingQueueCreateRequest.to_json())

# convert the object into a dict
game_center_matchmaking_queue_create_request_dict = game_center_matchmaking_queue_create_request_instance.to_dict()
# create an instance of GameCenterMatchmakingQueueCreateRequest from a dict
game_center_matchmaking_queue_create_request_from_dict = GameCenterMatchmakingQueueCreateRequest.from_dict(game_center_matchmaking_queue_create_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


