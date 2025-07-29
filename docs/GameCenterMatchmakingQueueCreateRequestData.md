# GameCenterMatchmakingQueueCreateRequestData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**attributes** | [**GameCenterMatchmakingQueueCreateRequestDataAttributes**](GameCenterMatchmakingQueueCreateRequestDataAttributes.md) |  | 
**relationships** | [**GameCenterMatchmakingQueueCreateRequestDataRelationships**](GameCenterMatchmakingQueueCreateRequestDataRelationships.md) |  | 

## Example

```python
from openapi_client.models.game_center_matchmaking_queue_create_request_data import GameCenterMatchmakingQueueCreateRequestData

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterMatchmakingQueueCreateRequestData from a JSON string
game_center_matchmaking_queue_create_request_data_instance = GameCenterMatchmakingQueueCreateRequestData.from_json(json)
# print the JSON string representation of the object
print(GameCenterMatchmakingQueueCreateRequestData.to_json())

# convert the object into a dict
game_center_matchmaking_queue_create_request_data_dict = game_center_matchmaking_queue_create_request_data_instance.to_dict()
# create an instance of GameCenterMatchmakingQueueCreateRequestData from a dict
game_center_matchmaking_queue_create_request_data_from_dict = GameCenterMatchmakingQueueCreateRequestData.from_dict(game_center_matchmaking_queue_create_request_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


