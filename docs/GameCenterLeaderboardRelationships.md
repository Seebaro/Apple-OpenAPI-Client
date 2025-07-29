# GameCenterLeaderboardRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**game_center_detail** | [**GameCenterAchievementReleaseRelationshipsGameCenterDetail**](GameCenterAchievementReleaseRelationshipsGameCenterDetail.md) |  | [optional] 
**game_center_group** | [**GameCenterAchievementRelationshipsGameCenterGroup**](GameCenterAchievementRelationshipsGameCenterGroup.md) |  | [optional] 
**group_leaderboard** | [**GameCenterLeaderboardRelationshipsGroupLeaderboard**](GameCenterLeaderboardRelationshipsGroupLeaderboard.md) |  | [optional] 
**game_center_leaderboard_sets** | [**GameCenterLeaderboardRelationshipsGameCenterLeaderboardSets**](GameCenterLeaderboardRelationshipsGameCenterLeaderboardSets.md) |  | [optional] 
**localizations** | [**GameCenterLeaderboardRelationshipsLocalizations**](GameCenterLeaderboardRelationshipsLocalizations.md) |  | [optional] 
**releases** | [**GameCenterDetailRelationshipsLeaderboardReleases**](GameCenterDetailRelationshipsLeaderboardReleases.md) |  | [optional] 
**activity** | [**GameCenterAchievementRelationshipsActivity**](GameCenterAchievementRelationshipsActivity.md) |  | [optional] 
**challenge** | [**GameCenterLeaderboardRelationshipsChallenge**](GameCenterLeaderboardRelationshipsChallenge.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_leaderboard_relationships import GameCenterLeaderboardRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterLeaderboardRelationships from a JSON string
game_center_leaderboard_relationships_instance = GameCenterLeaderboardRelationships.from_json(json)
# print the JSON string representation of the object
print(GameCenterLeaderboardRelationships.to_json())

# convert the object into a dict
game_center_leaderboard_relationships_dict = game_center_leaderboard_relationships_instance.to_dict()
# create an instance of GameCenterLeaderboardRelationships from a dict
game_center_leaderboard_relationships_from_dict = GameCenterLeaderboardRelationships.from_dict(game_center_leaderboard_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


