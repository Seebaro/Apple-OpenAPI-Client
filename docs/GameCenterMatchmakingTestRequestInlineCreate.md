# GameCenterMatchmakingTestRequestInlineCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | [optional] 
**attributes** | [**GameCenterMatchmakingTestRequestInlineCreateAttributes**](GameCenterMatchmakingTestRequestInlineCreateAttributes.md) |  | 
**relationships** | [**GameCenterMatchmakingTestRequestInlineCreateRelationships**](GameCenterMatchmakingTestRequestInlineCreateRelationships.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_matchmaking_test_request_inline_create import GameCenterMatchmakingTestRequestInlineCreate

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterMatchmakingTestRequestInlineCreate from a JSON string
game_center_matchmaking_test_request_inline_create_instance = GameCenterMatchmakingTestRequestInlineCreate.from_json(json)
# print the JSON string representation of the object
print(GameCenterMatchmakingTestRequestInlineCreate.to_json())

# convert the object into a dict
game_center_matchmaking_test_request_inline_create_dict = game_center_matchmaking_test_request_inline_create_instance.to_dict()
# create an instance of GameCenterMatchmakingTestRequestInlineCreate from a dict
game_center_matchmaking_test_request_inline_create_from_dict = GameCenterMatchmakingTestRequestInlineCreate.from_dict(game_center_matchmaking_test_request_inline_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


