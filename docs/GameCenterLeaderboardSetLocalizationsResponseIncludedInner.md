# GameCenterLeaderboardSetLocalizationsResponseIncludedInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**GameCenterAchievementImageAttributes**](GameCenterAchievementImageAttributes.md) |  | [optional] 
**relationships** | [**GameCenterLeaderboardSetImageRelationships**](GameCenterLeaderboardSetImageRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_leaderboard_set_localizations_response_included_inner import GameCenterLeaderboardSetLocalizationsResponseIncludedInner

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterLeaderboardSetLocalizationsResponseIncludedInner from a JSON string
game_center_leaderboard_set_localizations_response_included_inner_instance = GameCenterLeaderboardSetLocalizationsResponseIncludedInner.from_json(json)
# print the JSON string representation of the object
print(GameCenterLeaderboardSetLocalizationsResponseIncludedInner.to_json())

# convert the object into a dict
game_center_leaderboard_set_localizations_response_included_inner_dict = game_center_leaderboard_set_localizations_response_included_inner_instance.to_dict()
# create an instance of GameCenterLeaderboardSetLocalizationsResponseIncludedInner from a dict
game_center_leaderboard_set_localizations_response_included_inner_from_dict = GameCenterLeaderboardSetLocalizationsResponseIncludedInner.from_dict(game_center_leaderboard_set_localizations_response_included_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


