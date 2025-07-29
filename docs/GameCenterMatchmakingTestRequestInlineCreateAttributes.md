# GameCenterMatchmakingTestRequestInlineCreateAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**request_name** | **str** |  | 
**seconds_in_queue** | **int** |  | 
**locale** | **str** |  | [optional] 
**location** | [**Location**](Location.md) |  | [optional] 
**min_players** | **int** |  | [optional] 
**max_players** | **int** |  | [optional] 
**player_count** | **int** |  | [optional] 
**bundle_id** | **str** |  | 
**platform** | [**Platform**](Platform.md) |  | 
**app_version** | **str** |  | 

## Example

```python
from openapi_client.models.game_center_matchmaking_test_request_inline_create_attributes import GameCenterMatchmakingTestRequestInlineCreateAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterMatchmakingTestRequestInlineCreateAttributes from a JSON string
game_center_matchmaking_test_request_inline_create_attributes_instance = GameCenterMatchmakingTestRequestInlineCreateAttributes.from_json(json)
# print the JSON string representation of the object
print(GameCenterMatchmakingTestRequestInlineCreateAttributes.to_json())

# convert the object into a dict
game_center_matchmaking_test_request_inline_create_attributes_dict = game_center_matchmaking_test_request_inline_create_attributes_instance.to_dict()
# create an instance of GameCenterMatchmakingTestRequestInlineCreateAttributes from a dict
game_center_matchmaking_test_request_inline_create_attributes_from_dict = GameCenterMatchmakingTestRequestInlineCreateAttributes.from_dict(game_center_matchmaking_test_request_inline_create_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


