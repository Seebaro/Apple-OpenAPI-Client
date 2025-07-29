# GameCenterLeaderboardLocalizationRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**game_center_leaderboard** | [**GameCenterChallengeCreateRequestDataRelationshipsLeaderboard**](GameCenterChallengeCreateRequestDataRelationshipsLeaderboard.md) |  | [optional] 
**game_center_leaderboard_image** | [**GameCenterLeaderboardLocalizationRelationshipsGameCenterLeaderboardImage**](GameCenterLeaderboardLocalizationRelationshipsGameCenterLeaderboardImage.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_leaderboard_localization_relationships import GameCenterLeaderboardLocalizationRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterLeaderboardLocalizationRelationships from a JSON string
game_center_leaderboard_localization_relationships_instance = GameCenterLeaderboardLocalizationRelationships.from_json(json)
# print the JSON string representation of the object
print(GameCenterLeaderboardLocalizationRelationships.to_json())

# convert the object into a dict
game_center_leaderboard_localization_relationships_dict = game_center_leaderboard_localization_relationships_instance.to_dict()
# create an instance of GameCenterLeaderboardLocalizationRelationships from a dict
game_center_leaderboard_localization_relationships_from_dict = GameCenterLeaderboardLocalizationRelationships.from_dict(game_center_leaderboard_localization_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


