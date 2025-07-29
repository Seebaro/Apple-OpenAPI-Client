# GameCenterLeaderboardRelease


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**id** | **str** |  | 
**attributes** | [**GameCenterAchievementReleaseAttributes**](GameCenterAchievementReleaseAttributes.md) |  | [optional] 
**relationships** | [**GameCenterLeaderboardReleaseRelationships**](GameCenterLeaderboardReleaseRelationships.md) |  | [optional] 
**links** | [**ResourceLinks**](ResourceLinks.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_leaderboard_release import GameCenterLeaderboardRelease

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterLeaderboardRelease from a JSON string
game_center_leaderboard_release_instance = GameCenterLeaderboardRelease.from_json(json)
# print the JSON string representation of the object
print(GameCenterLeaderboardRelease.to_json())

# convert the object into a dict
game_center_leaderboard_release_dict = game_center_leaderboard_release_instance.to_dict()
# create an instance of GameCenterLeaderboardRelease from a dict
game_center_leaderboard_release_from_dict = GameCenterLeaderboardRelease.from_dict(game_center_leaderboard_release_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


