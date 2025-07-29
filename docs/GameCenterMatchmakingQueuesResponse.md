# GameCenterMatchmakingQueuesResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[GameCenterMatchmakingQueue]**](GameCenterMatchmakingQueue.md) |  | 
**included** | [**List[GameCenterMatchmakingRuleSet]**](GameCenterMatchmakingRuleSet.md) |  | [optional] 
**links** | [**PagedDocumentLinks**](PagedDocumentLinks.md) |  | 
**meta** | [**PagingInformation**](PagingInformation.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_matchmaking_queues_response import GameCenterMatchmakingQueuesResponse

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterMatchmakingQueuesResponse from a JSON string
game_center_matchmaking_queues_response_instance = GameCenterMatchmakingQueuesResponse.from_json(json)
# print the JSON string representation of the object
print(GameCenterMatchmakingQueuesResponse.to_json())

# convert the object into a dict
game_center_matchmaking_queues_response_dict = game_center_matchmaking_queues_response_instance.to_dict()
# create an instance of GameCenterMatchmakingQueuesResponse from a dict
game_center_matchmaking_queues_response_from_dict = GameCenterMatchmakingQueuesResponse.from_dict(game_center_matchmaking_queues_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


