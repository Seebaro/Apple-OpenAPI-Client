# GameCenterLeaderboardCreateRequestDataRelationships


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**game_center_detail** | [**GameCenterAchievementReleaseRelationshipsGameCenterDetail**](GameCenterAchievementReleaseRelationshipsGameCenterDetail.md) |  | [optional] 
**game_center_group** | [**GameCenterAchievementRelationshipsGameCenterGroup**](GameCenterAchievementRelationshipsGameCenterGroup.md) |  | [optional] 
**game_center_leaderboard_sets** | [**GameCenterLeaderboardCreateRequestDataRelationshipsGameCenterLeaderboardSets**](GameCenterLeaderboardCreateRequestDataRelationshipsGameCenterLeaderboardSets.md) |  | [optional] 

## Example

```python
from openapi_client.models.game_center_leaderboard_create_request_data_relationships import GameCenterLeaderboardCreateRequestDataRelationships

# TODO update the JSON string below
json = "{}"
# create an instance of GameCenterLeaderboardCreateRequestDataRelationships from a JSON string
game_center_leaderboard_create_request_data_relationships_instance = GameCenterLeaderboardCreateRequestDataRelationships.from_json(json)
# print the JSON string representation of the object
print(GameCenterLeaderboardCreateRequestDataRelationships.to_json())

# convert the object into a dict
game_center_leaderboard_create_request_data_relationships_dict = game_center_leaderboard_create_request_data_relationships_instance.to_dict()
# create an instance of GameCenterLeaderboardCreateRequestDataRelationships from a dict
game_center_leaderboard_create_request_data_relationships_from_dict = GameCenterLeaderboardCreateRequestDataRelationships.from_dict(game_center_leaderboard_create_request_data_relationships_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


