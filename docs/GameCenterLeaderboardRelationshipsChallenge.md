# GameCenterLeaderboardRelationshipsChallenge


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**RelationshipLinks**](RelationshipLinks.md) |  | [optional] 
**data** | [**GameCenterChallengeVersionRelationshipsChallengeData**](GameCenterChallengeVersionRelationshipsChallengeData.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_leaderboard_relationships_challenge import GameCenterLeaderboardRelationshipsChallenge

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterLeaderboardRelationshipsChallenge from a JSON string
game_center_leaderboard_relationships_challenge_instance = GameCenterLeaderboardRelationshipsChallenge.from_json(json)
# print the JSON string representation of the object
print(GameCenterLeaderboardRelationshipsChallenge.to_json())

# convert the object into a dict
game_center_leaderboard_relationships_challenge_dict = game_center_leaderboard_relationships_challenge_instance.to_dict()
# create an instance of GameCenterLeaderboardRelationshipsChallenge from a dict
game_center_leaderboard_relationships_challenge_from_dict = GameCenterLeaderboardRelationshipsChallenge.from_dict(game_center_leaderboard_relationships_challenge_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


