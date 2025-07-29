# GameCenterDetailRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**app** | [**AlternativeDistributionKeyCreateRequestDataRelationshipsApp**](AlternativeDistributionKeyCreateRequestDataRelationshipsApp.md) |  | [optional] 
**game_center_app_versions** | [**GameCenterAppVersionRelationshipsCompatibilityVersions**](GameCenterAppVersionRelationshipsCompatibilityVersions.md) |  | [optional] 
**game_center_group** | [**GameCenterDetailRelationshipsGameCenterGroup**](GameCenterDetailRelationshipsGameCenterGroup.md) |  | [optional] 
**game_center_leaderboards** | [**GameCenterActivityRelationshipsLeaderboards**](GameCenterActivityRelationshipsLeaderboards.md) |  | [optional] 
**game_center_leaderboard_sets** | [**GameCenterDetailRelationshipsGameCenterLeaderboardSets**](GameCenterDetailRelationshipsGameCenterLeaderboardSets.md) |  | [optional] 
**game_center_achievements** | [**GameCenterActivityRelationshipsAchievements**](GameCenterActivityRelationshipsAchievements.md) |  | [optional] 
**game_center_activities** | [**GameCenterDetailRelationshipsGameCenterActivities**](GameCenterDetailRelationshipsGameCenterActivities.md) |  | [optional] 
**game_center_challenges** | [**GameCenterDetailRelationshipsGameCenterChallenges**](GameCenterDetailRelationshipsGameCenterChallenges.md) |  | [optional] 
**default_leaderboard** | [**GameCenterChallengeCreateRequestDataRelationshipsLeaderboard**](GameCenterChallengeCreateRequestDataRelationshipsLeaderboard.md) |  | [optional] 
**default_group_leaderboard** | [**GameCenterChallengeCreateRequestDataRelationshipsLeaderboard**](GameCenterChallengeCreateRequestDataRelationshipsLeaderboard.md) |  | [optional] 
**achievement_releases** | [**GameCenterAchievementRelationshipsReleases**](GameCenterAchievementRelationshipsReleases.md) |  | [optional] 
**activity_releases** | [**GameCenterDetailRelationshipsActivityReleases**](GameCenterDetailRelationshipsActivityReleases.md) |  | [optional] 
**challenge_releases** | [**GameCenterDetailRelationshipsChallengeReleases**](GameCenterDetailRelationshipsChallengeReleases.md) |  | [optional] 
**leaderboard_releases** | [**GameCenterDetailRelationshipsLeaderboardReleases**](GameCenterDetailRelationshipsLeaderboardReleases.md) |  | [optional] 
**leaderboard_set_releases** | [**GameCenterDetailRelationshipsLeaderboardSetReleases**](GameCenterDetailRelationshipsLeaderboardSetReleases.md) |  | [optional] 
**challenges_minimum_platform_versions** | [**AppRelationshipsAppStoreVersions**](AppRelationshipsAppStoreVersions.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_detail_relationships import GameCenterDetailRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterDetailRelationships from a JSON string
game_center_detail_relationships_instance = GameCenterDetailRelationships.from_json(json)
# print the JSON string representation of the object
print(GameCenterDetailRelationships.to_json())

# convert the object into a dict
game_center_detail_relationships_dict = game_center_detail_relationships_instance.to_dict()
# create an instance of GameCenterDetailRelationships from a dict
game_center_detail_relationships_from_dict = GameCenterDetailRelationships.from_dict(game_center_detail_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


