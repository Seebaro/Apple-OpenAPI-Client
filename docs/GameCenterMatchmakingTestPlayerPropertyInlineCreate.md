# GameCenterMatchmakingTestPlayerPropertyInlineCreate


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | [optional] 
**attributes** | [**GameCenterMatchmakingTestPlayerPropertyInlineCreateAttributes**](GameCenterMatchmakingTestPlayerPropertyInlineCreateAttributes.md) |  | 

## Example

```python
from openapi_client.models.game_center_matchmaking_test_player_property_inline_create import GameCenterMatchmakingTestPlayerPropertyInlineCreate

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterMatchmakingTestPlayerPropertyInlineCreate from a JSON string
game_center_matchmaking_test_player_property_inline_create_instance = GameCenterMatchmakingTestPlayerPropertyInlineCreate.from_json(json)
# print the JSON string representation of the object
print(GameCenterMatchmakingTestPlayerPropertyInlineCreate.to_json())

# convert the object into a dict
game_center_matchmaking_test_player_property_inline_create_dict = game_center_matchmaking_test_player_property_inline_create_instance.to_dict()
# create an instance of GameCenterMatchmakingTestPlayerPropertyInlineCreate from a dict
game_center_matchmaking_test_player_property_inline_create_from_dict = GameCenterMatchmakingTestPlayerPropertyInlineCreate.from_dict(game_center_matchmaking_test_player_property_inline_create_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


