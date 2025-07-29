# GameCenterLeaderboardSetAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**reference_name** | **str** |  | [optional] 
**vendor_identifier** | **str** |  | [optional] 

## Example

```python
from openapi_client.models.game_center_leaderboard_set_attributes import GameCenterLeaderboardSetAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterLeaderboardSetAttributes from a JSON string
game_center_leaderboard_set_attributes_instance = GameCenterLeaderboardSetAttributes.from_json(json)
# print the JSON string representation of the object
print(GameCenterLeaderboardSetAttributes.to_json())

# convert the object into a dict
game_center_leaderboard_set_attributes_dict = game_center_leaderboard_set_attributes_instance.to_dict()
# create an instance of GameCenterLeaderboardSetAttributes from a dict
game_center_leaderboard_set_attributes_from_dict = GameCenterLeaderboardSetAttributes.from_dict(game_center_leaderboard_set_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


