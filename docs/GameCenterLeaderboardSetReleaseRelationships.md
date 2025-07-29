# GameCenterLeaderboardSetReleaseRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**game_center_detail** | [**GameCenterAchievementReleaseRelationshipsGameCenterDetail**](GameCenterAchievementReleaseRelationshipsGameCenterDetail.md) |  | [optional] 
**game_center_leaderboard_set** | [**GameCenterLeaderboardSetLocalizationRelationshipsGameCenterLeaderboardSet**](GameCenterLeaderboardSetLocalizationRelationshipsGameCenterLeaderboardSet.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_leaderboard_set_release_relationships import GameCenterLeaderboardSetReleaseRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterLeaderboardSetReleaseRelationships from a JSON string
game_center_leaderboard_set_release_relationships_instance = GameCenterLeaderboardSetReleaseRelationships.from_json(json)
# print the JSON string representation of the object
print(GameCenterLeaderboardSetReleaseRelationships.to_json())

# convert the object into a dict
game_center_leaderboard_set_release_relationships_dict = game_center_leaderboard_set_release_relationships_instance.to_dict()
# create an instance of GameCenterLeaderboardSetReleaseRelationships from a dict
game_center_leaderboard_set_release_relationships_from_dict = GameCenterLeaderboardSetReleaseRelationships.from_dict(game_center_leaderboard_set_release_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


