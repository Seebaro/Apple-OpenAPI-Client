# GameCenterLeaderboardReleaseRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**game_center_detail** | [**GameCenterAchievementReleaseRelationshipsGameCenterDetail**](GameCenterAchievementReleaseRelationshipsGameCenterDetail.md) |  | [optional] 
**game_center_leaderboard** | [**GameCenterChallengeCreateRequestDataRelationshipsLeaderboard**](GameCenterChallengeCreateRequestDataRelationshipsLeaderboard.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_leaderboard_release_relationships import GameCenterLeaderboardReleaseRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterLeaderboardReleaseRelationships from a JSON string
game_center_leaderboard_release_relationships_instance = GameCenterLeaderboardReleaseRelationships.from_json(json)
# print the JSON string representation of the object
print(GameCenterLeaderboardReleaseRelationships.to_json())

# convert the object into a dict
game_center_leaderboard_release_relationships_dict = game_center_leaderboard_release_relationships_instance.to_dict()
# create an instance of GameCenterLeaderboardReleaseRelationships from a dict
game_center_leaderboard_release_relationships_from_dict = GameCenterLeaderboardReleaseRelationships.from_dict(game_center_leaderboard_release_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


