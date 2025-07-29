# GameCenterMatchmakingQueueCreateRequestDataAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**reference_name** | **str** |  | 
**classic_matchmaking_bundle_ids** | **List[str]** |  | [optional] 

## Example

```python
from openapi_client.models.game_center_matchmaking_queue_create_request_data_attributes import GameCenterMatchmakingQueueCreateRequestDataAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterMatchmakingQueueCreateRequestDataAttributes from a JSON string
game_center_matchmaking_queue_create_request_data_attributes_instance = GameCenterMatchmakingQueueCreateRequestDataAttributes.from_json(json)
# print the JSON string representation of the object
print(GameCenterMatchmakingQueueCreateRequestDataAttributes.to_json())

# convert the object into a dict
game_center_matchmaking_queue_create_request_data_attributes_dict = game_center_matchmaking_queue_create_request_data_attributes_instance.to_dict()
# create an instance of GameCenterMatchmakingQueueCreateRequestDataAttributes from a dict
game_center_matchmaking_queue_create_request_data_attributes_from_dict = GameCenterMatchmakingQueueCreateRequestDataAttributes.from_dict(game_center_matchmaking_queue_create_request_data_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


