# GameCenterLeaderboardLocalizationAttributes


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**locale** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**formatter_override** | [**GameCenterLeaderboardFormatter**](GameCenterLeaderboardFormatter.md) |  | [optional] 
**formatter_suffix** | **str** |  | [optional] 
**formatter_suffix_singular** | **str** |  | [optional] 

## Example

```python
from openapi_client.models.game_center_leaderboard_localization_attributes import GameCenterLeaderboardLocalizationAttributes

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterLeaderboardLocalizationAttributes from a JSON string
game_center_leaderboard_localization_attributes_instance = GameCenterLeaderboardLocalizationAttributes.from_json(json)
# print the JSON string representation of the object
print(GameCenterLeaderboardLocalizationAttributes.to_json())

# convert the object into a dict
game_center_leaderboard_localization_attributes_dict = game_center_leaderboard_localization_attributes_instance.to_dict()
# create an instance of GameCenterLeaderboardLocalizationAttributes from a dict
game_center_leaderboard_localization_attributes_from_dict = GameCenterLeaderboardLocalizationAttributes.from_dict(game_center_leaderboard_localization_attributes_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


