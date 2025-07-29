# GameCenterChallengeRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**game_center_detail** | [**GameCenterAchievementReleaseRelationshipsGameCenterDetail**](GameCenterAchievementReleaseRelationshipsGameCenterDetail.md) |  | [optional] 
**game_center_group** | [**GameCenterAchievementRelationshipsGameCenterGroup**](GameCenterAchievementRelationshipsGameCenterGroup.md) |  | [optional] 
**versions** | [**GameCenterChallengeRelationshipsVersions**](GameCenterChallengeRelationshipsVersions.md) |  | [optional] 
**leaderboard** | [**GameCenterChallengeRelationshipsLeaderboard**](GameCenterChallengeRelationshipsLeaderboard.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_challenge_relationships import GameCenterChallengeRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterChallengeRelationships from a JSON string
game_center_challenge_relationships_instance = GameCenterChallengeRelationships.from_json(json)
# print the JSON string representation of the object
print(GameCenterChallengeRelationships.to_json())

# convert the object into a dict
game_center_challenge_relationships_dict = game_center_challenge_relationships_instance.to_dict()
# create an instance of GameCenterChallengeRelationships from a dict
game_center_challenge_relationships_from_dict = GameCenterChallengeRelationships.from_dict(game_center_challenge_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


