# GameCenterLeaderboardSetRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**game_center_detail** | [**GameCenterAchievementReleaseRelationshipsGameCenterDetail**](GameCenterAchievementReleaseRelationshipsGameCenterDetail.md) |  | [optional] 
**game_center_group** | [**GameCenterAchievementRelationshipsGameCenterGroup**](GameCenterAchievementRelationshipsGameCenterGroup.md) |  | [optional] 
**group_leaderboard_set** | [**GameCenterLeaderboardSetRelationshipsGroupLeaderboardSet**](GameCenterLeaderboardSetRelationshipsGroupLeaderboardSet.md) |  | [optional] 
**localizations** | [**GameCenterLeaderboardSetRelationshipsLocalizations**](GameCenterLeaderboardSetRelationshipsLocalizations.md) |  | [optional] 
**game_center_leaderboards** | [**GameCenterActivityRelationshipsLeaderboards**](GameCenterActivityRelationshipsLeaderboards.md) |  | [optional] 
**releases** | [**GameCenterDetailRelationshipsLeaderboardSetReleases**](GameCenterDetailRelationshipsLeaderboardSetReleases.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_leaderboard_set_relationships import GameCenterLeaderboardSetRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterLeaderboardSetRelationships from a JSON string
game_center_leaderboard_set_relationships_instance = GameCenterLeaderboardSetRelationships.from_json(json)
# print the JSON string representation of the object
print(GameCenterLeaderboardSetRelationships.to_json())

# convert the object into a dict
game_center_leaderboard_set_relationships_dict = game_center_leaderboard_set_relationships_instance.to_dict()
# create an instance of GameCenterLeaderboardSetRelationships from a dict
game_center_leaderboard_set_relationships_from_dict = GameCenterLeaderboardSetRelationships.from_dict(game_center_leaderboard_set_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


