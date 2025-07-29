# GameCenterLeaderboardLocalization


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**GameCenterLeaderboardLocalizationAttributes**](GameCenterLeaderboardLocalizationAttributes.md) |  | [optional] 
**relationships** | [**GameCenterLeaderboardLocalizationRelationships**](GameCenterLeaderboardLocalizationRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_leaderboard_localization import GameCenterLeaderboardLocalization

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterLeaderboardLocalization from a JSON string
game_center_leaderboard_localization_instance = GameCenterLeaderboardLocalization.from_json(json)
# print the JSON string representation of the object
print(GameCenterLeaderboardLocalization.to_json())

# convert the object into a dict
game_center_leaderboard_localization_dict = game_center_leaderboard_localization_instance.to_dict()
# create an instance of GameCenterLeaderboardLocalization from a dict
game_center_leaderboard_localization_from_dict = GameCenterLeaderboardLocalization.from_dict(game_center_leaderboard_localization_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


