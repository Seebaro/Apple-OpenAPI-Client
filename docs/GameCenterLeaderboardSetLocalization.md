# GameCenterLeaderboardSetLocalization


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**GameCenterLeaderboardSetLocalizationAttributes**](GameCenterLeaderboardSetLocalizationAttributes.md) |  | [optional] 
**relationships** | [**GameCenterLeaderboardSetLocalizationRelationships**](GameCenterLeaderboardSetLocalizationRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_leaderboard_set_localization import GameCenterLeaderboardSetLocalization

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterLeaderboardSetLocalization from a JSON string
game_center_leaderboard_set_localization_instance = GameCenterLeaderboardSetLocalization.from_json(json)
# print the JSON string representation of the object
print(GameCenterLeaderboardSetLocalization.to_json())

# convert the object into a dict
game_center_leaderboard_set_localization_dict = game_center_leaderboard_set_localization_instance.to_dict()
# create an instance of GameCenterLeaderboardSetLocalization from a dict
game_center_leaderboard_set_localization_from_dict = GameCenterLeaderboardSetLocalization.from_dict(game_center_leaderboard_set_localization_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


